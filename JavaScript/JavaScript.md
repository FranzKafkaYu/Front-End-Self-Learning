# 基础知识

JavaScript与Python一样属于解释性语言而非编程性语言，用于在网页中定义用户与网页的交互行为。如拖动、滑动、弹框等等。

JavaScript以\<script\>作为开始，以\</script\>作为结束。在这两个标签之间的内容则是JavaScript的内容。但通常我们会将\<script\>与\</script\>及两者之间的内容一起称为JavaScript。

JavaScript的内容通常会放在\<head\>或者\<body\>中

如放在\<head\>中：

\<!DOCTYPE html\>

\<html\>

\<head\>

\<script\>

function myFunction()

{

document.getElementById("demo").innerHTML="我的第一个 JavaScript 函数";

}

\</script\>

\</head\>

\<body\>

\<h1\>我的 Web 页面\</h1\>

\<p id="demo"\>一个段落\</p\>

\<button type="button" onclick="myFunction()"\>尝试一下\</button\>

\</body\>

\</html\>

如放在\<body\>中：

\<!DOCTYPE html\>

\<html\>

\<body\>

\<h1\>我的 Web 页面\</h1\>

\<p id="demo"\>一个段落\</p\>

\<button type="button" onclick="myFunction()"\>尝试一下\</button\>

\<script\>

function myFunction()

{

document.getElementById("demo").innerHTML="我的第一个 JavaScript 函数";

}

\</script\>

\</body\>

\</html\>

除了直接放在html中，我们也可以将JavaScript的内容单独保存为一个后缀为.js格式的文件，然后在html中进行引用。

如下所示：

scriptExample.js

function JavaScriptFunction()

{

document.getElementById(“demo”).innerHTML=”我的第一个JavaScript函数”;

}

需要注意的是，在单独的.js文件内是不需要\<script\>与\</script\>标签的。

我们在html文件中引用上述JavaScript代码：

\<!DOCTYPE html\>

\<html\>

\<body\>

\<script src=" scriptExample.js"\>\</script\>

\</body\>

\</html\>

在JS中，同样使用//作为行注释

## 数据类型

基本类型：字符串（string）、数字（number）、布尔（Boolean）、对空（Null）、未定义（Undefined）、Symbol

对象类型：对象（Object）、数组（Array）、函数（Function），还有两个特殊的对象正则与日期

## 变量

变量：使用var关键字来定义变量，使用=来为变量进行赋值。在JS中，变量必须以字母开头，而且变量对字母大小写敏感。

我们可以在一条语句内声明多个变量，该语句以var开头，并使用逗号进行隔开。

关于变量的修饰符，有两个关键字：let与const。let声明的变量只在let所在的代码块内有效。而const声明一个只读的常量，一旦声明，常量的值就不可改变。

关于全局变量：在函数外（function关键字）声明的变量作用域是全局的。全局变量在JavaScript程序的任何地方都是可以访问的。

关于局部变量：在函数内声明的变量作用域是局部的

## 对象

在JavaScript中，几乎所有的事物都是对象。对象也是一个变量，但对象可以包含多个值（多个变量），每个值以name:value的形式存在。

如这样一个例子：var car={name:”Fiat”,model:500,color:”red”}

在Js中，数据类型可以多种，但在表现形式上分为两类：文本与数值，文本通常以单引号或者双引号进行表示，而数值则以普通的数字表示

访问对象属性时通过.进行访问，如person.lastName

对象方法时包含在对象的方法，类似与面向对象编程的成员函数这个概念。在Js中定义对象方法如下所示：

methodName：

## 函数

## 输出与打印

JavaScript自身没有任何打印或者输出的函数。

JavaScript可以通过不同的方式来输出数据：

1.  使用window.alert()弹出警告框

2.  使用document.write()方法将内容写到HTML文档中

3.  使用innerHTML写入到HTML元素

4.  使用console.log()写入到浏览器的控制台

如使用window.alert()进行弹框提醒：

弹框提示数值12

\<!DOCTYPE html\>

\<html\>

\<body\>

\<h1\>我的第一个页面\</h1\>

\<p\>我的第一个段落。\</p\>

\<script\>

window.alert(12);

\</script\>

\</body\>

\</html\>

弹框提示字符串，需要通过双引号进行引用

\<!DOCTYPE html\>

\<html\>

\<body\>

\<h1\>我的第一个页面\</h1\>

\<p\>我的第一个段落。\</p\>

\<script\>

window.alert(“这是一个弹框提醒”);

\</script\>

\</body\>

\</html\>
