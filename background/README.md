
## background

`background` 是 `css` 的简写属性。用于一次性定义各种背景（`color`,`position`,`image`,`size`等等）属性。 

```copy
<style>
    div{
        width:200px;
        height:200px;
        background:red url('https://developer.mozilla.org/static/img/web-docs-sprite.22a6a085cf14.svg') 0 0 / 219px 48px no-repeat;
    }
</style>

<div></div>
```

### properties

|properties|value|
|---|---|
|background-color|`rgba()`,`rgb()`,`hsla()`,`#fff`,`white`,`transparent`,`currentColor`,<br>`inherit`,`initial`,`unset`,`none`,`*gradient`|
|background-image|`url`,`none`,`inherit`|
|background-repeat|`repeat-x`,`repeat-y`|
|background-attachment|`fixed`,`scroll`,`local`,`inherit`,`initial`,`unset`|
|background-position|`0 0 `,`10px 10px`,`10% 10%`,`center left`|
|background-origin||
|background-clip||
|background-size||
|background-clip||
|background-blend-mode||

>`unset` 表示没有设置，即继承父级的值。 `unset` 可以被用在许多其他属性，比如说 `color`

```copy
<style>
.parents{
    background:red
}
.child-1{
    background:green;
}
.child-2{
    background:unset;
}
</style>

<div class="parents">
    <div class="child-1">child-1</div>              // 绿色的背景
    <div class="child-2">child-2</div>              // 继承父级属性值红色的背景
</div>
```
