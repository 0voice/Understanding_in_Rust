# Rust结构体方法语法

方法类似于函式，因为它们在 方法还包含引数和返回值。但是，当在 这些方法的第一个引数始终是`start``then``fn``struct``self`

## 定义方法

在`struct`

```rust
struct Square  
{  
    a : u32,  
}  
impl Square  
{  
    fn area(&self)->u32  
    {  
        self.a * self.a  
    }  
}  

fn main()  
{  
    let square = Square{a:10};  
    print!("Area of square is {}", square.area());  
}
```

执行上面范例程式码，得到以下结果 -

```shell
Area of square is 100
```

当在`struct``impl`

```rust
impl Square  
{  
    fn area(&self)->u32  
    {  
        self.a * self.a  
    }  
}
```

第一个引数是签名中的`self`

在这里，使用方法语法来呼叫 方法语法是一个范例，后跟点运算子，方法名称，引数和任何引数。`area()`

```rust
square.area();
square`是范例，`area()
```

> 注意：如果想要更改呼叫该方法的范例，那么使用`&mut self``&self`

**方法语法的优点：**

使用方法语法而不是函式的主要优点是，与范例相关的所有资料都放在`impl``impl`
