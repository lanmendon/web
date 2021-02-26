S的使用

html+teb健

右击，检查是开发者工具。
URL统一资源定位符。即网络地址
分为三步分：协议：HTTP；域名：资源路径。

![网页访问过程](E:\Users\大一下学期\周一直播PPT\Screenshot_20200217_102115_com.alibaba.android.ri.jpg)

## web的相关概念。

+ web指的是万维网。万维网是一个有许多相互连接的超文本组成的系统，通过互联网访问，又称网页。亦称“www”．
+ 万维网信息服务是依据客户端和服务器方式进行合作的。

​       ｗｅｂ浏览器展示网页内容，并让用户与这些文件交互的软 件。

+ web服务器：

​       URL遵守一个协议：HTTP协议

+ **网站访问过程：输入URL，找到服务器，反馈给浏览器代码，浏览器展现网页⭐

​      ｈｔｔｐ：／／ｔｅｃｈ．ｓｉｎａ．ｃｏｍ．ｃｎ／ｉｔ／ ｄｏｃ－ｉａｖｘ．ｈｔｍｌ
      协议　　　　　服务器地址（找到web服务器的IP地址）在it文件里的此文件，后缀名为ｈｔｍｌ．**

+ **网络应用程序架构：优缺点，例子。⭐

  + Ｂ／Ｓ通过浏览器访问的网络应用程序。可维护性更强。浏览器就是B/S中的B。可以维护升级。
    + 特点：
         1.无需安装特定客户端程序，通过URL访问。
         2.跨平台能力（Windows、Linux、Android、IOS…）。
         3.无缝升级，客户端免维护。
         4.（缺点）不能直接使用客户端硬件资源，用户体验单一。
   + Ｃ／Ｓ架构通过客户端访问的网络应用程序。
      + 特点：
        1(缺点).需要安装特定客户端程序。
        2.(缺点)针对不同平台开发不同版本。
        3.(缺点)升级应用须重新安装。
        4.(优点)能够直接使用客户端硬件资源。响应速度快，可构建大型3D效果应用
        5.(优点)信息安全控制能力强。


UI交互设计师，专门设计界面的。要懂心理学的内容。
O2O：指的是线上到线下。
项目提出：组织,公司高层。
需求分析：需求分析师/产品经理
        需求分析方法
        沟通能力、创新能力。
        成果：需求分析报告，产品原型
        需要时间的积累。。。。
设计：UI设计师做设计。
     系统设计：系统分析师；软件架构师（大牛要对每一步有很深的了解）。
开发：前端开发：将psd图
    静态页面：数据固定的
    动态页面：静态页面+数据更新。
    大部分网页都是动态网页。
    后台开发：后台开发工程师。需要数据库技术，不断更新。
测试：测试工程师：功能测试方法、自动化测试方法、压力测试方法
     用测试用例写测试报告。
上线：运维工程师：系统集成、部署，网络管理，数据库管理。
     维护无节假日！！！！！！
要学习理论；勤于动手（敲代码，**手写**代码）；掌握工具
不仅上课听，自己对知识点进行挖掘！！！！
参考内容：MDN参考手册 
        W3school参考手册。
        segmentfault网站专门解决程序员的问题。
        将代码托管到GitHub上。

+ index.html为首页。

## HTML 语法基础
+ HTML 基础语法，**三要素“词汇、语法、语义”**
+ HTML 的全称： 超文本标记语言。
  它不是一种编程语言而是一种标记语言。标记语言是一套标记标签。HTML 使用标记标签来描述网页。
+ HTML 标记标签通常被称为 HTML 标签，它是由尖括号包围的关键词，如<html>.
+ ctrl+?键注释
+ <!DOCTYPE html>为文档声明，告诉浏览器用HTML5来解释代码。必须放第一行。 <meta>必须写在<head>
+ HTML 元素指的是从开始标签到结束标签的所有代码。 
### 网页文件

+ **网页元素**是指构成网页的各项内容。 
+ 浏览器中看到的网页实质为：**网页文件**
+ 网页文件
   + 文本文件
   + 扩展名为 .html 或 .htm
   + 文件内容为 HTML 代码和文本内容


 ### 标签的分类
