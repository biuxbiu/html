## input

```javascript
<input>             //没有结束标签
```

#### input的属性和类型

|属性|值|描述|
|::-|::-|::-|
|accept|audio/* video/* image/* MIME_type|规定提交的文件类型（针对 type="file" 存在）|
|alt|text|定义图像的替代文本|
|autocomplete|on/off|启动或者关闭是否采用自动完成功能|
|autofocus|autofocus|表示页面在加载时该元素自动获得焦点|
|checked|checked|表示页面在加载时预先选定该元素|
|disabled|disabled|表示该元素被禁用|
|form|form_id|包含多个表单|
|formaction|url|表示表单在提交的时候，输入控件的URL地址（针对 type="submit" / type="image" 存在）|
|formenctype|application/x-www-form-urlencoded multipart/form-data text/plain|表示提交表格时的编码格式|
|formmethod|get/post|提交的方法（针对 type="submit" / type="image" 存在）|
|formnovalidate|formnovalidate|覆盖表单的 novalidate 属性。如果使用该属性，则提交表单时不进行验证。|
|formtarget|_blank<br>_self<br>_parent<br>_top<br>framename|覆盖表单的 target 属性。（适用于 type="submit" 和 type="image"）|
|height|px<br>%|设置 `<input>` 的高度|
|list⭐️⭐️⭐️|datalist-id|表示输入字段的预选项|
|max|number<br>date|与 `min` 相结合使用，设置合法值范围，适用于以下 `<input>` 类型：number, range, date, datetime, datetime-local, month, time 以及 week|
|min|number<br>date|与 `max` 相结合使用，设置合法值范围，适用于以下 `<input>` 类型：number, range, date, datetime, datetime-local, month, time 以及 week|
|max-length|number|允许字符的最大长度|
|multiple|multiple|允许一次性选择多个，一般与 `type="file"` 结合使用|
|name|field_name|表示 `<input>` 的名称|
|pattern|regexp_pattern|设定输入字段的格式 pattern="[0-9]" 表示必须是 0 到 9 之间的数字|
|placeholder|text|用户填写提示|
|readonly|readonly|设置为只读|
|required|required|定义这个输入框在提交表格的时候必填项，如果有该属性，则该字段是必填或者必选|
|size|number_of_char|定义的是**以像素为单位**的输入字段宽度（定义输入框的宽度）|
|src|url|定义以提交按钮显示出来的图片的URL|
|step⭐️⭐️⭐️|number|规定输入字的的合法数字间隔（以这个间隔变化）|
|type⭐️⭐️⭐️|button<br>checkbox<br>file<br>hidden<br>image<br>password<br>radio<br>reset<br>submit<br>text|按钮<br>多选框<br>文件上传<br>隐藏的文本<br>按钮形式的图片<br>密码形式<br>单选<br>重置按钮<br>提交按钮<br>文字输入框|
|value|value|规定 `<input>` 元素的值|
|width|pixel<br>%|定义 input 字段的宽度。（适用于 type="image"）|


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

```

