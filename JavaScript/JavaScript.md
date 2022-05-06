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
