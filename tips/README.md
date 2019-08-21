## 黑科技

这里我会把一些比较有用的知识点归类起来，形成一个快速查看黑科技的一个入口。

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