+ 双标签：由“开始标签”和“结束标签”两部分构成。结束标签比开始标签多了一个“/”（比如<body></body>），必须成对使用。/是结束符。
+ 单标签：在开始标签中进行关闭，即以开始标签的结束而结束（比如<meta/>）。斜杠就是表示关闭标签。

​        双标签因为需要控制范围，单表签仅在标签处有效。

+ HTML 标签可以拥有属性 ——为 HTML 元素提供附加信息

   属性书写形式：name = "value" （即名称/值对）
   属性书写位置：开始标签
   不同标签具有不同属性，属性之间要用空格隔开，与开始标签也要用空格隔开。
   <meta charset="UTF-8">
   <title>Document</title>都只能写在<title>中。

###  出现结构
1.ctrl+n 创建文件
2.ctrl+s 进行保存，后缀名为.html。
3.英文状态下的！+tab键就可以出来结构。
4.一个html文件只有1个基本结构.

### 标题及内容
浏览器中，标题独占一行。<h1>……</h1>至<h6>……</h6>默认加粗。
<p>   </p>标签是段落标签，独占一行。                   

### 插图片

+ <img/>单表签，插入图片。属性：src:指明存储图像的位置。alt:为图片添加替换文本。<img src="绝对路径/文件名"/  alt=“这是一张图">
+ 相对路径：
   •图片和网页在同级目录     src="./图片名"（./可省略）

   •图片在网页的下一级目录  src="目录名称/图片名"

   •图片在网页的上一级目录  src="../图片名"  ../表一级 ../../是上两级。

Ø优点：文件夹被移动，其内部文件的相对路径不变。 
注意：
  1.不要使用本机绝对路径，推荐使用相对路径
  2.图片文件单独存放在一个文件夹中
  3.图片文件夹与页面文件放在同一个目录下

属性：

  alt 属性用于指定图片的替换文字,当图片不能正常显示时,则显示 alt 中的文字,表达要传递的信息。（5分）

​    title 属性用于设置当前对象的说明信息。作用是当用户将鼠标指向图片时，提示给用户的信息。⭐

### 超链接

eg:<a href=" ww w. baidu.com"> 百度</a>

eg:<a  href="1.html" target= "_blank">1.html</a>

+ href 值为空时，表页面刷新

+ href值为#时表防止刷新，并跳转到页面顶部。
+ target="_blank"(在新窗口打开)
  target="_self"(在当前窗口打开)“默认状态”

### 列表

+ 无序列表<ul>双标签，默认表现为黑点。

   <li>写在里面 </li> 列表  独占一行

+ 有序列表<ol>双标签，默认表现为1. 2. 3.

   <li> </li> 列表  独占一行

+ <strong></strong>字体加粗。

+ <br />换行

+ <hr /> 分割线

## 第三章
### 网页中插入表格

+ html没有列的概念，只有行的概念。默认是没有边框的。

  <table border="1"></table>定义表格。只能嵌套行。

+ + table只能嵌套captionn tr
  + tr只能嵌套th td 
  + <tr></tr>一行写在里面。
  + <th></th>写表头，加粗。
  + <td></td>表一个单元格。

+ table标签里插的：

  属性：border:表格边框宽度；
              bordercolor:表格边框颜色；
              background:表格背景图；
              bgcolor：表格背景颜色；

  eg:<table border="1" 
  background="/i/eg_bg_07.gif">

  ​            cellspacing:单元格与单元格间距离
              cellpadding:单元格中文字与边缘的距离。

  ​            width :      规定表格元素的宽度（pixels或%）
              height :     规定表格元素的高度（pixels或%）

  ​            colspan ：跨列合并 colspan="2"
              rowspan:跨行合并 rowspan="2"

  ​            align：      表格的对齐方式（left  center  right)

  ​            align="center" left right

  ​            caption ：表格主题。

  ​            <caption>成绩单</caption>表格标题
             

###网页中插入表单
+ <form></form>表单区域，表单的开始和结束。<form></form>可以嵌套<table></table>;也可以互换。

#### 相关属性：

+ action：   规定向何处发送提交的表单数据。值：URL

