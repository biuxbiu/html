## input

#### text类型

```copy
<input type="text">
```

<br>
<br>

**改变输入框的光标颜色**


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

