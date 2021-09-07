# Thrift IDL 定义

本章主要包括 Thrift IDL 相关知识，并将带你手动写一些结构体和实现（后续章节里将使用过程宏生成这些代码）。

## 0x00 什么是 IDL 以及为什么需要 IDL

IDL 是 RPC 的必要组成部分，是客户端和服务端对通信的数据结构和调用方法的约定。

举例来说，我们有一个结构体想要发送接收：

```
struct User {
    name: String,
    password: String,
}
```

我们可以使用一个自定义的语言来描述这个定义：

这里 `struct` 和 `str` 都是自定义的类型。

```
struct User {
    1: str,
    2: str,
}
```

之前群里有人吐槽：golang 的 RPC 框架要用 IDL 生成代码好麻烦，还要跑专门的工具；为什么不基于 HTTP，用户自定义 json 结构体，收消息然后自行解析？ 实际上 RPC 框架是封装了消息收发、结构体编解码、IDL->结构体生成，以及一些服务治理逻辑。

与 golang 不同之处在于，在 rust 中我们可以利用 build.rs 来基于 IDL 生成结构体和结构体实现，代码生成会在后面章节讲到。利用这一点，就可以做到：

1. 生成代码不会被 Git 管理，不会插入用户 src 文件夹
2. 框架便于更新升级，不会受制于用户未重新生成代码导致的问题（这一点在 golang 下尤为致命）
3. 代码生成全自动，不需要用户手动运行脚本

## 0x01 Thrift IDL 定义

下文主要是从官方文档抄来的。

使用 BNF 表示：

- `+` 表示出现一次或多次
- `*` 表示出现零次或多次
- `|` 表示选择，第一个命中的会被选中

### 标识符

```
Identifier      ::=  ( Letter | '_' ) ( Letter | Digit | '.' | '_' )*
Letter          ::=  ['A'-'Z'] | ['a'-'z']
Digit           ::=  ['0'-'9']
```

标识符定义为 以字母或下划线开头，由字母、数字、点或下划线组成。举例来说，`bytedance` 和 `_bytedance123` 都是标识符，但 `1user` 不是。

### 字面量

```
Literal         ::=  ('"' [^"]* '"') | ("'" [^']* "'")
```

字面量由双引号或单引号包裹。例如 `"yyds"`就是一个字面量，字面量是不分类型的。

### 基础类型

```
BaseType        ::=  'bool' | 'byte' | 'i8' | 'i16' | 'i32' | 'i64' | 'double' | 'string' | 'binary' | 'slist'
```

基础类型有上述几种，含义基本看名字就知道（其中 slist 已 deprecated）。

### 容器类型

```
ContainerType   ::=  MapType | SetType | ListType
MapType         ::=  'map' CppType? '<' FieldType ',' FieldType '>'
SetType         ::=  'set' CppType? '<' FieldType '>'
ListType        ::=  'list' '<' FieldType '>' CppType?
CppType         ::=  'cpp_type' Literal

FieldType       ::=  Identifier | BaseType | ContainerType
```

其中 CppType 是用 `'cpp_type'` 声明的字面量（用法不详，应该是 fb 内部使用）。

容器类型包括 Map、Set 和 List。

Map 定义例如 `map < string, string >`，其中 key 和 value 类型都是 FieldType， 可以是 Identifier、BaseType 和 ContainerType（也就是说，类型是可以嵌套的，map 也可以是 map 的 key）。 Set 和 List 类似，区别在于 Set 存储不重复的无序元素而 List 允许重复且有序，在此不赘述。

### 常量类型

```
ConstValue      ::=  IntConstant | DoubleConstant | Literal | Identifier | ConstList | ConstMap
IntConstant     ::=  ('+' | '-')? Digit+
DoubleConstant  ::=  ('+' | '-')? Digit* ('.' Digit+)? ( ('E' | 'e') IntConstant )?
ConstList       ::=  '[' (ConstValue ListSeparator?)* ']'
ConstMap        ::=  '{' (ConstValue ':' ConstValue ListSeparator?)* '}'
```

常量可以是 Int、Double、List 和 Map，也可以是 Literal 和 Identifier。Double 可以带小数点，可以使用科学计数法。