+ method：规定以何种方式将表单数据传送到服务器。值：get/post
  + get :信息在地址栏内展现
  + post:信息在地址栏内不展现

  所有表单控件都必须放在<form></form>标签之间，否则用户输入的信息无法提交到服务器！

  <input />（单表签）（不独占一行）
+ 文本框
eg: 填写用户名：

```
  <form>
     <input type = "text" name = "名称" value = "文本" />
</form>

```
1. type：当type = "text"时，输入框为文本输入框。

2. name：为输入框命名，以备后台程序使用。

3. value：为输入框设置默认值。(一般起到提示作用)**文本框中会出现文本二字。**

+ 密码框：

    type="password"
    <input type = "password" name = "名称" value = "文本" />
    name为和后台打交道使用。

    **密码框会出现2个黑点遮住的文本二字，如果value值什么都没写，就没有黑点遮盖。**

+ 单选框：

   1.type : 当 type = "radio" 时，控件为单选框

   2.value：提交数据到服务器的值。

   3.name：为控件命名。

   4.checked：当添加 checked 时，该选项默认选中。
```  
  <form>
<input type = "radio"  value = "Male"      name = "sex"  checked />男（男是给人看的）
<input type = "radio"  value = "feMale"   name = "sex"  />女
  </form>  （name值要一样，value值要不一样）
```
​         (checked：属于布尔属性，写了就有，没写就没有·。)

+ 复选框：checkbox是复选框。

  1. type : 当 type =“checkbox” 时，控件为复选框。
  2. value：提交数据到服务器的值。
  3. name：为控件命名。
  4. checked：当添加 checked 时，该选项默认选中。
```
<form>
<input type = "checkbox"  value = "good1"  name = "goods" />    I have a bike 
<input type = "checkbox"  value = "good2"  name = "goods" />     I have a car 
</form>
```
+ 当 type 属性值为 file 时，用于文件上传。

```
<form>
     <input type = "file" name = "files" />
</form>
```
​       上面会自动出现选择文件四个字的。

+ 按钮：

   提交按钮：type="submit"提交表单信息到服务器
   重置按钮：type="reset"重置表单信息至初始状态
   普通按钮：type="button"
   不是提交一些数据的，不用写name。

```
 <form>
     <input type="submit" value="提交" name="su" />
     <input type="reset"  value="重置" name="re" />
     <input type="button" value="按钮" name="bu" />
</form> 
```
* **按钮的长宽设置包含内边距内容和边框。**

+ 多行文本域

  标签：<textarea></textarea>
  相关属性：
  rows：规定文本区内可见行数。(默认)
  cols：规定文本区内可见列数。（默认）
  value体现在标签之间。

```
<form>
      <textarea  name = "cat " rows = "3" cols = "30"> 
             The cat was playing in the garden.
      </textarea>
 </form> 
```
+ 下拉列表：

<select></select> 元素定义下拉列表
<option></option> 定义待选择的选项
默认把首个选项显示为被选选项，可通过添加 selected 属性设置默认选项

```
<form>
     <select name = "class">
          <option value = "one"  selected> 软件一班 </option>
          <option value = "two"> 软件二班 </option>
          <option value = "three"> 软件三班 </option>
       </select>
</form> 
```
（此时value给后台看，标签间的内容给用户看。）

+ checked    selected也是布尔属性。

​       disabled表示此输入框不可以使用。布尔属性。

## CSS语言
### 介绍：
+ CSS 是 Cascading Style Sheets 的缩写。译作「层叠样式表」。
+ CSS 是用于(增强)控制网页样式并允许将**样式与网页内容**分离的一种声明式语言。
+ 选择器{ 属性：属性值；属性：属性值 ; ……}一个声明（属性加属性值）之间用分号隔开。

### 选择器
#### 标签选择器 —— 选择器是 HTML 标签
```
<style>
        p {
            color: red;
            font-size: 14px;
        }

        h1 {
            color: green;
            font-size: 50px;
        }       
    </style>
```
#### 类选择器   以“.”开头定义的选择器
影响所有以 class 属性引用该类的标签样式。
   (注意：类名的第一个字符不能使用数字！)
