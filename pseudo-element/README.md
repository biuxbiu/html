
### first-line

`::first-line` 表示某个 `块级元素` 文本中的第一行。

>`::first-line` 只能在 `display` 为 `inline-block`, `block`, `table-cell`, `table-caption` 的块级元素中起作用。

```copy
<style>
.text{
    width:100px;
}
.text::first-line{
    margin:100px;
    padding:100px;
    text-indent:100px;
}
</style>

<div class="text">
The ::first-line CSS pseudo-element applies styles to the first line of a block-level element. Note that the length of the first line depends on many factors, including the width of the element, the width of the document, and the font size of the text.
</div>
```

!>目前看来，在这个伪元素上只有可以做出的效果比较少，只有很小的一部分css属性能被使用，比如说：文字相关 `font`，字体颜色相关 `color`,背景相关 `background`,

*   字体相关属性：`font properties`
*   字体颜色属性：`color properties`
*   文字间距属性：`word-spacing`, `letter-spacing`, `text-decoration`, `text-transform`, and `line-height`。
*   文字修饰属性：`text-shadow`, `text-decoration`, `text-decoration-color`, `text-decoration-line`, `text-decoration-style`, and `vertical-align`。
*   背景相关属性：`background properties`
*   其他相关属性：`box-shadow`, `clear`

!>`text-indent`，`margin`，`padding` 这些值在该伪类元素上是无效的。如果不在上述的属性列表中的话，需要慎用。

