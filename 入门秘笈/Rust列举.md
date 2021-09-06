# Rust列举

列举是一种自定义资料型别，包含一些确定的值。它在列举名称之前使用 它还包括方法。`enum`

列举的语法：

```rust
enum enum_name  
{  
  variant1,  
  variant2,  
  .
  .
}
```

在上面的语法中，`enum_name``variant1``variant2``..`

例如：

```rust
enum Computer_language{
  C,  
  C++,  
 Java,
}
```

在上面的例子中，`computer_language``C``C++``Java``computer_language`

## 列举值

下面建立每个变数的范例，如下所示：

```rust
let c = Computer_language::C;  
let cplus = Computer_language::C++;  
let java = Computer_language::Java;
```

在上面的场景中，分别建立了包含值 列举的每个变体都在其识别符号下命名，并使用双冒号。这很有用，因为`C``C++``Java``c``cplus``java``Computer_language::C``Computer_language::C++``Computer_language::Java``Computer_language`

还可以在特定范例上定义函式，定义采用`Computer_language`

```rust
fn language_type(language_name::Computer_language);
```

任何变体都可以呼叫此函式：

```rust
language_type(Computer_language::C++);
```

通过一个例子来理解。

```c
enum Employee {  
    Name(String),  
    Id(i32),  
    Profile(String),  
}  
fn main() {  

    let n = Employee::Name("Hema".to_string());  
    let i = Employee::Id(2);  
    let p = Employee::Profile("Computer Engineer".to_string());  
    println!(" {:?} s {:?} b {:?}", n,i,p);  
}
```

执行上面范例程式码，得到以下结果 -

```shell
Name("Hema") s Id(2) b Profile("Computer Engineer")
```

在上面的范例中，`Employee``Name(String)``Id(i32)``Profile(String)``:?`
