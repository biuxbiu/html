
# 黑科技汇总

`css` 里面有一些很特别的黑科技，这里我汇集了一些，不停更新中。

#### 不一样的下拉框

使用 `<input>` 属性 `list="id"` 做出不一样的下拉框

```html
<form>
  letter: <input list="letter"/>
  <dadalist id="letter">
    <option value="A">
    <option value="B">
    <option value="c">
    <option value="d">
  </dadalist>
</form>
```

<form >
  letter: <input list="letter">
  <datalist id="letter">
    <option value="A">
    <option value="B">
    <option value="c">
    <option value="d">
  </datalist>
</form>

<Br>
<Br>

#### 改变输入框的光标颜色

- 通过 caret-color 属性：

```html
input{
    caret-color:yellow
}
```

<br>
<br>

- 通过 `:first-line` 伪元素：

```css
input{
    color:black;
    &:first-line{
        color:yellow;
    }
}
```





#### 设置最小起始时间和最大结束之间

使用 `max` 和 `min` 属性

```html
<form action="demo_form.html">
  结束时间最晚不能晚于 1980-01-01:
  <input type="date" name="bday" max="1979-12-31">

  起始时间最小不能小于 2020-01-02:
  <input type="date" name="bday" min="2020-01-02">

  限定数字在 1 - 5 之间:
  <input type="number" name="quantity" min="1" max="5">

  <input type="submit">
</form>
```

<form action="demo_form.html">
  结束时间最晚不能晚于 1980-01-01:
  <input type="date" name="bday" max="1979-12-31">

  起始时间最小不能小于 2020-01-02:
  <input type="date" name="bday" min="2020-01-02">

  限定数字在 1 - 5 之间:
  <input type="number" name="quantity" min="1" max="5">

  <input type="submit">
</form>

<Br>
<Br>


#### 原生的数字控件

###### 可滑动的数字空间

>要改原生滑块的样式，最主要是记住两个属性<br>
`::-webkit-slider-thumb`：滑块的样式<br>
`::-webkit-slider-runnable-track`：滑块轨道的样式

```html
<input class="rangeOne" type="range" min="1" max="100" step="1">
<input class="rangeTwo" type="range" min="1" max="100" step="1">

<style>
</style>
```

<input class="rangeOne" type="range" value="0" min="1" max="100" step="1">
<input class="rangeTwo" type="range" value="0" min="1" max="100" step="1">

<style>
.rangeOne {
-webkit-appearance: none;
max-width: 350px;
width: 100%;
height: 10px;
outline: none;
}
.rangeOne::-webkit-slider-thumb{
    -webkit-appearance: none;/*清除默认样式*/
    height:25px;/*设置滑块高度*/
    width:25px;/*设置滑块宽度*/
    background: #fff;/*设置背景色*/
    border-radius:50%;/*加个圆角边*/
    /* margin-top:-1vw; 使用position的话会导致滑块不滑动,但是绑定的value是改变的,所以这里使用margin-top去做定位*/
    box-shadow: 0 1px 1px rgba(0,0,0,.5);
    cursor: pointer;
}
.rangeOne::-webkit-slider-runnable-track{
    border-radius: 30px;
    background:#128;
    height:25px;
}

.rangeTwo {
    -webkit-appearance: none;
    max-width: 350px;
    width: 100%;
    height: 10px;
    border-radius: 5px;
    background: #1B2B33;
    outline: none;
    margin-top: 50px;
    margin-bottom: 30px
}

.rangeTwo::-webkit-slider-thumb {
    -webkit-appearance: none;
    appearance: none;
    width: 25px;
    height: 25px;
    border-radius: 50%;
    background: #fff;
    box-shadow: 0 1px 1px rgba(0,0,0,.5);
    border:1px solid #eee;
    cursor: pointer;
}

.rangeTwo::-moz-range-thumb {
    width: 25px;
    height: 25px;
    border-radius: 50%;
    background: #fff;
    box-shadow: 0 1px 3px rgba(0,0,0,.1);
    cursor: pointer;
}
</style>

<br>
<br>

- 通过 `:first-line` 伪元素：

```html
input{
    color:black;
    &:first-line{
        color:yellow;
    }
}
```

#### 修改style标签样式实时刷新页面内容

!>这里最主要是设置 `style` 标签是可见的并且可编辑的来实现实时修改样式并且页面回应的效果

```css
<style style="display:block" contenteditable="true">
    body{
        background:#fff
    }
</style>
```

**你可以尝试改变下面的 `css` 样式看看效果**

<style style="display:block" contenteditable="true">
    body{
        background:#fff
    }
</style>

<style>

form input{
    background:none;
    border:1px solid #eee;
}

form input[type="text"]{
    height:30px;
    padding-left:10px;
    padding-right:10px;
}

form input[type="submit"]{
    height:30px;
    color:#fff;
    background:#a8a8a8;
}
</style>
