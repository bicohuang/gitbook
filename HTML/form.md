##form表单笔记

##1、form标签的使用
1. `name`属性 &nbsp;用来区分多个表单
2. `action`属性&nbsp;用来指明处理表单数据的人是谁
3. `method` 属性&nbsp;表示数据的传输方式
	-  `post` &nbsp;数据量较大 安全性高
	- `get` &nbsp;数据量较少 安全性低

<form  name="reg" action="reg.php" method="post">
			姓名：
			<input type="text" name="username" id="" value="" /><br />
			
			<input type="submit" value="确定"/>
</form>
    
```html
<form  name="reg" action="reg.php" method="post">
			<input type="text" name="username" id="" value="" /><br />
			
			<input type="submit" value="确定"/>
</form>

```
> **备注**:form表单是用户用来提交数据的方式之一

    
[参考链接](http://baidu.com)
![百度](https://www.baidu.com/img/bd_logo1.png)



##2、input标签的使用
表单家族里面最大的单个元素了，因为他有多个类型 所以功能也是最多的
1. `type`属性&nbsp; 表示输入框的具体类型
	- `text`  文字输入框 &nbsp;用于输入文字 
	- `password`   &nbsp;密码输入 输入的文字会以`*`表示
	- `ridio`    单选框 &nbsp; `name`属性要一致的，以表示同一组选项
	- `checkbox`  复选框 ,&nbsp; `name`属性最好一致的，还要加上`[]`，以表示同一组选项 `checked` 表示默认选中
	- `search` 搜索框 &nbsp;用于搜索
	- `bottom` 普通按钮&nbsp;需要脚本语言配合
	- `submit` 提交按钮&nbsp;用来确定数据的提交
	- `reset`  重置按钮&nbsp;用来清除表单的输入数据
	- `image` 图片按钮&nbsp;点击图片时触发按钮功能
	- `hidden` &nbsp;隐藏某些特殊的数据
	- `file` &nbsp;文件上传，但是必须要`form`表单的`enctype`属性设置为`multpart/form-data`,`method`属性必须设置为`post`,如果需要多文件上传，可以增加一个`multiple`属性
2. `name`属性 &nbsp;用来区分的多个input元素，并且该属性是必须的。
3. `value`属性 &nbsp;用来装载具体的值，可以是用户输入的，也可以是预先设置好的
4. `maxlengh`&nbsp;表示输入数据的最大字数，不分中英文
5. `readonly` &nbsp;是一个单属性，通常只需要把属性名字写上即可，表示该属性只读，不允许修改，不影响数据的提交 
6. `disebled` &nbsp;也是一个单属性，表示禁用，不允许修改和提交
7. `placeholder`&nbsp; 用来显示提示
    
```html
<input type="text" name="username"value="bgg"
	maxlength="15" placeholder="请输入用户名" readonly disabled/>
<input type="password" name="pw"/><br />

<input type="radio" name="sex" id="man" value="1" />
	<label for="man">男</label> 
<input type="radio" name="sex" id="reman" value="2" />
 	<label for="reman">女</label>

<input type="checkbox" name="fav[]" id="fav[]"  checked value="1" />LOL
<input type="checkbox" name="fav[]" id="fav[]" value="2" />PHP
<input type="checkbox" name="fav[]" id="fav[]" value="3" />kkkkk

<input type="submit" value="确定"/>
<input type="reset" value="重置"/>
<input type="button" value="普通按钮" onclick="alert('bgg')"/>
<input type="image"  value="" src="img/HBuilder.png"/>
<br />
<button> 我也是一个普通的按钮</button>
<input type="hidden" name="ip_adress" id="ip_adress" value="192.168.100.101" />
<input type="file" name="file" id="file"/>
```
> 备注：其中，只有`type`为submit和image的按钮默认具有提交表单的功能
    
##3、textarea标签
1. 文本域 用于接收较多文字的输入

```html

```
> 备注:要注意文本域的值是写在标签对之间，并且把所有的空格和换行记录并显示出来,如果想要禁止改变文本域的大小需要css属性的**resize: none;**

     
##3、select下拉菜单
```html
<select name="city">
<option value="0"selected>   </option>
<option value="1">北京</option>
<option value="2">上海</option>
<option value="3">深圳</option>
<option value="4">广州</option>
<option value="4">🤖</option>
</select>
```
> 备注1：单选模式的话，跟单选框类似，只能选其一，如果需要设置默认选中，则给相应的选项设置`selected`属性
> 备注2：多选模式，需要给select标签增加nultiple属性，并且`name`属性最好带**[  ]中括号**
    
#[caniuse.com](http://www.caniuse.com) 查询兼容性