Css 

--------------------------------------

1. 什么是css？

html 是姑娘，非常漂亮，但是没有穿衣服。

css 就是给这个姑娘穿上漂亮的衣服。


层叠样式表 (Cascading Style Sheets) 

<h1>你好</h1>  

字  --- 红色 

字  ---- 蓝色  

显示为蓝色  认为 蓝色把红色干掉了  错误的认识  

真确： 蓝色把红色给盖住了  -- 层叠


2. 如何使用css？

	① 在标签中使用style属性，将属性值设置为需要的css样式。
		<h1 style='color:red;'>
	② 通过style标签来设置css，需要将style标签放在head里面
		<style>
			h1 {
				color : red;
			}
		</style>
	③ 通过link标签引入外部的单独的css文件 
		<link rel="stylesheet" href="style.css">

	④ 通过@import url 方式引入单独css文件,这个用法必须写在style标签中
		<style>
			@import url('style.css')
		</style>

Tip:浏览器解析网页的时候，从上到下，从左向右
①②③三种引入css的方式都是遵从网页从上向下，从左向右的顺序，但是唯独④不一样，当浏览器解析网页的时候，碰到了④中方式，会先将它放到一旁不去管它，而是继续解析，直到把网页解析完成再去解析④方式引入的css。


html  结构  css 样式

结构与样式分离


3. css选择器 

html 网页的结构  --- > h1  div p 

css 是用来美化结构的。---想要美化必须要找到需要美化的标签


基础选择器：
1. html标签选择器  
	在style中直接写需要找的标签，例如
	h1 {
		color:red;
	}

	缺点：找到的标签不够精确。

2. id选择器

	在style中写#id明 ，如下：
	#p1 {
		color:red;
	}
	Tip：id值因为具有唯一性，所以说，尽量少用这种选择器。

3. class 选择器 

	class也是一个全局属性，所有的标签都可以使用这个属性.
	class属性值可以重复。

	在style中直接写.class名 ：如
	.d1 {
		color:red;
	}

***********id值和class值不要一样。*****************************
Tip:问题：
	当id选择器 ，class选择器 ，html标签选择器 三种选择器同时给一个标签设置相同属性的时候，这个标签的样式听谁的？


	作业： 代码3遍 
				 整理笔记
				 思考练习题