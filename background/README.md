
## background

`background` 是 `css` 的简写属性。用于一次性定义各种背景属性。 

时至今日的 `background` 简写已经扩展支持更多的背景属性，有 `background-clip`，`background-color`，`background-image`，`background-origin`，`background-position`，`background-repeat`，`background-size`，`background-attachment`。

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
|background-color|`rgba()`,`rgb()`,<span class="special-orange">`hsla()`</span>,`#fff`,<br>`white`,`transparent`,`currentColor`,<br>`inherit`,`initial`, <span class="special-orange">`unset`</span> ,`none`,`*gradient`|
|background-image|`url`,`none`,`inherit`|
|background-repeat|`repeat-x`,`repeat-y`,`repeat`,`no-repeat`,`inherit`|
|background-attachment|`fixed`,`scroll`,`local`,`inherit`,`initial`, <span class="special-orange">`unset`</span>|
|background-position|`0 0 `,`10px 10px`,`10% 10%`,`center left`|
|background-origin|`padding-box`,`content-box`,`border-box`|
|background-clip|`padding-box`,`content-box`,`border-box`,`text`|
|background-size|`contain`,`cover`,`30%`,`100px`|
|background-blend-mode|`normal`,`multiply`,`screen`,<br>`overlay`,`darken`,`lighten`,`color-dodge`,<br>`color-burn `,`hard-light`,<br>`soft-light`,`difference`,`exclusion`,<br>`hue`,`saturation`,`color`,`luminosity`|

!>`unset` 表示没有设置。<br> 
它的作用同等于 `initial` 和 `inherit`。

当该属性有默认继承的属性的时候， `unset` = `inherit`；<br>
当该属性没默认继成的属性的时候， `unset` = `intial`；


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

!>`hsla` <br>
`h(Hue)`：色调，`0` 或者 `360` 表示红色，120表示绿色，240表示蓝色;<br>
`s(Saturation)`：饱和度，0.0% - 100%；<br>
`l(Light)`：亮度，0.0% - 100%；<br>
`a(Alpha)`：透明度；

### background-color
