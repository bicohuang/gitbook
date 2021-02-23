# table 表格笔记

## 1、table 标签

  1. `name` 属性 &nbsp;定义名称
  2. `border`属性 &nbsp; 表示`table`边框的粗细， 默认是1
  3. `cellpadding`属性&nbsp;表示格子和格子之间的距离
  4. `cellspacing`属性&nbsp;表示格子与内容的距离
  5. `align`属性 &nbsp;定义内容的对齐方式

  	- `left` &nbsp;左对齐
  	- `center` &nbsp;中心对齐
  	- `right` &nbsp;右对齐
  6. `valign`属性&nbsp;垂直排列方式
	- `top` &nbsp;顶部对齐
	- `middle` &nbsp;中间对齐
	- `bottom` &nbsp;底部对齐

## 2、th标签
### 定义表格的标题

  1. `align`属性 &nbsp;定义内容的对齐方式

  	- `left` &nbsp;左对齐
  	- `center` &nbsp;中心对齐
  	- `right` &nbsp;右对齐
  2. `valign`属性&nbsp;垂直排列方式
	- `top` &nbsp;顶部对齐
	- `middle` &nbsp;中间对齐
	- `bottom` &nbsp;底部对齐
##3、tr标签 
###定义表格的行
  1. `align`属性 &nbsp;定义内容的对齐方式

  	- `left` &nbsp;左对齐
  	- `center` &nbsp;中心对齐
  	- `right` &nbsp;右对齐
  2. `valign`属性&nbsp;垂直排列方式
	- `top` &nbsp;顶部对齐
	- `middle` &nbsp;中间对齐
	- `bottom` &nbsp;底部对齐
##4、td标签
###定义单元格
  1. `align`属性 &nbsp;定义内容的对齐方式

  	- `left` &nbsp;左对齐
  	- `center` &nbsp;中心对齐
  	- `right` &nbsp;右对齐
  2. `valign`属性&nbsp;垂直排列方式
	- `top` &nbsp;顶部对齐
	- `middle` &nbsp;中间对齐
	- `bottom` &nbsp;底部对齐
  3. `colspan`属性&nbsp合并列单元格
  4. `rowspan`属性&nbsp合并行单元格
  
     
```html
		<table border="1" cellpadding="10" cellspacing="1"
			width="100" height="100">
			<tr>
				<td>列</td>
				<td>列</td>
				<td>列</td>
			</tr>
			<tr>
				<td>列</td>
				<td>列</td>
				<td>列</td>
			</tr>
			<tr>
				<td>列</td>
				<td>列</td>
				<td>列</td>
			</tr>
		</table>
```

## 4、a标签
### 定义页面跳转

 1. `href`属性&nbsp;表示要跳转过去的地方
 2. `title`属性&nbsp;表示链接栏的提示信息
 3. `target`属性&nbsp;定义打开新页面的方式
  - _blank &nbsp;新的空白页
  - _self &nbsp;当前页
  - _top &nbsp;顶上
    
### 锚点 
##### 表示跳转的地方在同一页面内,`href`属性写的是该地方的`id`
## 5、img标签
### 展示图片

1. `src` &nbsp;表示图片的出处
 - 相对地址&nbsp;在项目文件里，相对HTML的位置
<ol type="I">
	<li>./&nbsp;表示当前目录 </li>
	<li>../&nbsp;返回上层目录</li>
	<li>image/&nbsp;进入一层目录</li>
	<li>../image/&nbsp;先返回上层，再进入image目录</li>
</ol>
 - 绝对地址&nbsp;不在项目文件里，例如引用网上的图片
2. `alt` &nbsp;定义图片的替代文本
3. `width`&nbsp;设置图片的宽度
4. `height`&nbsp;设置图片的高度
   
### 热区

1. `Map`&nbsp;表示热区集合
 1. `area`&nbsp;表示单个热区
     - `shape` &nbsp;热区形状
     - `coords` &nbsp;形状的坐标值
     
```html
<img src="https://www.baidu.com/img/bd_logo1.png" usemap="map"/>
<map name="map">
<area shape="rect" coords="0,0,400,400" href="fisrt.html" alt="加载失败" />
</map>
```

## 6.H1~H6标题标签
### H1~H6不同的字体大小，加粗

<h1>标题1</h1>		
<h2>标题2</h2>
<h3>标题3</h3>
<h4>标题4</h4>
<h5>标题5</h5>
<h6>标题6</h6>
## 7、文本格式化

1. `<P>`&nbsp;定义段落
2. `<span>` &nbsp;定义一个片段
3. `<b>`&nbsp;定义粗体文本
4. `<i>` &nbsp;定义斜体文本 
5. `<del>`&nbsp;定义删除文本
6. `<sup>`&nbsp;定义上标字
7. `<sub>`&nbsp;定义下标字
   

<b>定义粗体文本</b>
    
<i> 定义斜体文本 </i>  
    
<del>定义删除文本</del>
     
x<sup>2</sup>
    
x<sub>2</sub>
    
```html
<b>定义粗体文本</b>
<i> 定义斜体文本 </i>  
<del>定义删除文本</del>
x<sup>2</sup>
x<sub>2</sub>
```

   

