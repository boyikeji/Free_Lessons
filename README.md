![秦皇岛博易科技](/images/logo3.jpg)

----------
## 博易科技免费课程（一）

### **扫一扫二维码立即添加微信公众号**

![微信二维码](/images/weixin2Dcode.jpg)

---

### 本节免费课程内容：

1. [常用html标签](#demo01-常用html标签)
1. [常用css样式](#demo02-常用css样式)
1. [css语法](#demo03-css语法)
1. [元素分类](#demo04-元素分类)
1. [元素浮动](#demo05-元素浮动)
1. [菜单](#demo06-菜单)
1. [div浮动](#demo07-div浮动)
1. [css嵌入方式](#demo08-css嵌入方式)
1. [伪类选择器](#demo09-伪类选择器)
1. [网页结构](#demo10-网页结构)
1. [盒模型](#demo11-盒模型)
1. [居中](#demo12-居中)
1. [自适应](#demo13-自适应)
1. [定位](#demo14-定位)


----------

## Demo01: 常用html标签

>* [展示](https://boyikeji.github.io/Free_Lessons_01/demo01/index.html)
>* [资源](https://github.com/boyikeji/Free_Lessons_01/blob/master/demo01/index.html)

### 本节介绍html的常用标签：
1. `<h1>`~`<h6>`为标题标签：标题标签根据标题的程度划分等级，一共六个等级；各标签的区别在于字体大小的不同。
![h标签](/images/h.gif)
2. `<p>`为段落标签：当文字形成段落的时候需要使用p标签。
![p标签](/images/p.gif)
3. `<ul>`为列表标签：当内容需要使用列表形式呈现的时候，需要使用列表标签；同时ul需要和li标签共同使用。
![ul标签](/images/ul.gif)
4. `<a>`为超链接标签：href为链接的目标。
5. `<img>`为图片插入标签：src属性指定了显示图像的URL(统一资源定位符:获取资源位置路径)。

### 代码展示：

````html	
	<h1>我的第一个网页</h1>
	<h2>选择题</h2>
	<h3>第一题</h3>
	<p>你喜欢哪一个水果？</p>
	<ul>
		<li>A:香蕉</li>
		<li>B:苹果</li>
		<li>C:鸭梨</li>
		<li>D:水蜜桃</li>
	</ul>
	<h3>第二题</h3>
	<p>你喜欢哪一项运动？</p>
	<ul>
		<li>A:篮球</li>
		<li>B:足球</li>
		<li>C:排球</li>
		<li>D:乒乓球</li>
	</ul>
	<h3>第二题</h3>
	<p>你喜欢哪一张图片？</p>
	<ul>
		<li>A:<img src="../images/logo1.png"></li>
		<li>B:<img src="../images/logo2.png"></li>
		<li>C:<img src="../images/logo3.png"></li>
	</ul>
````

## Demo02: 常用css样式

>* [展示](https://boyikeji.github.io/Free_Lessons_01/demo02/index.html)
>* [资源](https://github.com/boyikeji/Free_Lessons_01/blob/master/demo02/index.html)

### 本节介绍常用css样式：

1. 属性名为color:设置文本的颜色。

	`{color:red;}`

2. 属性名为back-ground:设置元素的背景颜色。

	`{background:blue;}`

3. 属性名为font-size:设置字体的大小。

	`{font-size:12px;}`

4. 属性名为width:设置元素的宽度。

	`{width:100px;}`

5. 属性名为height:设置元素的宽度。

	`{height:80px;}`

style样式内的代码展示：
````css
	h1{
		color:red;
	}
	h2{
		background-color: yellow;
	}
	.question{
		background-color: green;
		color:white;
		font-size: 30px;
	}
	#first-img{
		width:80px;
		height:80px;
	}
````

## Demo03: css语法

>* [展示](https://boyikeji.github.io/Free_Lessons_01/demo03/index.html)
>* [资源](https://github.com/boyikeji/Free_Lessons_01/blob/master/demo03/index.html)

### 本节介绍css语法：

1. 通用选择器：css语法中使用`*`表示。

	`*{color:red;}`

2. id选择器：css语法中使用`#`表示。

	`#my-id{background:blue;}`

3. 类选择器：css语法中使用`.`表示。

	`.my-class{font-size:20px;}`

4. 派生选择器：依据元素在其位置的上下文关系来定义样式。

	`#list li{color:green;}`

代码展示：

````html

	<!DOCTYPE html>
	<html lang="en">
	<head>
		<meta charset="UTF-8">
		<title>Document</title>
		<style type="text/css">
			/*通用选择器*/
			/**{color:red;}*/
			h1{
				color:red;
			}
			#my-id{
				color:blue;
			}
			.my-class{
				color:yellow;
			}
			#list li{
				color:green;
			}
	
		</style>
	</head>
	<body>
		<h1>标签（元素）选择器</h1>
		<h2 id="my-id">id选择器</h2>
		<h3 class="my-class">class（类）选择器</h3>
		<ul id="list">
			<li>香蕉</li>
			<li>苹果</li>
			<li>鸭梨</li>
		</ul>
		<ul>
			<li>足球</li>
			<li>篮球</li>
			<li>羽毛球</li>
		</ul>
	</body>
	</html>
````

## Demo04: 元素分类

>* [展示](https://boyikeji.github.io/Free_Lessons_01/demo04/index.html)
>* [资源](https://github.com/boyikeji/Free_Lessons_01/blob/master/demo04/index.html)

### 本节介绍元素的分类：

1. 块元素：独立成行。`{display:block}`，常见标签`<h1>`~`<h6>`/`<p>`/`<ul>`/`<li>`/`<div>`
2. 行级元素(内联元素)：和其他元素在一行，不可以设置宽高。顶部、底部边距不能设置。具体宽高是内部文字或图片的宽高。`{display:inline}`，常见标签`<a>`/`<span>`
3. 内联块元素：元素的宽高可以设置，上下边距可以设置，可以与其他元素在一行。`{display:inline-block}`

代码展示：

````html

	<!DOCTYPE html>
	<html lang="en">
	<head>
	<meta charset="UTF-8">
	<title>Document</title>
	<style type="text/css">
		*{
			margin:0px;
			padding:0px;
		}
		.e-a{
			margin-top:100px; /*a标签设置上下边距没有作用*/
			margin-left:100px;
			padding-top:100px; /*a标签设置上下边距没有作用*/
			padding-left:100px;
		}
		p{
			text-indent: 100px;
		}
		.box-inline{
			width:100px;
			height:100px;
			border:1px solid #f00;
			display: inline;
		}
		.box-inline-block{
			
			height:100px;
			border:1px solid #f00;
			display: inline-block;
		}
		.big-box{

		}
		.box{
			width:100px;
			height:100px;
			border:1px solid #f00;
			float: left;
		}

	</style>
	</head>
	<body>
		<!-- 块元素：独立成行.display:block -->
		<div>div标签</div>
		<h1>标题一</h1>
		<h2>标题二</h2>
		<h3>标题三</h3>
		<h4>标题四</h4>
		<h5>标题五</h5>
		<h6>标题六</h6>
		<ul>
		    <li>列表一</li>
		    <li>列表二</li>
		    <li>列表三</li>
		</ul>
		<p>这是一个段落，是一个块元素！这是一个段落，是一个块元素！这是一个段落，是一个块元素！
			这是一个段落，是一个块元素！这是一个段落，是一个块元素！这是一个段落，是一个块元素！
			这是一个段落，是一个块元素！这是一个段落，是一个块元素！这是一个段落，是一个块元素！
			这是一个段落，是一个块元素！这是一个段落，是一个块元素！这是一个段落，是一个块元素！
			这是一个段落，是一个块元素！这是一个段落，是一个块元素！这是一个段落，是一个块元素！
			这是一个段落，是一个块元素！这是一个段落，是一个块元素！这是一个段落，是一个块元素
		</p>
		<p>这是一个段落，是一个块元素！这是一个段落，是一个块元素！这是一个段落，是一个块元素！
			这是一个段落，是一个块元素！这是一个段落，是一个块元素！这是一个段落，是一个块元素！
			这是一个段落，是一个块元素！这是一个段落，是一个块元素！这是一个段落，是一个块元素！
		</p>
		<!-- 内联元素：和其他元素在一行，不可以设置宽高。顶部、底部边距不能设置。具体宽高是内部文字或图片的宽高。
		display:inline -->
		<a class="e-a" href="">链接<span class="e-span">可以给span单独添加样式</span></a>
		<div>
			<a href="">这是一个a</a>
			<a href="">这也是一个a</a>
		</div>
		<!-- 内联块元素:元素的宽高可以设置，上下边距可以设置，可以与其他元素在一行。
		    display:inline-block -->
		<img src="" alt="显示图片">
		<div>
			<img src="../images/logo1.png" alt="">
			<img src="../images/logo2.png" alt="">
		</div>
		<div class="big-box-inline">
			<div class="box-inline">asdfasdf</div>
			<div class="box-inline">asdfsadf</div>
			<div class="box-inline">asdfsadf</div>
		</div>
		<div class="big-box-inline-block">
			<div class="box-inline-block">asdfas dfsafs afs af safaf</div>
			<div class="box-inline-block">asdfsadf</div>
			<div class="box-inline-block">asdfsadf</div>
		</div>
		<div class="big-box">
			<div class="box">asdfas dfsafs afs af safaf</div>
			<div class="box">asdfsadf</div>
			<div class="box">asdfsadf</div>
		</div>
	</body>
	</html>
````

## Demo05: 元素浮动

>* [展示](https://boyikeji.github.io/Free_Lessons_01/demo05/index.html)
>* [资源](https://github.com/boyikeji/Free_Lessons_01/blob/master/demo05/index.html)

### 本节介绍元素浮动：

在样式中设置元素浮动：`{float:left;}`

代码展示：

````html

	<!DOCTYPE html>
	<html lang="en">
	<head>
		<meta charset="UTF-8">
		<title>Document</title>
		<style type="text/css">
			#list li{
				float:left;
				border:1px solid #f00;
				list-style: none;
			}
		</style>
	</head>
	<body>
		<ul id="list">
			<li>香蕉</li>
			<li>苹果</li>
			<li>鸭梨</li>
		</ul>
	</body>
	</html>

````

## Demo06: 菜单

>* [展示](https://boyikeji.github.io/Free_Lessons_01/demo06/index.html)
>* [资源](https://github.com/boyikeji/Free_Lessons_01/blob/master/demo06/index.html)

### 本节介绍菜单的原理：

代码展示：

````html

	<!DOCTYPE html>
	<html lang="en">
	<head>
		<meta charset="UTF-8">
		<title>Document</title>
		<style type="text/css">
			#nav{
				list-style:none;
	
			}
			#nav li{
				float:left;
				width:80px;
			}
	
		</style>
	</head>
	<body>
		<ul id="nav">
			<li>主页</li>
			<li>视频</li>
			<li>图片</li>
			<li>新闻</li>
			<li>游戏</li>
		</ul>
	</body>
	</html>

````

## Demo07: div浮动

>* [展示](https://boyikeji.github.io/Free_Lessons_01/demo07/index.html)
>* [资源](https://github.com/boyikeji/Free_Lessons_01/blob/master/demo07/index.html)

### 本节介绍div浮动：

代码展示：

````html

	<!DOCTYPE html>
	<html lang="en">
	<head>
		<meta charset="UTF-8">
		<title>Document</title>
		<style type="text/css">
			*{
				margin:0;
				padding:0;
			}
			.box{
				width:200px;
				height:200px;
				float:left;
			}
			.box1{
				background-color:red;
			}
			.box2{
				background-color:green;
			}
			.box3{
				background-color:blue;
			}
			.box4{
				background-color:black;
			}
			.box5{
				background-color:yellow;
			}
		</style>
	</head>
	<body>
		<div class="box box1"></div>
		<div class="box box2"></div>
		<div class="box box3"></div>
		<div class="box box4"></div>
		<div class="box box5"></div>
	</body>
	</html>

````

## Demo08: css入门

>* [展示](https://boyikeji.github.io/Free_Lessons_01/demo08/index.html)
>* [资源](https://github.com/boyikeji/Free_Lessons_01/blob/master/demo08/index.html)

### 本节介绍css基础：

1. css插入形式：内联样式（写在标签内部）；嵌入样式（写在头文件中）；外部样式（独立成css样式文件）
2. 语法：选择器{属性名:属性值;}

代码展示：

````html

	<!DOCTYPE html>
	<html lang="en">
	<head>
		<meta charset="UTF-8">
		<title>Document</title>
		<style type="text/css">
			#first-css{
				color:red;
			}
		</style>
	</head>
	<body>
		<h1 id="first-css">hello css</h1>
	</body>
	</html>

````

## Demo09: 伪类选择器

>* [展示](https://boyikeji.github.io/Free_Lessons_01/demo09/index.html)
>* [资源](https://github.com/boyikeji/Free_Lessons_01/blob/master/demo09/index.html)

### 本节介绍伪类选择器：

语法：`#nav li:hover{background-color: red;}`

````html

	<!DOCTYPE html>
	<html lang="en">
	<head>
		<meta charset="UTF-8">
		<title>Document</title>
		<style type="text/css">
			#nav{
				list-style:none;
	
			}
			#nav li{
				float:left;
				width:80px;
				text-align: center;;
				height:30px;
				line-height: 30px;
			}
			#nav li:hover{
				background-color: red;
			}
	
		</style>
	</head>
	<body>
		<ul id="nav">
			<li>主页</li>
			<li>视频</li>
			<li>图片</li>
			<li>新闻</li>
			<li>游戏</li>
		</ul>
	</body>
	</html>

````

## Demo10: 网页结构

>* [展示](https://boyikeji.github.io/Free_Lessons_01/demo10/index.html)
>* [资源](https://github.com/boyikeji/Free_Lessons_01/blob/master/demo10/index.html)

### 本节介绍网页的结构：

* div通常命名规则

代码展示：

````html

	<!DOCTYPE html>
	<html lang="en">
	<head>
		<meta charset="UTF-8">
		<title>Document</title>
		<style type="text/css">
	
		</style>
	</head>
	<body>
		<div id="header">
			<div class="nav"></div>
			<div class="banner"></div>
		</div>
		<div id="container">
			<div class="left-col"></div>
			<div class="center-col"></div>
			<div class="right-col"></div>
		</div>
		<div id="footer"></div>
	</body>
	</html>

````

## Demo11: 盒模型

>* [展示](https://boyikeji.github.io/Free_Lessons_01/demo11/index.html)
>* [资源](https://github.com/boyikeji/Free_Lessons_01/blob/master/demo11/index.html)

### 本节介绍盒模型：

代码展示：

````html

	<!DOCTYPE html>
	<html lang="en">
	<head>
		<meta charset="UTF-8">
		<title>Document</title>
		<style type="text/css">
			*{
				margin:0;
				padding:0;
			}
			.box{
				width:300px;
				height:300px;
				border:1px solid red;
				float:left;
			}
			.box1{
				padding-top:20px;
				padding-bottom:20px;
				margin-right:20px;
			}
			.box2{
				margin-left:50px;
			}
		</style>
	</head>
	<body>
		<div class="box box1">
			<h1>内容1</h1>
		</div>
		<div class="box box2">
			<h1>内容2</h1>
		</div>
	</body>
	</html>

````

## Demo12: 居中

>* [展示](https://boyikeji.github.io/Free_Lessons_01/demo12/index.html)
>* [资源](https://github.com/boyikeji/Free_Lessons_01/blob/master/demo12/index.html)

### 本节介绍居中：

* 行内元素居中：设置父级为`{text-align:center;}`
* 定宽块元素居中：`{margin:0 auto;}`
* 不定宽块元素居中：需要套table，给table设置`{margin:0 auto;}`

代码展示：

````html

	<!DOCTYPE html>
	<html>
	  <head>
	    <meta charset="utf-8">
	    <title>居中</title>
	    <style type="text/css">
	      *{
	        margin:0;
	        padding:0;
	      }
	      .div-center{
	        text-align: center;/*居中文本,或行内元素*/
	      }
	      .box{
	        width:960px;
	        height: 200px;
	        background-color: #888;
	        margin:0 auto;/*定宽块元素居中*/
	        margin-bottom: 10px;
	      }
	      .no-width{
	        height: 200px;
	        background-color: #888;
	      }
	      .list-box{
	        margin:0 auto;
	      }
	      .list li{
	        list-style: none;
	        float: left;
	        margin-left:10px;
	      }
	    </style>
	  </head>
	  <body>
	    <h3>文本或行内元素的水平居中,可以设置父级text-align: center;</h3>
	    <div class="div-center">
	      一个居中的段落
	    </div>
	    <div class="div-center">
	      <img src="../1-html&css/images/1.jpg" alt="" />
	    </div>
	    <div class="div-center">
	        <a href="http://baidu.com">百度</a>
	    </div>
	    <h3>定宽块元素水平居中,可以通过设置margin:0 auto;</h3>
	    <div class="box">
	
	    </div>
	
	    <h3>不定宽块元素需要外面套table，然后给table设置margin:0 auto;</h3>
	    <table class="list-box">
	      <tr>
	        <td>
	          <ul class="list">
	            <li><a href="#">1</a></li>
	            <li><a href="#">2</a></li>
	            <li><a href="#">3</a></li>
	            <li><a href="#">4</a></li>
	          </ul>
	        </td>
	      </tr>
	    </table>
	
	  </body>
	</html>

````

## Demo13: 自适应

>* [展示](https://boyikeji.github.io/Free_Lessons_01/demo13/index.html)
>* [资源](https://github.com/boyikeji/Free_Lessons_01/blob/master/demo13/index.html)

### 本节介绍自适应：

* 不设置盒子高度,盒子可以适应内容高度

代码展示：

````html

	<!DOCTYPE html>
	<html>
	  <head>
	    <meta charset="utf-8">
	    <title></title>
	    <style type="text/css">
	      .box{
	        background-color: yellow;
	        /*height: 100px;*/
	      }
	    </style>
	  </head>
	  <body>
	      <h3>高度自适应</h3>
	      <div class="box">
	          <p>
	            你好这是一个测试.
	          </p>
	          <p>
	            你好这又是一个测试.
	          </p>
	          <p>
	            你好这又是一个测试.
	          </p>
	          <p>
	            你好这又是一个测试.
	          </p>
	      </div>
	  </body>
	</html>

````

## Demo14: 定位

### 本节介绍定位：

* 绝对定位：`{postion:absolute;}`

>* [展示](https://boyikeji.github.io/Free_Lessons_01/demo14/index-ab.html)
>* [资源](https://github.com/boyikeji/Free_Lessons_01/blob/master/demo14/index-ab.html)

代码展示：

````html

	<!DOCTYPE html>
	<html lang="en">
	<head>
		<meta charset="UTF-8">
		<title>Document</title>
		<style type="text/css">
			*{
				margin:0px;
				padding:0px;
			}
			#big-box{
				width:500px;
				height:500px;
				margin-left:50px;
				border:1px solid red;
			}
			.abs-box{
				width:100px;
				height:100px;
				position: absolute;
			}
			.box1{
				background-color: red;
				top:0px;
				left:0px;
				z-index: 999
			}
			.box2{
				background-color: blue;
				top:50px;
				left:50px;
				z-index: 0
			}
		</style>
	</head>
	<body>
		<div id="big-box">
			<div class="abs-box box1"></div>
			<div class="abs-box box2"></div>
		</div>
	</body>
	</html>

````

* 相对定位：`{position: relative;}`

>* [展示](https://boyikeji.github.io/Free_Lessons_01/demo14/index-rel.html)
>* [资源](https://github.com/boyikeji/Free_Lessons_01/blob/master/demo14/index-rel.html)

代码展示：

````html

	<!DOCTYPE html>
	<html>
	  <head>
	    <meta charset="utf-8">
	    <title></title>
	    <style type="text/css">
	      *{
	        margin:0px;
	        padding:0px
	      }
	      .big-box{
	        width:500px;
	        height:500px;
	        background-color: yellow;
	        margin:100px 0 0 200px;
	      }
	      .rel-box{
	        width:100px;
	        height:100px;
	        background-color: red;
	        position: relative;
	        top:150px;
	        left:350px;
	      }
	      .bot-box{
	        width:100px;
	        height:200px;
	        background-color: green;
	      }
	    </style>
	  </head>
	  <body>
	    <div class="big-box">
	
	    </div>
	    <div class="rel-box">
	
	    </div>
	    <div class="bot-box">
	
	    </div>
	  </body>
	</html>

````

* 固定定位 `{position:fixed;}`

>* [展示](https://boyikeji.github.io/Free_Lessons_01/demo14/index-fixed.html)
>* [资源](https://github.com/boyikeji/Free_Lessons_01/blob/master/demo14/index-fixed.html)

````html

	<!DOCTYPE html>
	<html>
	  <head>
	    <meta charset="utf-8">
	    <title></title>
	    <style type="text/css">
	      *{
	        margin:0px;
	        padding:0px;
	      }
	      .box{
	        height:500px;
	      }
	      .box1{
	        border:1px solid red;
	      }
	      .box2{
	        border:1px solid yellow;
	      }
	      .box3{
	        border:1px solid blue;
	      }
	      .fix-box{
	        height:30px;
	        width:800px;
	        background-color: green;
	        position: fixed;
	        top:0;
	        left:20%;
	      }
	    </style>
	  </head>
	  <body>
	    <div class="box box1">
	
	    </div>
	    <div class="box box2">
	
	    </div>
	    <div class="box box3">
	
	    </div>
	    <div class="fix-box">
	
	    </div>
	  </body>
	</html>

````

* 选择参照物定位：需要参照的元素`{position: relative;}`,需要定位的元素`{position: absolute;}`

>* [展示](https://boyikeji.github.io/Free_Lessons_01/demo14/index-rel-ab.html)
>* [资源](https://github.com/boyikeji/Free_Lessons_01/blob/master/demo14/index-rel-ab.html)

代码展示：

````html

	<!DOCTYPE html>
	<html>
	  <head>
	    <meta charset="utf-8">
	    <title></title>
	    <style type="text/css">
	      *{
	        margin:0px;
	        padding:0px;
	      }
	      .big-box{
	        width:500px;
	        height:500px;
	        background-color: yellow;
	        margin:100px 0 0 200px;
	        position: relative;
	      }
	      .rel-box{
	        width:100px;
	        height:100px;
	        background-color: red;
	        position: absolute;
	        top:0px;
	        left:0px;
	      }
	    </style>
	  </head>
	  <body>
	    <div class="big-box">
	      <div class="rel-box">
	
	      </div>
	    </div>
	  </body>
	</html>

````