元素可以加入多个类。把各个类名放在 class 属性中，各个类名之间用**一个空格分隔**，类名的**顺序并不重要。**
  有两个名字时，两个效果都会出现，如果矛盾了，就会后面的覆盖前面的。
  eg:.red.font {

     color:purple;
    
     }

#### lD选择器 —— 以“#”开头定义的选择器 ð��\
影响以 id 属性引用该选择符的标签样式。
单一页面中，一个 id 选择器**只能使用一次！**
```
<style>
        #red {
            color: red;
            font-size: 14px;
        }
</style>
<body>
<p id="red">这是第二个段落。</p>
</body>
```
ID属性值只能有一个！！
### CSS语法
将 CSS 样式与 HTML 的内容整合有三种方式：⭐

- 行内样式

- 页内样式

- 外部样式

  

- 行内样式 —— 在元素标签内通过 style 属性添加样式

 `<h1 style="color:red; font-size:28px;">我是标题</h1>`⭐
 用途：指定网页中个别元素的显示效果。不符合样式与内容分离原则，不推荐使用。

+ 页内样式 —— 在 head 内的 style 标签内添加样式

  用途：对页面中某些标签或元素设置样式风格。控制当前页面样式，维护较困难。
   style标签可以有多个。
  type="text/css"在style标签中的属性，可省略。

+ 外部样式 —— 引用外部建立的 .css 文件
  <link rel="stylesheet" type="text/css" href="E:\Users\大一下学期\web开发\1.css" />

  (固定的这个样子，.css文件中直接写a{color:red;}即可)
  用途：可同时控制多个页面，适用于各类大型网站，**可用性最强，推荐使用。复用程度最高**。

####优先级问题
+ 样式优先级：
  ID选择器 > 类选择器 > 标签选择器（前提：作用于同一标签时）
  行内样式 > 页内样式 > 外部样式（前提：先引进外部元素，再写页内元素，就近原则，距离元素最近的样式优先级最高）

+ css的权重
   权重高优先级高。
    重值：（可累加）
   行内样式                                                                1000
   id选择器                                                                100
   类选择器、属性选择器和伪类选择器（hover）10

   (标签选择器)元素和伪元素 （:after; :before;)   1                                 

+ ！important  允许开发人员强制应用某样式。（写在属性值后面分号前面）
#### CSS的两大特点（重要的）
+ CSS 样式的叠加
  多个样式，在同一内容上共同实现，叫做 CSS 样式的叠加。
+ CSS 样式的可继承性
  文档中的某些元素，将沿用为其父元素所设置的样式，这种特点叫做 CSS样式的可继承性。（超链接比较特殊 不能继承父的**颜色标签** 其他的可以继承）只有单独给a标签写color标签
#### CSS注释
+ CSS 注释方法：/*…*/  多行注释
+ html 注释方法：注释标签 <!-- 与 -->       
#### 群组选择器：
```css
p,ul{
    color:blue;
}
ul {
    font:12px;
}
```



###  CSS基本样式修饰 

#### 字体属性

1.字体系列：font-family

+ 设置一种字体

​     font-family : '宋体' ;

+ 设置多种字体

​     font-family : '宋体', '仿宋', 'Times New Roman' ;

​    若用户系统里有宋体，用宋体，无宋体则用仿宋……

2.字体大小：font-size

+ 设置字体大小为绝对值

   font-size : 20px;

   将文本设置为指定的大小，不允许用户在浏览器中改变文本大小。

+ 设置字体大小为相对值

   font-size : 2em;（或 font-size : 200%;）

   相对于父级元素来设置大小。允许用户改变文本大小 

   2em=2*父级元素字大小

   若未规定字体大小，普通文本的默认大小是 16 像素 (16px=1em)。



3.字体样式：font-style

​     normal正常（默认）;italic 斜体；oblique  倾斜；inherit  继承父元素；

4.字体粗细 font-weight      关键字设置字体粗细

  Øfont-weight : bolder;

  Ø属性值：lighter（比默认值细） 、normal （正常值） 、 bold（粗体）、bolder （加粗体）

 数字设置字体粗细

  Øfont-weight：900;

  Ø属性值取值范围为 100~900

  Ø400 等同于 normal，而 700 等同于 bold 

