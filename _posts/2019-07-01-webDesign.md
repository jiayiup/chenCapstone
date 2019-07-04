---
layout: page
title: "从最基础的布局上手——页面结构"
categories:
  - 平面设计
---


- 想要制作一个网页，首先我们要知道最基础的布局——页面结构


### DOCTYPE声明
`<!DOCTYPE html>`

- 用来告诉浏览器使用什么样的HTML或XHTML规范来解析网页

### 字符编码的声明
`<meta charset="UTF-8">`

- 它用来描述当前页面的特性，例如文档字符集，即上图中的charset="utf-8"。
- “utf-8”是指一种字符集名称，被称为“万国码”，“utf-8”为默认的字符集，这让页面在世界上的几乎所有地区都能正常显示。

### 用于布局的标签

#### 页眉
`<header></header>`

#### 主要的内容栏
`<main></main>`

#### 左侧（浏览）栏
`<aside></aside>`

#### 页脚
`<footer></footer>`

- 在进行页面布局时，我们可以把以上的标签结合起来。
- 
> 将各功能用块元素包裹起来，这样可以简化布局工作,于是页面就由一棵元素树组成

![页面布局元素树](https://assets.gitee.com/jiayichen/jiayichen/raw/5295a5f7abf4cb194eda49ec243a510431a679d3/assets/images/yuansushu.png)

### 制作出一个完成的HTML页面
```yml
<!DOCTYPE html>
<html>
	<head>
		<meta charset="UTF-8">
			<title>一个页面</title>
	</head>
	
	<body>
		<header>
			<h1>页面</h1>       
		</header>
		
		<nav>
			<a href="">首页</a>|
			<a href="">平面设计</a>|
			<a href="">网页设计</a>|
			<a href="">SVG制作</a>|
		</nav>
		
		<article>
			<hgroup >
				<h1>学习页面结构</h1>
				<h3>页面结构标签</h3>
			</hgroup>
				
			<aside>
			这是一篇学习页面结构的文章
			</aside>
		
			<section>
				<p>这是一个简单例子</p>         
			</section>
		</article>
		
		<footer> &copy;2019-陈嘉仪个人学习网站</footer>
	</body>
 </html>

```

- 以下是效果：

*****

<html>
	<head>
		<meta charset="UTF-8">
			<title>一个页面</title>
	</head>
	
	<body>
		<header>
			<h1>页面</h1>       
		</header>
		
		<nav>
			<a href="http://jiayichen.gitee.io/">首页</a>|
			<a href="http://jiayichen.gitee.io/jiayichen/categories/%E5%B9%B3%E9%9D%A2%E8%AE%BE%E8%AE%A1/">平面设计</a>|
			<a href="http://jiayichen.gitee.io/jiayichen/categories/%E7%BD%91%E7%AB%99%E8%AE%BE%E8%AE%A1/">网页设计</a>|
			<a href="http://jiayichen.gitee.io/jiayichen/categories/%E7%BD%91%E7%AB%99%E8%AE%BE%E8%AE%A1/">SVG制作</a>|
		</nav>
		
		<article>
			<hgroup >
				<h1>学习页面结构</h1>
				<h3>页面结构标签</h3>
			</hgroup>
				
			<aside>
			这是一篇学习页面结构的文章
			</aside>
		
			<section>
				<p>这是一个简单例子</p>         
			</section>
		</article>
		
		<footer> &copy;2019-陈嘉仪个人学习网站</footer>
	</body>
 </html>
 
 *****