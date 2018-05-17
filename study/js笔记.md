---
typora-copy-images-to: Pictures
---

# 深入浅出Javascript

## Javascript初步

### JS简介

#### 1.JS简介

一种显示在HTML中的脚本语言，能够实现网页内容的交互显示，能够让网页动起来。

JavaScript一种直译式脚本语言，是一种动态类型、弱类型、基于原型的语言，内置支持类型。它的解释器被称为JavaScript引擎，为浏览器的一部分，广泛用于客户端的脚本语言，最早是在HTML（标准通用标记语言下的一个应用）网页上使用，用来给HTML网页增加动态功能。 

特点：

- 是一种解释性脚本语言（代码不进行预编译）。
- 主要用来向[HTML]（[标准通用标记语言]下的一个应用）页面添加交互行为。 
- 可以直接嵌入HTML页面，但写成单独的[js]文件有利于结构和行为的分离。
- 跨平台特性，在绝大多数浏览器的支持下，可以在多种平台下运行（如Windows、Linux、Mac、Android、iOS等）。

#### 2.如何使用Javascript

​	1.通过<scrip></script>中直接编写

```js
<script type='text/javascript'>  
	alert('你好老茂')
</script>
```

​	2.通过<script src='目标文档URL'></script>链接外部的Js文件

​		<script src="script/js/test1.js" type="text/javascript" charst="utf-8"></scrip>

​	3.作为某个元素的事件属性值或者超链接的href属性值

​		<a href = javascript:confirm('您确认要报名学习Javascript课程吗？')></a>

#### 3.代码屏蔽

```
<script type='text/javascript'>
<!--
	js代码
//-->
</script>
```

有一些浏览器不支持js代码，那么添加的注释就不会执行js代码，如果浏览器支持，那么就会注释模块执行js代码。如果浏览器不支持js，可以使用<noscript></noscript>标签，显示noscript中的内容。

#### 4.Jascript基础语法

- js执行顺序：按照在HTML中出现的顺序依次执行。（如果需要在HTML文件执行函数或者全局变量，最好将其放在HTML的头部中。<head>）
- 大小写敏感：js严格区分大小写。
- 忽略空白和换行符：Js会忽略关键字、变量名、数字、函数名或其他各种元素之间的空格、制表符或换行符。*我们可以使用缩进、换行来使代码整齐，提升可读性*
- 语句分隔符
  1. 使用 ; 结束语句 *尽量保证代码每一句都有结束符，养成良好代码习惯*
  2. 可以把多个语句写在一行
  3. 最后一个语句的分号可以省略，但尽量不要省略
  4. 可以使用{}括成一个语句组，形成一个块block
- 通过 \ 对代码进行折行操作： 'document.write(' hello\world');'
- 注释
  1. 单行注释//
  2. 多行注释/* 注释内容 */
- [Javascript中的保留字](http://www.w3school.com.cn/js/pro_js_reservedwords.asp) 命名的时候尽量避开保留字，否则会产生冲突、歧意、报错等。
- 通过document.write()向文档书写内容
- 通过console.log()向控制台写入内容
- JavaScript中的报错
  1. 语法错误：通过控制台进行调试
  2. 逻辑错误：通过alert()进行调试

## Javascript面向对象编程

## Javascript进阶



