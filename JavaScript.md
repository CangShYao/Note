# JavaScript

## 对象和方法

```javascript
// 对象
var person = {
    firstName: "John",
    lastName : "Doe",
    id : 5566,
    fullName : function() {
       return this.firstName + " " + this.lastName;
    }
};

// 调用对象方法
person.fullName();

// 取出对象值
name=person.lastname;
name=person["lastname"];
```

## undefined和null

Undefined 这个值表示变量不含有值，定义了，但是没有初始化。  
可以通过将变量的值设置为 null 来清空变量。就是设为null  

```javascript
var person;
var car="Volvo";
var car=null
// print person -> undefined
// print car    -> Volvo
// print car    -> null
```