### Enum、Union 和 Struct

```
Enum            ::=  'enum' Identifier '{' (Identifier ('=' IntConstant)? ListSeparator?)* '}'
Struct          ::=  'struct' Identifier 'xsd_all'? '{' Field* '}'
Union           ::=  'union' Identifier 'xsd_all'? '{' Field* '}'
Exception       ::=  'exception' Identifier '{' Field* '}'
```

可用于对结构体的定义。Enum 是枚举类型，Struct 是结构体，Union 类似 C 语言里的 Union 只包含一个 child，Exception 是自定义的错误信息描述。

### Function

```
Function        ::=  'oneway'? FunctionType Identifier '(' Field* ')' Throws? ListSeparator?
FunctionType    ::=  FieldType | 'void'
Throws          ::=  'throws' '(' Field* ')'

Field           ::=  FieldID? FieldReq? FieldType Identifier ('=' ConstValue)? XsdFieldOptions ListSeparator?
FieldReq        ::=  'required' | 'optional' 
FieldID         ::=  IntConstant ':'
ListSeparator   ::=  ',' | ';'
Throws          ::=  'throws' '(' Field* ')'
```

FunctionType 可以是 FieldType（前文提到过，包括 Identifier、BaseType 和 ContainerType）也可以是 `void`，它表示了 function 的返回值定义。

Identifier 是 function 的名字。

括号里是参数列表，由多个 Field 描述。

每个 Field 由 FieldID FieldReq FieldType 描述（如 `1: required bool are_we_ready (=false);`、`i32 user_count,`）。

Function 整体描述如：`void func1() throws (XXException)`、`i32 get_user_count(1: Paid paid);`

### Service

```
Service         ::=  'service' Identifier ( 'extends' Identifier )? '{' Function* '}'
```

Service 是由多个 Function 构成的。

### Definition

```
Definition      ::=  Const | Typedef | Enum | Senum | Struct | Union | Exception | Service
Document        ::=  Header* Definition*
Header          ::=  Include | CppInclude | Namespace
```

Document 由 Header 和 Definition 组成，即 `Const | Typedef | Enum | Senum | Struct | Union | Exception | Service` 可在 IDL 中被顶层定义。

## 0x03 写一个 Thrift IDL 并翻译成 Rust

我们设想一个从数据库 select 用户的需求，可选地提供 user_id 或 user_name 或性别，返回多个 User。

```
namespace rust demo

struct User {
    1: required i32 id,
    2: required string user_name,
    3: required bool is_male,

    10: optional map<string, string> extra,
}

struct GetUserRequest {
    1: i32 user_id,
    2: string user_name,
    3: bool is_male,
}

struct GetUserResponse {
    1: required list<User> users,
}

service ItemService {
    GetUserResponse GetUser (1: GetUserRequest req),
}
```

手动翻译一下 IDL：

```
use std::collections::HashMap;

#[derive(Debug, Clone, Default, PartialEq)]
pub struct User {
    user_id: i32,
    user_name: String,
    is_male: bool,

    extra: Option<HashMap<String, String>>,
}

#[derive(Debug, Clone, Default, PartialEq)]
pub struct GetUserRequest {
    user_id: i32,
    user_name: String,
    is_male: bool,
}

#[derive(Debug, Clone, Default, PartialEq)]
pub struct GetUserResponse {
    users: Vec<User>,
}
```

注：只生成了基本结构体，Service 未生成。

Thrift 的基本结构在 Rust 中往往有相对应的东西，可以直接映射一下。

另外，Thrift 的 Map 转换为了 rust 中的 HashMap 其实是有一定问题的，因为 Map 也可以作为另一个 Map 的 Key，而 HashMap 本身是不可 Hash 的。 这个问题我们暂时搁置，因为当前并没有将 Map 作为 Key 使用。这个在后续代码生成时可以考虑两个方案：

1. 全部使用 BTreeMap
2. 判断是否作为 Key 使用，如未作为 Key 则生成 HashMap，否则使用 BTreeMap

## 参考链接

- Thrift IDL 定义： https://thrift.apache.org/docs/idl.html
- 一些额外的定义解释： https://erikvanoosten.github.io/thrift-missing-specification/
