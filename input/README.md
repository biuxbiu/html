## input

```javascript
<input>             //没有结束标签
```

#### input的属性和类型

|属性|值|描述|
|::-|::-|::-|
|[accept](input/#accept)|audio/* video/* image/* MIME_type|规定提交的文件类型（针对 type="file" 存在）|
|[alt](input/#alt)|text|定义图像的替代文本|
|[autocomplete](input/#autocomplete)|on/off|启动或者关闭是否采用自动完成功能|
|[autofocus](input/#autofocus)|autofocus|表示页面在加载时该元素自动获得焦点|
|[checked](input/#checked)|checked|表示页面在加载时预先选定该元素|
|[disabled](input/#disabled)|disabled|表示该元素被禁用|
|[form](input/#form)|form_id|包含多个表单|
|[formaction](input/#formaction)|url|表示表单在提交的时候，输入控件的URL地址（针对 type="submit" / type="image" 存在）|
|[formenctype](input/#formenctype)|application/x-www-form-urlencoded multipart/form-data text/plain|表示提交表格时的编码格式|
|[formmethod](input/#formmethod)|get/post|提交的方法（针对 type="submit" / type="image" 存在）|
|[formnovalidate](input/#formnovalidate)|formnovalidate|覆盖表单的 novalidate 属性。如果使用该属性，则提交表单时不进行验证。|
|[formtarget](input/#formtarget)|_blank<br>_self<br>_parent<br>_top<br>framename|覆盖表单的 target 属性。（适用于 type="submit" 和 type="image"）|
|[height](input/#height)|px<br>%|设置 `<input>` 的高度|
|[list](input/#list)|datalist-id|表示输入字段的预选项|
|[max](input/#max)|number<br>date|与 `min` 相结合使用，设置合法值范围，适用于以下 `<input>` 类型：number, range, date, datetime, datetime-local, month, time 以及 week|
|[min](input/#min)|number<br>date|与 `max` 相结合使用，设置合法值范围，适用于以下 `<input>` 类型：number, range, date, datetime, datetime-local, month, time 以及 week|
|[max-length](input/#max-length)|number|允许字符的最大长度|
|[multiple](input/#multiple)|multiple|允许一次性选择多个，一般与 `type="file"` 结合使用|
|[name](input/#name)|field_name|表示 `<input>` 的名称|
|[pattern](input/#pattern)|regexp_pattern|设定输入字段的格式 pattern="[0-9]" 表示必须是 0 到 9 之间的数字|
|[placeholder](input/#placeholder)|text|用户填写提示|
|[readonly](input/#readonly)|readonly|设置为只读|
|[required](input/#required)|required|定义这个输入框在提交表格的时候必填项，如果有该属性，则该字段是必填或者必选|
|[size](input/#size)|number_of_char|定义的是**以像素为单位**的输入字段宽度（定义输入框的宽度）|
|[src](input/#src)|url|定义以提交按钮显示出来的图片的URL|
|[step](input/#step)|number|规定输入字的的合法数字间隔（以这个间隔变化）|
|type|[button](input/#button)<br>[checkbox](input/#checkbox)<br>[color](input/#color)<br>[readonly](date/#date)<br>[datetime](input/#datetime)<br>[datetime-local](input/#datetime-local)<br>[email](input/#email)<br>[file](input/#file)<br>[hidden](input/#hidden)<br>[image](input/#image)<br>[month](input/#month)<br>[number](input/#number)<br>[password](input/#password)<br>[radio](input/#radio)<br>[range](input/#range)<br>[tel](input/#tel)<br>[time](input/#time)<br>[url](input/#url)<br>[week](input/#week)<br>[reset](input/#reset)<br>[submit](input/#submit)<br>[text](input/#text)|定义可点击的按钮<br>定义复选框<br>定义拾色器<br>定义 date 控件（包括年、月、日，不包括时间）<br>定义 date 和 time 控件（包括年、月、日、时、分、秒、几分之一秒，基于 UTC 时区）<br>定义 date 和 time 控件（包括年、月、日、时、分、秒、几分之一秒，不带时区）。<br>定义用于 e-mail 地址的字段。<br>定义文件选择字段和 "浏览..." 按钮，供文件上传。<br>定义隐藏输入字段。<br>定义图像作为提交按钮。<br>定义 month 和 year 控件（不带时区）<br>定义用于输入数字的字段<br>定义密码字段（字段中的字符会被遮蔽）<br>定义单选按钮<br>定义用于精确值不重要的输入数字的控件（比如 slider 控件）<br>定义重置按钮（重置所有的表单值为默认值）<br>定义用于输入搜索字符串的文本字段。<br>定义提交按钮。<br>定义用于输入电话号码的字段。<Br>默认。定义一个单行的文本字段（默认宽度为 20 个字符）。<Br>定义用于输入时间的控件（不带时区）。<Br>定义用于输入 URL 的字段。<Br>New	定义 week 和 year 控件（不带时区）。<br>|
|[value](input/#value)|value|规定 `<input>` 元素的值|
|[width](input/#width)|pixel<br>%|定义 input 字段的宽度。（适用于 type="image"）|

<br>

###### accept

```html
<form>
    Choose File: <input type="file" accept="png">
</form>
```

<form>
    Choose File: <input type="file" accept="png">
</form>

<br>
<br>

###### alt

```html
<form>
    <input type="image" alt="bottom" src="../img/chenqinchao.png">
</form>
```

<form>
    <input type="image" alt="bottom" src="../img/chenqinchao.png">
</form>

<br>
<br>

###### autocomplete

```html
<form>
    Your Email: <input type="email" name="email"  autocomplete="on">
</form>
```

<form>
    Your Email: <input type="email" name="email" autocomplete="on">
</form>


<br>
<br>

###### autofocus

```html
<form>
    First name: <input type="text" name="fname" autofocus>
</form>
```

<form>
    First name: <input type="text" name="fname" autofocus>
</form>

<br>
<br>

###### autofocus

```html
<form>
    Boy: <input type="radio"  name="sex">
    Girl: <input type="radio" name="sex" checked>
</form>
```

<form>
    Boy: <input type="radio"  name="sex"><Br>
    Girl: <input type="radio" name="sex" checked>
</form>


<br>
<br>

###### autofocus

```html
<form>
    Boy: <input type="radio"  name="sex">
    Girl: <input type="radio" name="sex" checked>
</form>
```

<form>
    Boy: <input type="radio"  name="sex"><Br>
    Girl: <input type="radio" name="sex" checked>
</form>


<br>
<br>

###### 改变输入框的光标颜色


* 通过 caret-color 属性：

```copy
input{
    caret-color:yellow
}
```

<br>
<br>

* 通过 `:first-line` 伪元素：

```copy
input{
    color:black;
    &:first-line{
        color:yellow;
    }
}
```

