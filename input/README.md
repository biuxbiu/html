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
|[checked](input/#checked)|checked|表示页面在加载时预先选定该元素（只针对 type="radio" 和 type="checkbox"）|
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
|[min](input/#max)|number<br>date|与 `max` 相结合使用，设置合法值范围，适用于以下 `<input>` 类型：number, range, date, datetime, datetime-local, month, time 以及 week|
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
|type|[button](input/#button)<br>[checkbox](input/#checkbox)<br>[color](input/#color)<br>[readonly](date/#date)<br>[datetime](input/#datetime)<br>[datetime-local](input/#datetime-local)<br>[email](input/#email)<br>[file](input/#file)<br>[hidden](input/#hidden)<br>[image](input/#image)<br>[month](input/#month)<br>[number](input/#number)<br>[password](input/#password)<br>[radio](input/#radio)<br>[range](input/#range)<br>[tel](input/#tel)<br>[time](input/#time)<br>[url](input/#url)<br>[week](input/#week)<br>[reset](input/#reset)<br>[submit](input/#submit)<br>[text](input/#text)|定义可点击的按钮<br>定义复选框<br>定义拾色器<br>定义 date 控件（包括年、月、日，不包括时间）<br>定义 date 和 time 控件<br>定义 date 和 time 控件<br>定义用于 e-mail 地址的字段<br>定义文件选择字段和 "浏览..." 按钮，供文件上传<br>定义隐藏输入字段<br>定义图像作为提交按钮。<br>定义 month 和 year 控件<br>定义用于输入数字的字段<br>定义密码字段（字段中的字符会被遮蔽）<br>定义单选按钮<br>定义用于精确值不重要的输入数字的控件（比如 slider 控件）<br>定义重置按钮（重置所有的表单值为默认值）<br>定义用于输入搜索字符串的文本字段。<br>定义提交按钮。<br>定义用于输入电话号码的字段。<Br>默认。定义一个单行的文本字段（默认宽度为 20 个字符）。<Br>定义用于输入时间的控件（不带时区）。<Br>定义用于输入 URL 的字段。<Br>New	定义 week 和 year 控件（不带时区）。<br>|
|[value](input/#value)|value|规定 `<input>` 元素的值|
|[width](input/#width)|pixel<br>%|定义 input 字段的宽度。（适用于 type="image"）|

<br>

###### accept

```html
<form>Choose File: <input type="file" name="file" accept="png" /></form>
```

<form>
    Choose File: <input type="file" name="file" accept="png">
</form>

<br>
<br>

###### alt

```html
<form>
  <input type="image" alt="bottom"  name="image"  src="../img/chenqinchao.png" />
</form>
```

<form>
    <input type="image" alt="bottom" name="image"  src="../img/chenqinchao.png">
</form>

<br>
<br>

###### autocomplete

```html
<form>Your Email: <input type="email" name="email" autocomplete="on" /></form>
```

<form>
    Your Email: <input type="email" name="email" autocomplete="on">
</form>

<br>
<br>

###### autofocus

```html
<form>First name: <input type="text" name="fname" autofocus /></form>
```

<form>
    First name: <input type="text" name="fname" autofocus>
</form>

<br>
<br>

###### radio

```html
<form>
  Boy: <input type="radio" name="sex" />
  Girl:<input type="radio" name="sex" checked />
</form>
```

<form>
    Boy: <input type="radio"  name="sex"><Br>
    Girl: <input type="radio" name="sex" checked>
</form>

<br>
<br>

###### checked

```html
<form>
  Boy: <input type="radio" name="sex" checked /> 
  Boy: <input type="checkbox" name="sex" checked />
</form>
```

<form>
    Boy: <input type="radio"  name="sex" checked><br>
    Boy: <input type="checkbox"  name="sex" checked>
</form>

<br>
<br>

###### disabled

!>表单中被禁用的 `<input>` 元素不会被提交<br>
disabled 属性不适用于 `<input type="hidden">`

```html
<form>
  Boy: <input type="radio" name="sex" disabled /> Boy:
  <input type="checkbox" name="sex" disabled /> Boy:
  <input type="text" name="sex" disabled />
</form>
```

<form>
    Boy: <input type="radio"  name="sex" disabled><br>
    Boy: <input type="checkbox"  name="sex" disabled><br>
    Boy: <input type="text"  name="sex" disabled>
</form>

<br>
<br>

###### form

```html
<form>
  BoyName: <input type="text" name="text" />
  <input type="submit" value="ok" />
</form>
```

<form>
    BoyName: <input type="text" name="text" ><br>
    <input type="submit" value="ok">
</form>

<br>
<br>

###### formaction

!>提交的时候要跳转的 `URL` 地址

```html
<form>
  BoyName: <input type="text" name="text"  />
  <input type="submit" value="单纯的提交" />
  <input type="submit" formaction="submit.html" value="ok" />
</form>
```

<form>
    BoyName: <input type="text" name="text" ><br>
    <input type="submit" value="单纯的提交"><br>
    <input type="submit" formaction="submit.html" value="跳转到某个页面进行提交">
</form>

<br>
<br>

###### action

**将数据提交给哪个页面进行处理**

```html
<form action="login.html">
  BoyName: <input type="text" name="text" />
  <input type="submit" value="单纯的提交" />
</form>
```

<form action="login.html">
    BoyName: <input type="text" name="text"  >
    <input type="submit" value="单纯的提交">
</form>

<Br>
<Br>

**`action` 与 `formaction` 的区别？**

!>`action` 作用在 `<form>` 上，`formaction` 作用在 `<input>` 上;<Br>
`<input>` 的 `formaction` 属性会覆盖 `<form>` 的 `action属性`，有 `formaction` 就没有 `action` 的什么事。

```html
<form action="login.html">
  BoyName: <input type="text" />
  <input type="submit" formaction="register.html" value="单纯的提交" />
</form>
```

<form action="login.html">
    BoyName: <input type="text" >
    <input type="submit" formaction="register.html" value="单纯的提交">
</form>

<br>
<br>

###### formenctype

**以什么样的编码格式提交**

```html
<form>
  BoyName: <input type="text" />
  <input type="submit" value="单纯的提交" />
  <input
    type="submit"
    formenctype="multipart/form-data"
    value="以 multipart/form-data 的格式提交"
  />
</form>
```

<form>
    BoyName: <input type="text" >
    <input type="submit" value="单纯的提交">
    <input type="submit" formenctype="multipart/form-data" value="以 multipart/form-data 的格式提交">
</form>

<br>
<br>

###### formmethod

**以什么样的方法操作这个表格**

```html
<form>
  BoyName: <input type="text" />
  <input
    type="submit"
    formmethod="post"
    formaction="login.html"
    value="post的方法提交"
  />
  <input
    type="submit"
    formmethod="get"
    formaction="login.html"
    value="get的方法提交"
  />
</form>
```

<form action="login.html">
    BoyName: <input type="text" >
    <input type="submit" formmethod="post" formaction="login.html" value="post的方法提交">
    <input type="submit" formmethod="get" formaction="login.html" value="get的方法提交">
</form>

<br>
<br>

###### formnovalidate

**设置表格提交时不用进行验证**

```html
<form>
  BoyName: <input type="text" />
  <input formnovalidate type="submit" value="单纯的提交" />
</form>
```

<form >
    BoyName: <input type="text" >
    <input formnovalidate type="submit" value="单纯的提交">
</form>

<Br>
<Br>

###### formtarget

**提交的时候打开窗口的方式**

```html
<form>
  BoyName: <input type="text" name="text"  />
  <input formtarget="_blank" type="submit" value="新窗口提交" />
  <input formtarget="_self" type="submit" value="原窗口提交" />
  <input formtarget="_parent" type="submit" value="父框架中提交" />
  <input formtarget="_top" type="submit" value="在整个窗口中响应" />
  <input formtarget="framename" type="submit" value="在制定的iframe中响应" />
</form>
```

<form >
    BoyName: <input type="text" name="text"   >
  <input formtarget="_blank" type="submit" value="新窗口提交" />
  <input formtarget="_self" type="submit" value="原窗口提交" />
  <input formtarget="_parent" type="submit" value="父框架中提交" />
  <input formtarget="_top" type="submit" value="在整个窗口中响应" />
  <input formtarget="framename" type="submit" value="在制定的iframe中响应" />
</form>

<Br>
<Br>

###### height

**这个属性只使用在 `type="image" `**

```html
<form>
  BoyName: <input type="text" name="text"  />
 <input type="image"  height="30" src="../img/chenqinchao.png" style="vertical-align:top"/>
</form>
```

<form >
  BoyName: <input type="text" name="text"  height="50" />
  <input type="image"  height="30" src="../img/chenqinchao.png" style="vertical-align:top"/>
</form>

<Br>
<Br>

###### list

**巧变下拉框**

```html
<form>
  letter: <input list="letter"/>
  <dadalist id="letter">
    <option value="A">
    <option value="B">
    <option value="c">
    <option value="d">
  </dadalist>
</form>
```

<form >
  letter: <input list="letter">
  <datalist id="letter">
    <option value="A">
    <option value="B">
    <option value="c">
    <option value="d">
  </datalist>
</form>

<Br>
<Br>


###### max

**设置最小起始时间和最大结束之间**

```html
<form action="demo_form.html">
  结束时间最晚不能晚于 1980-01-01:
  <input type="date" name="bday" max="1979-12-31">

  起始时间最小不能小于 2020-01-02:
  <input type="date" name="bday" min="2020-01-02">

  限定数字在 1 - 5 之间:
  <input type="number" name="quantity" min="1" max="5">

  <input type="submit">
</form>
```

<form action="demo_form.html">
  结束时间最晚不能晚于 1980-01-01:
  <input type="date" name="bday" max="1979-12-31">

  起始时间最小不能小于 2020-01-02:
  <input type="date" name="bday" min="2020-01-02">

  限定数字在 1 - 5 之间:
  <input type="number" name="quantity" min="1" max="5">

  <input type="submit">
</form>

<Br>
<Br>

###### multiple

```html
<form>
  请选择多个文件: <input type="file" name="file" multiple/>
</form>
```

<form >
  请选择多个文件: <input type="file" name="file" multiple/>
</form>

<Br>
<Br>


###### name

**需要把 `name` 属性写上，`form` 表格在提交的时候才能成功提交该值。`name` 属性在 `radio` 还充当重要的唯一角色**

```html
<form>
  请选择多个文件: <input type="file" name="file" multiple/>
  请选择你的性别：男：<input type="radio" name="sex">  女：<input type="radio" name="sex">
</form>
```

<form >
  请选择多个文件: <input type="file" name="file" multiple/><br>
  请选择你的性别：男：<input type="radio" name="sex">  女：<input type="radio" name="sex">
</form>


<Br>
<Br>


###### pattern 

验证正则表达式

```html
<form>
  请输入5个数字: <input type="text" name="textNumber" pattern="[0-9]{5}"/>
  <input type="submit">
</form>
```

<form >
  请输入5个数字: <input type="text" name="textNumber" pattern="[0-9]{5}"/>
  <input type="submit">
</form>

<Br>
<Br>


###### placeholder 

```html
<form>
  请输入你想找的内容: <input type="text" name="textNumber" placeholder="请输入你想找的内容" />
  <input type="submit">
</form>
```

<form >
  请输入你想找的内容: <input type="text" name="textNumber" placeholder="请输入你想找的内容"/>
  <input type="submit">
</form>

<br>
<br>

###### readonly 

* 只读的内容是不能更改的，但是可以拷贝
* 用户还是可以通过 `tab` 键进行选择

```html
<form>
  请输入你想找的内容: <input type="text" name="textNumber" value="这个是只读内容，不能更改"  readonly/>
  <input type="submit">
</form>
```

<form >
  请输入你想找的内容: <input type="text" name="textNumber" value="这个是只读内容，不能更改" readonly/>
  <input type="submit">
</form>

<Br>
<Br>


###### required  

**必填项**

```html
<form>
  请输入你想找的内容: <input type="text" required name="text" placeholder="这个内容你必须填写才能提交" />
  <input type="submit">
</form>
```

<form >
  请输入你想找的内容: <input type="text" required name="text" placeholder="这个内容你必须填写才能提交"/>
  <input type="submit">
</form>

<Br>
<Br>


###### size  

**指的是以字符计算的可见宽度**

```html
<form>
  请输入你想找的内容: <input type="text" size="10" name="text"  />
  <input type="submit">
</form>
```

<form >
  请输入你想找的内容: <input type="text" size="10" name="text" />
  <input type="submit">
</form>

<Br>
<Br>

###### src

**在 `<input>` 里面，这个属性多用在 `type="image" 上`**

```html
<form>
  请输入你想找的内容: <input type="text" size="10" name="text"  />
  <input type="image" height="30" src="../img/chenqinchao.png" style="vertical-align:top">
</form>
```

<form >
  请输入你想找的内容: <input type="text" size="10" name="text" />
  <input type="image" height="30" src="../img/chenqinchao.png" style="vertical-align:top">
</form>

<Br>
<Br>

###### step

```html
<form>
  一次间隔是2: <input type="number" step="2" name="number"  />
  一次间隔是5: <input type="number" step="5" name="number"  />
  一次滑动间隔是3：<input type="range" step="3" min="1" max="10" name="range">
</form>
```

<form >
  一次间隔是2: <input type="number" step="2" name="number"  /><br>
  一次间隔是5: <input type="number" step="5" name="number"  /><br>
  一次滑动间隔是3：<input type="range" step="3" min="1" max="10" name="range">
</form>

<Br>
<Br>

#### 改变输入框的光标颜色

- 通过 caret-color 属性：

```copy
input{
    caret-color:yellow
}
```

<br>
<br>

- 通过 `:first-line` 伪元素：

```copy
input{
    color:black;
    &:first-line{
        color:yellow;
    }
}
```

<style>

form input{
    background:none;
    border:1px solid #eee;
}

form input[type="text"],input[type="number"]{
    height:30px;
    padding-left:10px;
    padding-right:10px;
}

form input[type="submit"]{
    height:30px;
    color:#fff;
    background:#a8a8a8;
}




 .slider1 {
    -webkit-appearance: none;
    max-width: 350px;
    width: 100%;
    height: 10px;
    outline: none;
  }
  .slider1::-webkit-slider-thumb{
      -webkit-appearance: none;/*清除默认样式*/
      height:25px;/*设置滑块高度*/
      width:25px;/*设置滑块宽度*/
      background: #fff;/*设置背景色*/
      border-radius:50%;/*加个圆角边*/
      /* margin-top:-1vw; 使用position的话会导致滑块不滑动,但是绑定的value是改变的,所以这里使用margin-top去做定位*/
      box-shadow: 0 1px 1px rgba(0,0,0,.5);
      cursor: pointer;
  }
  .slider1::-webkit-slider-runnable-track{
      border-radius: 30px;
      background:#128;
      height:25px;
  }
 
  .slider2 {
    -webkit-appearance: none;
    max-width: 350px;
    width: 100%;
    height: 10px;
    border-radius: 5px;
    background: #1B2B33;
    outline: none;
    margin-top: 50px;
    margin-bottom: 30px
  }
 
  .slider2::-webkit-slider-thumb {
    -webkit-appearance: none;
    appearance: none;
    width: 25px;
    height: 25px;
    border-radius: 50%;
    background: #fff;
    box-shadow: 0 1px 1px rgba(0,0,0,.5);
    border:1px solid #eee;
    cursor: pointer;
  }
 
  .slider2::-moz-range-thumb {
    width: 25px;
    height: 25px;
    border-radius: 50%;
    background: #fff;
    box-shadow: 0 1px 3px rgba(0,0,0,.1);
    cursor: pointer;
  }

</style>
