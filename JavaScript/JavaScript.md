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

## 数据类型

基本类型：字符串（string）、数字（number）、布尔（Boolean）、对空（Null）、未定义（Undefined）、Symbol

对象类型：对象（Object）、数组（Array）、函数（Function），还有两个特殊的对象正则与日期

变量：使用var关键字来定义变量，使用=来为变量进行赋值

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
