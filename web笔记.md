[TOC]
# web笔记  
## 学习网站  
[MDN](https://developer.mozilla.org/zh-CN/)
[w3school](http://www.w3school.com.cn/)
[51CTO](http://edu.51cto.com/) 
[segmentfault](https://segmentfault.com/)
**网页访问过程** 
1、浏览器地址栏中输入相应的URL（协议、服务器地址/域名、资源路径）
2、根据URL在网络中找到对应的网页文件
3、浏览器将该网页文件展示成页面                                                                                                          **URL** 
统一资源定位符：是互联网标准资源的地址，可以从互联网上得到资源的位置和访问方法的简洁表示。
**B/S C/S** 
B/S:通过浏览器访问的网络应用程序
C/S:通过客户端应用软件访问的网络应用程序
优缺点：见PPT ch01-P21
**web浏览器**
显示网页内容，并让用户与这些文件交互的一种软件。
**web服务器** 
-物理设备：提供Web服务的计算机。
-软件：根据用户请求将信息资源传递给用户的应用程序。
-常用Web服务器：Apache和ngix服务器。
**万维网** 
web/WWW 全称World Wide Web
是一个由许多互相链接的超文本组成的系统，通过互联网访问。                                                                                **web开发过程**进行*网页页面制作*及其各项功能的开发 
项目提出----需求分析----设计：UI设计 ----开发：前端开发----系统测试----发布/维护
                                                   系统设计               后台开发
**超文本**
该文本中含有连接到其他文本的超链接

## HTML  
**Hyper Text Markup Language 超文本标记语言**
*  编程语言有逻辑
  标记语言无逻辑，是一套标记标签
### 基本结构  
```HTML
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8" />
    <title>Document</title>
</head>
<body>
</body>
</html>
```
### 标签及语法  
- <!-- --> 注释语法：也可以ctrl+?直接打出
- bgcolor 背景颜色
- text 文本颜色
- h1-h6 标题标签（双标签）输入h1按`tab`会自动补全
- &lt;p&gt;&lt;/p&gt;段落 
**自己找HTML实体(去网站）**
```HTML
<!--空白折叠--><!--HTML实体：&nbsp;-->
<p>&nbsp;&nbsp;为积极应对新冠肺炎疫情对就业工作带来的挑战和考验，全面贯彻落实学校就业工作决策部署，更大力度做好毕业生就业指导和服务工作，学期教育学院（旅游系）战疫情、守初心，多方发力，通过多措并举、分类施策和个性化辅导等方式，全面促进毕业生就业创业工作。</p>
```
> 段落p元素会自动在其前后创建一些空白
> 在&lt;h1 style="color:black;">可以定义文本颜色
- <img&gt;插入图片
> 绝对路径：e:\my_site\web\image\a.png
	优点：真实路径，定位清晰
	缺点：本机路径长，容易出错；如果站点文件夹移动，需要重新更改路径；
> 相对路径：同级目录：src="./图片名"
		图片在下一级目录：src="目录名称/图片名"
		图片在上一级目录:src="../图片名"
		图片在上上一级：src="../../图片名"
		优点：文件夹移动，其内部文件的相对路径不变
```HTML
<img src="图片路径" />
<!-- alt属性（为图片添加替换文本）-->
<img src="图片路径" alt="替换文本">
```
- 超链接：<a href="超链接路径"&gt;....</a&gt;
  target:在何处打开{_blank 在新窗口打开；__self 在当前窗口打开}
<target="_blank">
```HTML
<a href="">...</a>
<!--herf为空时，刷新页面-->
<a href="#">...</a>
<!--#防止页面刷新 跳转到页面的顶部-->
```
- **嵌套问题**
```HTML
<a href="http://www.baidu.com" target="_blank">
    <img src="image/baidu.jpg" alt="百度"/>
</a>
```
- 列表标签：有序列表：<ol&gt;双标签
		无序列表：<ul&gt;双标签 <li&gt;每个列表项
```HTML
<!--有序列表-->
<h2>
    这个学期的课程
</h2>
<ol>
    <li>web开发一</li>
    <li>程序设计基础</li>
</ol>
<!--无序列表-->
<ul>
    <li>web开发一</li>
    <li>程序设计基础</li>
</ul>
```
> 所有的标签必须关闭；
> 属性必须赋值；所有属性必须用引号括起来。
- <br /&gt;换行

- <hr /&gt;分割线

- <strong&gt;加强（加粗）

#### 表格和表单  

  (1)在HTML中没有列的概念，只有行的概念

  (2)<table&gt;</table&gt;表格标签	<tr&gt;</tr&gt;行标签
  	<th&gt;</th&gt;表头(默认加粗)	<td&gt;</td&gt;单元格标签

  (3)*table标签的相关属性:*

  ​	border:			表格边框的宽度

  ​	bordercolor:		表格边框的颜色

  ​	background:		表格的背景图

  ​	bgcolor:			表格的背景颜色

  ​	cellpadding:		表格边沿与其内容之间的距离

  ​	cellspacing:		单元格之间的空白

  ​	width:			表格元素的宽度

  ​	height:			表格元素的高度

  ​	align:			表格的对齐方式


> 在table中添加align:table相对于浏览器居中
> 

colspan:		跨列
rowspan:	 跨行
|标签|width|height|align|
|:-:|:-:|:-:|:-:|
|table|✓|✗|✓|
|tr|✗|✗|✓|
|td|✓|✓|✓|
|th|✓|✓|✓|

```HTML
 <table border="2" bordercolor="blue" bgcolor="yellow" cellpadding="10" cellspacing="20" >
     <caption>成绩单</caption>
		<tr>
			<th height="40">姓名</th>
			<th>年龄</th>
			<th>成绩</th>
		</tr>
		<tr>
			<td>历四百</td>
			<td>20</td>
			<td>100</td>
		</tr>
		<tr>
			<td rowspan="2">张三</td>
			<td colspan="2">100</td>
		</tr>
		<tr>
			<td>89</td>
			<td>99</td>
		</tr>
	</table>
```
(4)定义表格的主题
```HTML
<table>
    <caption>成绩单</caption>
</table>
```
```HTML
<table border="1px">
		<caption>支出证明单</caption>
		<tr>
			<td>支出事由</td>
			<td colspan="4"></td>
		</tr>
		<tr>
			<td>金额</td>
			<td colspan="4"></td>
		</tr>
		<tr>
			<td>单据</td>
			<td colspan="4"></td>
		</tr>
		<tr>
			<td>报销种类</td>
			<td colspan="4"></td>
		</tr>
		<tr>
			<td rowspan="2">批准人</td>
			<td>部门经理</td>
			<td></td>
			<td>喜用总监</td>
			<td></td>
		</tr>
		<tr>
			<td>财务总监</td>
			<td width="40px" height="10px"></td>
			<td>总经里</td>
			<td width="40px" height="10px"></td>
		</tr>
	</table>
```

(5)表单：表示文档中的一个区域，这个区域包含有交互控制元件，用来向Web服务器提交信息。
交互控制元件：文本框、下拉列表、单选框、复选框	
作用：从访问网站的用户那里获取信息，是用户向服务器传输数据的接口。

**所有表单控件都必须放在form标签之间，否则用户输入的信息无法提交到服务器**
#### input相关表单  
```HTML
<form><!--表示表单的开始和结束   定义一个表单-->
    <!--属性：action:规定向何处发送提交的表单数据。值（URL）
			method:规定以何种方式将表单数据传送到服务器。值（get会显示出来/post不会)-->
    <input type="text" name="名称" value="文本"  disabled/>
    <!--disabled为布尔属性，作用是不能在输入，也可以在提交时加上这个属性-->
    <!--当用户要在表单中键入字母数字等内容时用到的文本框  input不独占一行
            type:当为text时，输入框为文本输入框
		    name:为输入框命名，以备后台数据使用
			value:为输入框设置默认值，一般起到提示作用-->
    <input type="password" name="名称" value="000000"/>
</form>
```
```HTML
<form>
		用户名：<input type="text" name="username" value="请输入名字" /><br />
		密码： <input type="password" name="password" value="000000"/>
</form><!--可以在form中嵌套table做布局-->
```
```html
<form>
    <input type="radio" value="male" name="sex" checked />男
     <input type="radio" value="female" name="sex" />女
    <!--type="radio",控件为单选框
		value为提交数据到服务器的值
		name为控件命名
		checked添加时，该选项默认选中	为布尔属性（只有两种状态）
		单选框默认在一行-->
    
    <!--label属性可以将表单控件与文本关联在一起，即点击字也可以有相同效果-->
     <input type="radio" value="male" name="sex" checked id="male"/>
     <label for="male">男</label><!--显式绑定-->
     <label><input type="radio" value="female" name="sex" />女</label><!--隐式绑定-->
		
		<input type="checkbox" value="good1" name="goods" />
		I have a bike
		<input type="checkbox" value="good2" name="goods" />
		I have a car
    <!--type="checkbox",控件为复选框
		value为提交数据到服务器的值
		name为控件命名
		checked添加时，该选项默认选中-->
		
    提交文件
    <br /><!--用于文件上传-->
    <input type="file" name="files" /> 
</form>
```
```html
<!--提交表单信息到服务器按钮-->
<form>
    <input type="submit" value="提交" name="sub" />
</form>
<!--重置表单信息至初始状态按钮-->
<form>
    <input type="reset" value="重置" name="res" />
</form>
<!--普通按钮-->
<form>
    <input type="button" value="按钮" name="but" />
</form>
```
#### 多行文本域  
```html
<form>
    	<textarea name="cat" rows="3" cols="30">
            <!--rows文本区内可见行数
			   cols文本区内可见列数-->
    		The cat was playing in the garden.
    	</textarea>
    </form>
```
#### 下拉列表  
```html
<form>
    	<select name="class">
    		<option value="one" selected>软件一班</option>
    		<option value="two">软件二班</option>
    		<option value="three">软件三班</option>
    	</select>
</form>
<!--selected为布尔属性，默认选中选项
	value指定选项值-->
```
### 定义  

1. 单标签：无需表达范围，仅在标签作用处有效
  双标签：代表标签作用范围&lt;div>&lt;p>&lt;/P>&lt;/div>
2. 属性：charset="utf-8",开始标签
3. 统一规范小写
4. ctrl+n创建文件
5. ！（tab) 或html:5(tab)
6. 每一个网页背后都有一个网页文件
7. HTML语义化可以让页面的内容结构化，结构更清晰，便于对浏览器、搜索引擎解析

## CSS
**Cascading Style Sheets 层叠样式表**
CSS是用于控制网页形式并允许将样式与内容分离，尽行样式的修饰。
1. HTML控制元素样式的优点：针对元素样式设置的属性太少；修改元素麻烦；控制元素样式的代码冗余度过高。
2. CSS优点：更**专业**的样式修饰方法；更**简便**的样式修饰方法；更**简约**的布局方法。
3. CSS代码是由一条条语句构成，而每一条语句的结构都基本相同。
### 选择器  
规定该选择器定义的样式将对哪些元素生效
**ID选择器 > 类选择器 > 标签选择器**
**行内样式 > 页内样式 > 外部样式**
**就近原则，距离元素最近的样式优先级最高**
#### 标签选择器  
HTML标签选择器
```CSS
p{
    color:red;
}
```
#### 类选择器  
**权重值为10**
元素可以加入多个类。把各个类名放在class属性中，各个类名之间用一个空格分隔，类名的顺序不重要。

```CSS
.red{
    color:blue;
}
.red.green{
    color:red;
}
<p class="red">这是一个文图</p>
<p class="red green">这都我看过很多技术</p>
```
#### ID选择器  
**权重值为100**
**单一页面中，一个id选择器只能使用一次**

```css
#red{
    color:red;
}
<p id="red">这是一个问题</p>
```
###  css样式  
#### 行内样式  

通过style属性添加样式，指定网页中个别元素的显示效果。
style="属性：属性值；属性：属性值；···"
*不符合样式与内容分离的原则，不推荐使用。*

#### 页内标签  
在head内的style标签内添加样式，对页面某些标签或元素设置样式风格。

控制当前页面样式，维护较困难。

style标签可以有多个

#### 外部样式  
引用外部建立的.css文件
可同时控制多个页面，适用于各类大型网站，可用性最强，推荐使用。

```html
<head>
	<link rel="stylesheet" type="text/css" href="样式文件路径" >
    <!--stylesheet样式表	-->
</head>
```
#### 其他选择器  
[w3school](https://www.w3school.com.cn/css/css_selector_type.asp)
**通配符选择器:权重为0**
```html
*{
    color:red;
}
<!--*可以控制文档中每个元素-->
```
**属性选择器**
```html
*[title]{color:red;}
a[href][title]{color:red;}
img[alt]{border:5px solid red;}
```
**后代选择器**
```html
ul li{
    color:red;
}
```
**子元素选择器**

只能选择作为某元素子元素的元素

```html
h1 >strong{color:red;}
```
1. **叠加**
2. **可继承性**
3. **！importment允许开发人员强制应用某样式**
4. em是相对于父元素而言的。
	. normal 常规样式	italic 斜体样式
### 语法  

#### 

```html

```