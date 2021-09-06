# Rust for回圈

```
for`回圈是条件回圈，即回圈执行特定次数。Rust语言中 执行`for``for
```

for回圈的语法 -

```rust
for var in expression  
{  
    //block statements  
}
```

在上面的语法中，表示式可以转换为叠代器，叠代器遍历资料结构的元素。在每次叠代中，都从叠代器中获取值。当没有剩余值被提取时，回圈结束。

下面来看一个简单的例子。

```rust
 fn main()  
{  

  for i in 1..11  
  {  
    print!("{} ",i);  
  }   
}
```

执行上面范例程式码，得到以下结果 -

```shell
1 2 3 4 5 6 7 8 9 10
```

在上面的范例中，上限是不包含的，因此回圈将列印`1..11``1``10`

下面再来看一个简单的例子。

```rust
fn main()  
{  
    let mut result;  
    for i in 1..11  
    {  
        result=2*i;  
        println!("2*{}={}",i,result);  
    }  
}
```

执行上面范例程式码，得到以下结果 -

```shell
2*1=2
2*2=4
2*3=6
2*4=8
2*5=10
2*6=12
2*7=14
2*8=16
2*9=18
2*10=20
```

在上面的例子中，`for``2`

下面来看另一个简单的例子。

```rust
fn main(){
 let fruits=["mango","apple","banana","litchi","watermelon"];  
 for a in fruits.iter()  
 {  
   print!("{} ",a);  
 }
}
```

执行上面范例程式码，得到以下结果 -

```
mango apple banana litchi watermelon
```

在上面的例子中，当它到达阵列的最后一个元素，那么回圈就结束了。`iter()``fruits`

**while回圈和for回圈的区别：因此，可以说**
`while``for``for`
