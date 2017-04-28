# 01节-html

## 一、html简介

- 超文本标记语言（Hyper Text Markup Language）, 是一种 **标记语言**（与 **编程语言** 相对应）

## 二、html书写规范

> <html><br>
> 	<head><br>
> 		包括资讯信息 : 整个页面的属性, 指导浏览器解析标签,引入外部文件的标签<br>
>   </head><br>
>		<body><br>
> 		我们需要展示的内容<br>		
> 	</body><br>
> </html><br>

---

## 三、html基本标签

- ### 1、文件标签（结构标签）
  - <html> : 根标签
    - <head>
    - <title> : 页面的标题
	<body text="green" bgcolor="black" background="images/...jpg">
		↓↓↓
	text : 文本的颜色  为绿
	bgcolor : 背景色  为黑
	background : 背景图片  某张jpg（在 bgcolor 的上层）

	另 : 颜色写法:
	① 单词 : red  green  black
	② rgb : rgb(0,0,0)	0~255
	③ 十六进制 : #000000 黑色	#ffffff 白色	# 3245b3(通过ColorPicker拾取颜色)

	尺寸写法:
	① ?px -> 多少像素
	② ?%  -> 占百分比	区别 : 百分比会随着标签大小进行动态改变

2、排版标签
	① 注释标签 <!-- -->
	② 换行标签 <br/>
	③ 段落标签 <p align="left / center / right"></p>	注:段与段之间有空行
	④ 水平线标签 <hr width="长度(px) / %" size="粗度px" color="颜色" align="默认为center">

3、块标签
	① 行级块标签 : <div> (默认占据一整行)	-> div+css布局
	② 行内块标签 : <span> (仅占据一行一部分)	-> 进行友好提示

4、文字标签
	① 基本标签 : <font color="red" size="最小1,最大7,默认3" face="黑体">
	② 标题标签 : <h1>-<h6>	数字↑字体↓,默认加粗,并占据一行

5、清单标签
	① 无序列表 : <ul type="默认disc / square / circle">
			    <li> : 列表项
	② 有序列表 : <ol type="1,A,a,I,i" start="开始位置的数字">

	作用 : 网页菜单(结合css修饰)

6、图形标签
	<img src="images/...jpg" width="70%" height="70%" border="5" align="top/middle/bottom与文本相对位置" alt="文字说明" />

7、链接标签
	<a href="地址" name="锚点名称" target="默认_self本页打开 / _blank空白页打开">

	作用 :
	①页面跳转
		注 : 访问外网资源,前面必须加协议 http://,否则访问本地相对位置

	②锚点访问
		访问锚点的时候 书写格式 href="#name的值"	# 代表本页

8、表格标签
	<table border="2" width="50%" align="center" bgcolor="blue">
		<caption>表格标题</caption>
		<tr align="center">
			<th>表头(默认居中加粗)</th>
			<td colspan="列合并" rowspan="行合并">单元格</td>	// 可进行布局
	<thead>
	<tbody>
	<tfoot>		优化加载，增强用户体验
