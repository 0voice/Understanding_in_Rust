# Rust if let控制流程

```
if let`语法用于组合 运算子和`if``let``「match」``「if let」
```

**匹配运算子的范例**

```rust
fn main()  
{  
    let a = Some(5);  
    match a {  
    Some(5) => println!("five"),  
    _ => (),  
}}
```

执行上面范例程式码，得到以下结果 -

```
five
```

在上面的范例中，匹配运算子在值等于 执行第一个变数后，如果使用`Some(5)``_ =>()``if``match`

**if let范例**

```rust
fn main()  
{  
    let a=Some(3);  
    if let Some(3)=a{  
     println!("three");  
    }
}
```

执行上面范例程式码，得到以下结果 -
```shell
three
```
