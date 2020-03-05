## progress

标示任务的进度（进程）

```javascript
<progress></progress>
```

#### input的属性和类型

<br>



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

