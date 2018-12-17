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

undefined和null是不一样的  
null是空，赋值为空  
undefined是没有赋值，只是声明  

```javascript
var persion;
typeof persion  // 输出 undefined
var car = null;
typeof car;     // 输出 null
```

## JavaScript类型转换

```JavaScript
Number()    // 转换为数字
String()    // 转换为字符串
Boolean()   // 转化为布尔值

// 在 JavaScript 中有5种不同的数据类型：
string
number
boolean
object
function

{}
// 上面这条不要在意，目的为了不影响下main这些

// 在 JavaScript 中有 3 种对象类型：  
Object
Date
Array

// 在 JavaScript 中有 2 个不包含任何值的数据类型：  
null  
undefined  

typeof "John"                 // 返回 string
typeof 3.14                   // 返回 number
typeof NaN                    // 返回 number
typeof false                  // 返回 boolean
typeof [1,2,3,4]              // 返回 object
typeof {name:'John', age:34}  // 返回 object
typeof new Date()             // 返回 object
typeof function () {}         // 返回 function
typeof myCar                  // 返回 undefined (如果 myCar 没有声明)
typeof null                   // 返回 object
```

## constructor 属性

constructor 属性返回所有 JavaScript 变量的构造函数。  

```JavaScript
"John".constructor                 // 返回函数 String()  { [native code] }
(3.14).constructor                 // 返回函数 Number()  { [native code] }
false.constructor                  // 返回函数 Boolean() { [native code] }
[1,2,3,4].constructor              // 返回函数 Array()   { [native code] }
{name:'John', age:34}.constructor  // 返回函数 Object()  { [native code] }
new Date().constructor             // 返回函数 Date()    { [native code] }
function () {}.constructor         // 返回函数 Function(){ [native code] }
```

|方法|描述|
|----|----|
getDate()|从 Date 对象返回一个月中的某一天 (1 ~ 31)。
getDay()|从 Date 对象返回一周中的某一天 (0 ~ 6)。
getFullYear()|从 Date 对象以四位数字返回年份。
getHours()|返回 Date 对象的小时 (0 ~ 23)。
getMilliseconds()|返回 Date 对象的毫秒(0 ~ 999)。
getMinutes()|返回 Date 对象的分钟 (0 ~ 59)。
getMonth()|从 Date 对象返回月份 (0 ~ 11)。
getSeconds()|返回 Date 对象的秒数 (0 ~ 59)。
getTime()|返回 1970 年 1 月 1 日至今的毫秒数。