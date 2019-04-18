
## first-line

`:first-line` 表示某个 `块级元素` 中的第一行。

>`:first-line` 只能在 `display` 为 `inline-block`, `block`, `table-cell`, `table-caption` 中起作用。

```copy
<style>
.text{
    width:100px;
}
.text:first-line{
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

*   所有和字体有关的属性：`font`, `font-kerning`, `font-style`, `font-variant`, `font-variant-numeric`, `font-variant-position`, `font-variant-east-asian`, `font-variant-caps`, `font-variant-alternates`, `font-variant-ligatures`, `font-synthesis`, `font-feature-settings`, `font-language-override`, `font-weight`, `font-size`, `font-size-adjust`, `font-stretch`, 和 `font-family`。
*   和文字间距有关的属性：`word-spacing`, `letter-spacing`, `text-decoration`, `text-transform`, and `line-height`。
*   和文字修饰有关的属性：`text-shadow`, `text-decoration`, `text-decoration-color`, `text-decoration-line`, `text-decoration-style`, and `vertical-align`。
*   所有和背景有关的属性：`background-color`, `background-clip`, `background-image`, `background-origin`, `background-position`, `background-repeat`, `background-size`,  `background-attachment`, and `background-blend-mode`。
*   `box-shadow`

!>`text-indent`，`margin`，`padding` 这些值在改伪类元素上是无效的。如果不在上述的属性列表中的话，需要慎用。