5.字体综合属性 font

​      在一个声明中设置所有属性

•font：italic  bold  36px  '宋体';(中间用空格隔开)

•font：36px  '宋体'；

+ 设置顺序

  •font-style  font-weight   font-size  font-family

  •综合属性必须指定**字体大小**和**字体系列**

  •未设置的属性会使用默认值

#### + 文本相关属性  

1.文本缩进：text-indent

+ Ø设置段落元素的第一行缩进方式

  •text-indent : 2em;

  •text-indent : -3em; （悬挂缩进）

  •属性值可为绝对值（px），也可为相对值（em）

  Ø实战技巧

  •常用于设置段落的首行缩进

  •推荐将缩进设置成相对值，这种方式可以保证不论文字字号为多大，始终能够缩进大小为2个文字的位置。

2.水平对齐：text-align

+ •常用属性值有三种：left（左对齐） 、center（居中对齐）、right（右对齐）

  •text-align:left；

 + 默认左对齐

  

3.文本修饰：text-decoration

+ 属性值：none（无装饰）, overline（上划线）, underline（下划线），line-through（删除线）

  text-decoration : underline
+ a 元素默认有下划线，其他元素默认值为 none
  可用来去掉浏览器给 <a> 加的默认的下划线



4.字符转换：text-transform

+ 设置文本的大小写

  •text-transform：uppercase;

+ 属性值：

  •none： 不改变所写的大小写。

  •uppercase：把所有的字母转换成大写

  •lowercase：把所有的字母转换成小写

  •capitalize：只对每个单词的首字母大写

5.行高：line-height：1.5em；行高是第一行上面到第二行上面，所以数不可以小于1.

+ 设置行与行之间的距离

  属性值表示方式：

  •固定值（如：line-height : 36px; ）

  •相对值（如：line-height : 1.5em;）基于当前字体尺寸

+ 实战技巧

  一般行高是文字的 1.5~1.8 倍最为合适

  行间距不允许使用负值

 6.文本颜色：color

+ •color : green;

  •color : #008000;

  •color : rgb(0,128,0);

+ 缩写

  + \#ff0000   =  #f00

    \#00ff00   =  #0f0

    \#eeeeee  =  #eee

    缩写时有一个无法缩写你也不可以缩写。

#### 超链接的样式设置

+ 超链接的四种状态
  + 未被访问的超链接 a:link
  + 鼠标经过的超链接 a:hover
  + 链接被点击的那一刻 a:active
  + 访问过的超链接 a:visited

   l可对超链接的四种不同状态设置不 同样式 。

+ Ø设置超链接的多种状态（≥2）时，需要按特定顺序设置

     :link，:visited，:hover，:active

      llink 和 visited 只用于超链接 :

##### 伪类

+ focus 示例：设置input元素获得焦点时的样式

  ```css
  input:focus
  {
      background-color:yellow;
  }
  ```

  

  first-child 示例：设置列表第一个元素的样式

  `ul li:first-child{ background:green;}`

+ link 和 visited 只用于超链接

  其他可用于各种 HTML 元素

  示例：设置 div 鼠标效果

  hover 设置鼠标滑过效果

  active 设置鼠标点击效果

#### 背景的样式设置

+ 背景相关属性  

  + 背景色   ：background-color

    + 所有元素可设置背景色
    + 背景默认颜色是透明色
    + background-color : gray;
    + background-color : #808080；
    + background-color : rgb(128,128,128);
  + 背景图片：background-image

    + 例如：p { background-image : url(image/1.png);} 
  + 背景重复：background-repeat
    + repeat  默认。背景图像会在垂直方向和水平方向重复。
    + repeat-x 在水平方向重复
    + repeat-y 在垂直方向重复
    + no-repeat 背景图像只显示一次
    + inherit 从父元素继承background-repead属性的设置。
    + 可继承属性
  + 背景定位：background-position：70%；
     + 前提是l图像平铺模式设置为 no-repeat 。
     +  属性值: center或百分比
     + background-position 的默认值是 0% 0%，在功能上相当于 top left 
     + lbackground-position : 长度值； 长度值是指距离元素左上角的距离 
  + background(综合设置)
    在一个声明中设置所有背景属性  无顺序要求

