# Rust向量

向量是一种单一资料结构，可以在记忆体中彼此相邻地储存多个值。当有一个专案列表(例如：购物车中的资料项)时，向量很有用。

**要点：**

- 向量用于储存相同型别的值。
- 向量由`Vec <T>`
- `Vec <T>`由标准库提供，它可以储存任何型别的资料，其中`T`
- 向量的资料在堆上分配。
- 向量是一个可增长的阵列意味着可以在执行时新增新元素。

`Vec <T>` ：当向量保持特定型别时，它在角括号中表示。

## 如何建立向量？

可以使用`Vec::new()`

```rust
Let v : Vec<i32> = Vec::new();
```

在上面的宣告中，`v``i32``Vec::new()`

还有另一种建立向量的方法：

Rust提供`vec!`

例如：

```rust
let v = vec![10,20,30,40,50];
```

注意：如果想重复向量的初始值，那么还有另一种实现`vec`

```rust
let v = vec![2 ; i];
```

在上面的宣告中，向量`v``2``i`

## 存取元素

可以使用下标运算子`[]`

通过下面一个例子来理解：

```rust
fn main()  
{  
    let v =vec![20,30,40,50];  
    println!("first element of a vector is :{}",v[0]);  
    println!("Second element of a vector is :{}",v[1]);  
    println!("Third element of a vector is :{}",v[2]);  
    println!("Fourth element of a vector is :{}",v[3]);  
}
```

执行上面范例程式码，得到以下结果 -

```shell
first element of a vector is :20
Second element of a vector is :30
Third element of a vector is :40
Fourth element of a vector is :50
```

存取向量元素的第二种方法是使用`get(index)``vector``Option <＆t>`

看下面一个范例程式码 -

```rust
fn value(n:Option<&i32>)  
{  
    match n  
    {  
        Some(n)=>println!("Fourth element of a vector is {}",n),  
        None=>println!("None"),  
    }  
}  
fn main()  
{  
    let v =vec![20,30,40,50];  
    let a: Option<&i32>=v.get(3);  
    value(a);  
}
```

执行上面范例程式码，得到以下结果 -

```shell
Fourth element of a vector is 50
```

在上面的范例中，`get()`

## []和get()方法的区别：

当使用 因此，当尝试存取不存在的元素时，程式就会崩溃。如果尝试使用`[]``get()``None`

通过下面一个例子来理解这一点：

- get(index)函式

```rust
fn value(n:Option<&i32>)  
{  
 match n  
 {  
   Some(n)=>println!("Fourth element of a vector is {}",n),  
   None=>println!("None"),  
 }  
}  
fn main()  
{  
    let v =vec![20,30,40,50];  
    let a: Option<&i32>=v.get(7);  
    value(a);  
}
```

执行上面范例程式码，得到以下结果 -

```shell
None
```

- []运算子

```rust
fn main()  
{  
    let v =vec![20,30,40,50];  
    println!("{}",v[8]);  
}
```

执行上面范例程式码，得到以下结果 -

![img](https://tw511.com/upload/images/201910/20191014013932390.png)

## 叠代向量中的值

如果想要存取向量的每个元素，那么可以叠代向量的元素，而不是使用索引来存取向量的特定元素。

可以使用`for`

下面来看一个不可变参照的简单范例：

```rust
fn main()  
{  
    let v =vec![20,30,40,50];  
    print!("Elements of vector are :");  
    for i in v  
    {  
        print!("{} ",i);  
    }  
}
```

执行上面范例程式码，得到以下结果 -

```shell
Elements of vector are :20 30 40 50
```

下面来看一个可变参照的简单范例：

```rust
fn main()  
{  
    let mut v =vec![20,30,40,50];  
    print!("Elements of vector are :");  
    for i in &mut v  
    {  
        *i+=20;  
        print!("{} ",i);  
    }  
}
```

执行上面范例程式码，得到以下结果 -

```shell
Elements of vector are :20 30 40 50
```

在上面的例子中，改变向量的值。因此，向量是可变参考。在`i``*``v`

## 更新向量

当建立向量时，使用 在向量的末尾插入新元素。`push()``push()`

下面来看看一个简单的例子：

```rust
fn main()  
{  
  let mut v=Vec::new();  
  v.push('j');  
  v.push('a');  
  v.push('v');  
  v.push('a');  
  for i in v  
  {  
    print!("{}",i);  
  }  
}
```

执行上面范例程式码，得到以下结果 -

```shell
java
```

在上面的范例中，向量`push()``v`

## 删除向量

当向量超出范围时，它会自动删除或从记忆体中释放。通过一个简单的场景来理解这一点：

```rust
fn main()  
{  
   let v = !vec[30,40,50];  
} # => v 在這裡被釋放，因為它超出了範圍。
```

在上面的场景中，当向量超出范围时释放向量意味着将移除向量中存在的所有元素。

## 使用Enum储存多种型别

向量可以储存相同型别的元素，这是向量的一个很大的缺点。列举是一种自定义资料型别，它包含相同列举名称下的各种型别的变体。当想要将元素储存在不同型别的向量中时，使用列举型别。

下面通过一个例子来理解这一点：

```rust
#[derive(Debug)]  
enum Values {  
   A(i32),  
   B(f64),   
   C(String),  
}  

fn main()   
{  
     let v = vec![Values::A(5),   
     Values::B(10.7),Values::C(String::from("Yiibai"))];  
     for i in v  
    {  
       println!("{:?}",i);  
     }  
}
```

执行上面范例程式码，得到以下结果 -

```shell
A(5)
B(10.7)
C(Yiibai)
```

**在向量中使用列举的优点：**

- Rust在编译时知道向量元素的型别，以确定每个元素需要多少记忆体。
- 当向量由一个或多个型别的元素组成时，对元素执行的操作将导致错误，但使用带有匹配的列举将确保可以在执行时处理每个可能的情况。
