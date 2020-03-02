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
||||


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