+ span无语意标签

#### 列表常用样式
+ 列表标志类型：

  list-style-type  属性值：PPT45页（可以继承的属性）

  none：无标记。disc：默认。标记是实心圆。circle：标记是空心圆。square：标记是实心方块。decimal：标记是数字。

+ 列表标志图像：list-style-image

  + 使用图像来替换列表项的标记

     list-style-image : url（ images/arrow.png );

     列表标志位置：list-style-position

+ 设置列表标记的位置

  + list-style-position : inside;

  + 属性值：

    •outside：默认值。标记位于文本的左侧

    •inside：标记放置在文本以内

+ 列表综合属性

  ​	一个声明中设置所有的列表属性。

  list-style : url(images/arrow.png)  outside  circle;
  list-style : url(images/arrow.png)  inside  circle;

  |  字体修饰   |    文本修饰     | 超链接修饰 |      背景修饰       |      列表修饰       |
  | :---------: | :-------------: | :--------: | :-----------------: | :-----------------: |
  | font-family |   text-indent   |   a:link   |  background-color   |   list-style-type   |
  |  font-size  |   text-align    | a:visited  |  background-image   |  list-style-image   |
  | font-weight |      color      |  a:hover   |  background-repeat  | list-style-position |
  | font-style  |   line-height   |  a:active  | background-position |     list-style      |
  |    font     | text-decoration |            |     background      |                     |

  


## 第六章 盒子模型

* Web 中的盒子：一个矩形区域，内容包裹在盒子中。盒子的堆叠与嵌套形成整个页面的内容排布。

* 盒子的作用：

   * 页面内容的容器 。
   *  通过盒子与盒子的嵌套、堆叠，控制页面内容的展示位置（布局） 

* 属性：**内容 边框 内边距 外边距。**

* 每个盒子具有的特征：

   大小（width、height）

   边框（border）

   内边距（padding）

   外边距（margin）

* 大小
  内容区域的大小，像素。

* 边框
  边框的宽度：border-width : 5px;
  边框的样式：border-style : solid;
  边框的颜色：border-color : red;

* 内边距：padding

* 外边距：margin

* 也可以上下左右边框依次设置。

   * border-top-color : #cccccc; 

   * border-right-color : #cccccc;

   * border-bottom-color : #cccccc;

   * border-left-color : #cccccc；

   * border-width：20px 10px 30px 0px;⭐
* outline:不属于盒模型，不占据浏览器的位置，可用他代替border属性。outline:3px solid red;
  
#### 块级元素与行内元素

*  块级元素（block  level element）

  •元素在显示时会**独占一行**，并同时具有宽、高、内外边距特征。

  •举例：<p>

* 行内元素（inline element）

  •在显示时通常**不会以新行开始**，横向排列，到最右端自动折行。

  •举例：<a>

  •盒子模型的四个特征不全具备。**不具备上下外边距。**

* 行块级 ** input   img**  含有盒子模型的四个特征。**不独占一行**

* display属性

  - 用于指定 HTML 标签的显示方式 

  - 属性值：关键字

    •常用的有 4 个

  - - block     将元素显示为块级元素，该元素前后会带有换行符 
    - inline     元素会被显示为行内元素，该元素前后没有换行符 
    - inline-block     行内块元素 
    - none     该元素不会被显示 

+ 重置样式(清零)

  + *{

  ​      padding：0px；

  ​      margin：0px；

    }
  + a{
     text-decoration:none;
     }
  + ul{
     list-style-type:none;
      }
  + .clearfix:after{
           content:'';
           display:block;
           height:0;
           clear:both;
         }
+ 透明度设置（可继承属性）
    + img { 
      opacity:0.4;  
       } 默认值是1，范围0~1
    + opacity:opaticy设置的透明度会把其所有内容和元素都设置为透明的，rgba设置的透明度只会把设置为该属性所对应的操作设置为透明的。
+ div标签（块级） span标签（行级） 布局用
+ 居中问题

  1. 水平居中（text-align:center padding-right padding-left margin:0 auto;） 
  2. 垂直居中(padding-top padding-bottom line-height)



