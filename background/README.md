
## background

`background` 是 `css` 的简写属性。用于一次性定义各种背景（`color`,`position`,`image`,`size`等等）属性。 

时至今日的 `background` 简写已经扩展支持跟多的背景属性。

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
|background-color|`rgba()`,`rgb()`,`hsla()`,`#fff`,<br>`white`,`transparent`,`currentColor`,<br>`inherit`,`initial`, <span class="special-orange">`unset`</span> ,`none`,`*gradient`|
|background-image|`url`,`none`,`inherit`|
|background-repeat|`repeat-x`,`repeat-y`,`repeat`,`no-repeat`,`inherit`|
|background-attachment|`fixed`,`scroll`,`local`,`inherit`,`initial`, <span class="special-orange">`unset`</span>|
|background-position|`0 0 `,`10px 10px`,`10% 10%`,`center left`|
|background-origin|`padding-box`,`content-box`,`border-box`|
|background-clip|`padding-box`,`content-box`,`border-box`,`text`|
|background-size|`contain`,`cover`,`30%`,`100px`|
|background-blend-mode|`normal`,`multiply`,`screen`,<br>`overlay`,`darken`,`lighten`,`color-dodge`,<br>`color-burn `,`hard-light`,<br>`soft-light`,`difference`,`exclusion`,<br>`hue`,`saturation`,`color`,`luminosity`|

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
