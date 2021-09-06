# Rust结构体

结构体是使用者定义的资料型别，由不同资料型别的变数组成。通过在结构体名称之前使用 结构体成员包含在大括号内。在大括号内，结构体成员定义了它们的名称和型别，结构成员也称为栏位。`struct`

结构体语法：

```rust
struct Student  
{  
    member-variable1;  
    member-variable2;  
    .  
    .  
}
```

在上面的语法中，结构体是使用关键字 结构体包含不同型别的变数。`struct`

宣告结构体的范例 -

```rust
let user = Student{  
// key:value pairs;  
}
```

在上面的宣告中，它通过使用结构名称然后使用大括号来定义。大括号包含键：值对，其中键是栏位的名称，`user``Student``value`

下面程式码建立一个员工结构体：

```rust
struct Employee{  
    employee_name : String,  
    employee_id: u64,  
    employee_profile: String,  
    active: bool,  
}
```

员工结构体范例：

```rust
let employee = Employee{  
    employee_name : String::from("Akshay Gupta"),  
    employee_id: 12,  
    employee_profile : String::from("Computer Engineer"),  
    active : true,  
};
```

**如何存取结构体的成员变数？可以使用点( 假设想要存取**
`.``Employee``employee_name`

```rust
employee.employee_name;
```

> 注意：如果想通过使用点表示法来更改特定栏位的值，那么必须使范例可变，因为Rust不允许特定栏位为可变栏位。

```rust
let mut employee = Employee{  
    employee_name : String::from("Akshay Gupta"),  
    employee_id: 12,  
    employee_profile : String::from("Computer Engineer"),  
    active : true,  
};  
employee.employee_name = String :: from("Akhil Gupta");
```

在函式体中建立范例：

```rust
fn create_employee(name:String, profile:String)  
{  
    Employee{  
        employee_name:name,  
        employee_id:12,  
        employee_profile:profile,  
        active:true,  
    }  
}
```

在上面的范例中，在函式体中隐式建立了 函式返回具有给定名称和组态档案的`Employee``create_employee()``Employee`

当传递给函式和栏位的引数具有相同名称时，使用栏位初始化简写。

当变数和栏位具有相同的名称时，Rust提供了使用栏位初始化简写的灵活性。不需要重复栏位和变数。

```rust
 fn create_employee(employee_name:String, employee_profile:String)  
{  
    Employee{  
        employee_name,  
        employee_id:12,  
        employee_profile,  
        active:true,  
    }  
}
```

在上面的范例中，引数和栏位的名称相同。因此，不需要编写`employee_name:employee_name``employee_name`