##  第七章 网页布局     

+ 布局标签 —— div
  + 相当于一个容器（盒子）
  + 具有盒子模型的所有属性，布局时用来控制元素之间的距离和相对位置
  + 可以把文档分割为独立的、不同的部分
  + 通过 id 或 class 属性区分不同的容器

### 布局方法

+ float 浮动

  + float: none | left  | right 

  + 一个元素被设置float  则变成行块级

  + lfloat的初衷 —— 文字环绕图片效果

    给图片设置浮动，文字会往上跑。

+ 浮动（float）注意事项
   + 浮动元素距离父元素边框的位置，是该侧的父元素 padding +自身 margin 的值
   + 通常不会超过父元素的边界
   + 元素一旦浮动就不属于父元素了
   + 浮动元素不会相互重叠
   + 不能上下浮动，通常只设左/右一种浮动即可
   + 如果父元素宽度不够，浮动元素会另起一行显示

+ 父元素高度塌陷解决办法
   + 1.给父元素设置高度
   + 2.清除浮动 —— clear   用来设置该元素边上没有其他元素可以浮动
       + clear: left / right / both / none 
           left：不允许左边有浮动的元素
           right：不允许右边有浮动的元素
           both：不允许左右两边有浮动的元素
           none：默认值，可以浮动
   + 3.清除浮动 —— 伪元素（标签） :after  :before，并搭配属性 clear:both;（用的最多）
    + 4.溢出处理 —— overflow ：；PPT28页
        + 4.清除浮动 —— overflow: hidden;  "
           + 父元素不设高度并且子元素浮动时，使父元素高度**自动适应**子元素高度
           + 修剪非浮动元素的溢出部分，而父元素会适应浮动元素。写在父元素之中。

+ position 定位

  + static 默认值，没有定位。元素出现在正常的流中 。

  + 相对定位 relative

      与 left，right，top，bottom 等属性共同使用；

      以自身本应在的位置为参照物；

      保留自身位置；下面的元素不会到上面。

     + 绝对定位 —— position : absolute;

         + 与 left，right，top，bottom 等属性共同使用
         + 若祖先元素已定位，则以该祖先元素为参照物
         + 若祖先元素未定位，则以 body 元素为参照物
         + 不保留自身位置。
         + 绝对定位对称设置 

  + 固定定位——  position : fixed; 

       + 与 left，right，top，bottom 等属性共同使用

       +  以浏览器窗口为参照物进行定位

   + lfloat 和 position 不同点 

         + position 与 top、left 等配套使用
         + float 位置移动通过 margin、padding 等实现
         + overflow 和 clear 对 position 无效
         + 布局通常使用 float，而不是 position

   + 堆叠顺序  ——  z-index（只有定位的元素才有的效果）

        + 用于体现元素在 Z 轴空间的堆叠关系
        + 仅能在定位元素上奏效
        + 大部分情况以数字为取值
        + 可为多个元素设置
        + 定位的在未定位的上面，都定位了默认写在后面的在上面。定位元素默认z-index=1而非定位元素默认为0

  + 基线问题：vertical-align:bottom;       

注意：按钮的宽和高是包含了内容，padding，边框的。⭐

​           一个元素如果进行了浮动或者绝对定位，那么他就没有了自己的大小了，是由里面的内容撑起来的。

​           超链接的字体颜色无法继承。

​           小tip:当text-align:center;不起作用时，可以把参照的元素设置为行快级元素即可。⭐

​            在普通文档流中，垂直的盒子会出现外边距合并，但是浮动的和定位的时候不会合并。

​          CSS选择器的解析顺序是从右到左的，所以不可以出现选择层级过长。

​           定位时向右和向下是正值。⭐

​         鼠标变小手：cursor:pointer;

​           二级菜单隐藏时用  diaplay:none;

​         绝对定位和浮动一样会脱离文档流，像飘起了一样，二级菜单里需要二级菜单相对于一级菜单进行绝对定位。否则下面的内容会掩盖二级菜单。⭐

​           二级菜单里的对称线设置，用到before，after的伪类元素。重要（⭐）