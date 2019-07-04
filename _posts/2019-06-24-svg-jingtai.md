---
title: svg的静态效果展示
categories:
  - SVG制作
tags:
  - svg
---

#### Catch the Star
### 击中你的星！
- 请用鼠标悬停在星星上，查看效果
<head>
  <meta charset="UTF-8">
  <style>
    .star9 {
        width: 150px;
        height: 150px;
        color: yellow;    }
    .star9:hover {
		width: 150px;
		  height: 150px;
		  color: red;
    }
  </style>
</head>

<body>
<svg class="star9" viewBox="0 0 576 512">
 <path fill="currentColor" d="M259.3 17.8L194 150.2 47.9 171.5c-26.2 3.8-36.7 36.1-17.7 54.6l105.7 103-25 145.5c-4.5 26.3 23.2 46 46.4 33.7L288 439.6l130.7 68.7c23.2 12.2 50.9-7.4 46.4-33.7l-25-145.5 105.7-103c19-18.5 8.5-50.8-17.7-54.6L382 150.2 316.7 17.8c-11.7-23.6-45.6-23.9-57.4 0z"></path></svg>
</body>

## 使用CSS3给星星建立一个边框 

- 使用**border-radius**属性，给星星增加一个圆角边框
- 可以根据**border-radius**后的四个值分别对边框的四个角的圆角值进行调整，详细请看（[CSS圆角](https://www.w3cschool.cn/css3/css3-border-radius.html)）
- 请用鼠标悬停在星星上，查看效果
<head>
  <meta charset="UTF-8">
  <style>
    .star1 {
        width: 150px;
        height: 150px;
        color: yellow;    }
    .star1:hover {
    border:2px solid ;
    padding:10px 40px; 
    background: red;
    width:150px;
    border-radius:25px;
    }
  </style>
</head>

<body>
<svg class="star1" viewBox="0 0 576 512">
 <path fill="currentColor" d="M259.3 17.8L194 150.2 47.9 171.5c-26.2 3.8-36.7 36.1-17.7 54.6l105.7 103-25 145.5c-4.5 26.3 23.2 46 46.4 33.7L288 439.6l130.7 68.7c23.2 12.2 50.9-7.4 46.4-33.7l-25-145.5 105.7-103c19-18.5 8.5-50.8-17.7-54.6L382 150.2 316.7 17.8c-11.7-23.6-45.6-23.9-57.4 0z"></path></svg>
</body>

- 使用**box-shadow**属性，给星星添加阴影（具体可在**盒阴影**内容中查看）
- 请用鼠标悬停在星星上，查看效果
<head>
  <meta charset="UTF-8">
  <style>
    .star2 {
        width: 150px;
        height: 150px;
        color: yellow;    
     }
   .star2:hover {
     width:150px;
     height:150px;
     box-shadow: 10px 10px 5px #888888;
     }
  </style>
</head>

<body>
<svg class="star2" viewBox="0 0 576 512">
  <path fill="currentColor" d="M259.3 17.8L194 150.2 47.9 171.5c-26.2 3.8-36.7 36.1-17.7 54.6l105.7 103-25 145.5c-4.5 26.3 23.2 46 46.4 33.7L288 439.6l130.7 68.7c23.2 12.2 50.9-7.4 46.4-33.7l-25-145.5 105.7-103c19-18.5 8.5-50.8-17.7-54.6L382 150.2 316.7 17.8c-11.7-23.6-45.6-23.9-57.4 0z"></path></svg>
</body>

## 使用CSS3给星星增加一个渐变背景

- 使用**rgba( )**函数来定义颜色结点,用来创建减弱变淡效果的背景
- 请用鼠标悬停在星星上，查看效果
<head>
  <meta charset="UTF-8">
  <style>
    .star3 {
        width: 150px;
        height: 150px;
        color: yellow;        
  }
   .star3:hover {
    height: 150px;
    background: -webkit-linear-gradient(left, rgba(255,0,0,0), rgba(255,0,0,1)); 
    background: -o-linear-gradient(right, rgba(255,0,0,0), rgba(255,0,0,1)); 
    background: -moz-linear-gradient(right, rgba(255,0,0,0), rgba(255,0,0,1)); 
    background: linear-gradient(to right, rgba(255,0,0,0), rgba(255,0,0,1)); 
  </style>
</head>

<body>
<svg class="star3" viewBox="0 0 576 512">
  <path fill="currentColor" d="M259.3 17.8L194 150.2 47.9 171.5c-26.2 3.8-36.7 36.1-17.7 54.6l105.7 103-25 145.5c-4.5 26.3 23.2 46 46.4 33.7L288 439.6l130.7 68.7c23.2 12.2 50.9-7.4 46.4-33.7l-25-145.5 105.7-103c19-18.5 8.5-50.8-17.7-54.6L382 150.2 316.7 17.8c-11.7-23.6-45.6-23.9-57.4 0z"></path></svg>
</body>

- 使用**background: linear-gradient(direction, color-stop1, color-stop2, ...);**函数来定义颜色结点,用来创建创建一个线性渐变的背景

<head>
  <meta charset="UTF-8">
  <style>
    .star4 {
	    height: 150px;
		color: yellow;
    background: -webkit-linear-gradient(red, orange); 
    background: -o-linear-gradient(red, orange); 
    background: -moz-linear-gradient(red, orange);
    background: linear-gradient(red, orange);      
	}
  </style>
</head>

<body>
<svg class="star4" viewBox="0 0 576 512">
	<path fill="currentColor" d="M259.3 17.8L194 150.2 47.9 171.5c-26.2 3.8-36.7 36.1-17.7 54.6l105.7 103-25 145.5c-4.5 26.3 23.2 46 46.4 33.7L288 439.6l130.7 68.7c23.2 12.2 50.9-7.4 46.4-33.7l-25-145.5 105.7-103c19-18.5 8.5-50.8-17.7-54.6L382 150.2 316.7 17.8c-11.7-23.6-45.6-23.9-57.4 0z"></path></svg>
</body>

<head>
  <meta charset="UTF-8">
  <style>
    .star5 {
	    height: 150px;
		color: yellow;
    background: -webkit-linear-gradient(left, red , orange);
    background: -o-linear-gradient(right, red, orange);
    background: -moz-linear-gradient(right, red, orange);
    background: linear-gradient(to right, red , orange);
	}
  </style>
</head>

<body>
<svg class="star5" viewBox="0 0 576 512">
	<path fill="currentColor" d="M259.3 17.8L194 150.2 47.9 171.5c-26.2 3.8-36.7 36.1-17.7 54.6l105.7 103-25 145.5c-4.5 26.3 23.2 46 46.4 33.7L288 439.6l130.7 68.7c23.2 12.2 50.9-7.4 46.4-33.7l-25-145.5 105.7-103c19-18.5 8.5-50.8-17.7-54.6L382 150.2 316.7 17.8c-11.7-23.6-45.6-23.9-57.4 0z"></path></svg>
</body>

<head>
  <meta charset="UTF-8">
  <style>
    .star6 {
	    height: 150px;
		color: yellow;
    background: -webkit-linear-gradient(left top, orange , red); 
    background: -o-linear-gradient(bottom right, orange, red); 
    background: -moz-linear-gradient(bottom right, orange, red);
    background: linear-gradient(to bottom right, orange , red); 
	}
  </style>
</head>

<body>
<svg class="star6" viewBox="0 0 576 512">
	<path fill="currentColor" d="M259.3 17.8L194 150.2 47.9 171.5c-26.2 3.8-36.7 36.1-17.7 54.6l105.7 103-25 145.5c-4.5 26.3 23.2 46 46.4 33.7L288 439.6l130.7 68.7c23.2 12.2 50.9-7.4 46.4-33.7l-25-145.5 105.7-103c19-18.5 8.5-50.8-17.7-54.6L382 150.2 316.7 17.8c-11.7-23.6-45.6-23.9-57.4 0z"></path></svg>
</body>

- 使用**background: radial-gradient(center, shape size, start-color, ..., last-color);**函数来定义颜色结点,用来创建创建一个重复线性渐变的背景

<head>
  <meta charset="UTF-8">
  <style>
    .star7 {
	    height: 150px;
		color: yellow;
    background: -webkit-repeating-linear-gradient(red, orange 10%, green 20%); 
    background: -o-repeating-linear-gradient(red, orange 10%, green 20%);
    background: -moz-repeating-linear-gradient(red, orange 10%, green 20%);
    background: repeating-linear-gradient(red, orange 10%, green 20%); 
	}
  </style>
</head>

<body>
<svg class="star7" viewBox="0 0 576 512">
	<path fill="currentColor" d="M259.3 17.8L194 150.2 47.9 171.5c-26.2 3.8-36.7 36.1-17.7 54.6l105.7 103-25 145.5c-4.5 26.3 23.2 46 46.4 33.7L288 439.6l130.7 68.7c23.2 12.2 50.9-7.4 46.4-33.7l-25-145.5 105.7-103c19-18.5 8.5-50.8-17.7-54.6L382 150.2 316.7 17.8c-11.7-23.6-45.6-23.9-57.4 0z"></path></svg>
</body>

<head>
  <meta charset="UTF-8">
  <style>
    .star8 {
		color: yellow;
    height: 150px;
    width: 150px;
    background: -webkit-radial-gradient(red, orange, green); 
    background: -o-radial-gradient(red, orange, green); 
    background: -moz-radial-gradient(red, orange, green); 
    background: radial-gradient(red, orange, green);
	}
  </style>
</head>

<body>
<svg class="star8" viewBox="0 0 576 512">
	<path fill="currentColor" d="M259.3 17.8L194 150.2 47.9 171.5c-26.2 3.8-36.7 36.1-17.7 54.6l105.7 103-25 145.5c-4.5 26.3 23.2 46 46.4 33.7L288 439.6l130.7 68.7c23.2 12.2 50.9-7.4 46.4-33.7l-25-145.5 105.7-103c19-18.5 8.5-50.8-17.7-54.6L382 150.2 316.7 17.8c-11.7-23.6-45.6-23.9-57.4 0z"></path></svg>
</body>

#### 详细请看[CSS渐变](https://www.w3cschool.cn/css3/oj26bfli.html)



#### 总结
- 要完成一个简单的静态的svg制作，相对比较容易。首先要确定好你的svg图案，图案可从[Font awesome网站](https://fontawesome.com/icons?d=gallery)上寻找并下载到本地，再进行修改。
- 其次要思考，我们需要制作出什么样的效果，并根据需求进行背景的颜色搭配和样式选择，熟记相关属性来抓住这颗星星吧！
