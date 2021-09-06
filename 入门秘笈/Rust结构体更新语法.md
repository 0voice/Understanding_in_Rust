# Rust结构体更新语法

使用 当新范例使用旧范例的大部分值时，可以使用 考虑两名员工`Struct`
`struct update``employee1``employee2`

- 首先，建立`Employee``employee1`

```rust
let employee1 = Employee{  
    employee_name : String::from("Maxsu"),  
    employee_id: 12,  
    employee_profile : String::from("IT工程師"),  
    active : true,  
};
```

- 其次，建立 范例的某些值与 有两种方法可以宣告 第一种方法是在没有语法更新的情况下宣告`employee2``employee2``employee1``employee2`
  `employee2`

```rust
let employee2 = Employee{  
    employee_name : String::from("Maxsu"),  
    employee_id: 11,  
    employee_profile : employee1.employee_profile,  
    active : employee1.active,  
};
```

第二种方法是使用语法更新宣告`employee2`

```rust
let employee2 = Employee{  
    employee_name : String::from("Yiibai"),  
    employee_id: 11,  
    ..employee1  
};
```

语法`..`

下面来看一个结构的简单范例：

```rust
struct Triangle  
{  
    base:f64,  
    height:f64,  
}  

fn main()  
{  
    let triangle= Triangle{base:20.0,height:30.0};  
    print!("Area of a right angled triangle is {}", area(&triangle));  
}  

fn area(t:&Triangle)->f64  
{  
    0.5 * t.base * t.height  
}
```

执行上面范例程式码，得到以下结果 -

```shell
Area of a right angled triangle is 300
```

在上面的例子中，建立了三角形( 三角形(`Triangle``Triangle``main()`
