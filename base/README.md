# Vuejs

本文是基于<svg class="iconTag" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" width="70" height="20"><linearGradient id="b" x2="0" y2="100%"><stop offset="0" stop-color="#bbb" stop-opacity=".1"/><stop offset="1" stop-opacity=".1"/></linearGradient><clipPath id="a"><rect width="70" height="20" rx="3" fill="#fff"/></clipPath><g clip-path="url(#a)"><path fill="#555" d="M0 0h31v20H0z"/><path fill="#97ca00" d="M31 0h39v20H31z"/><path fill="url(#b)" d="M0 0h70v20H0z"/></g><g fill="#fff" text-anchor="middle" font-family="DejaVu Sans,Verdana,Geneva,sans-serif" font-size="110"> <text x="165" y="150" fill="#010101" fill-opacity=".3" transform="scale(.1)" textLength="210">vue</text><text x="165" y="140" transform="scale(.1)" textLength="210">vue</text><text x="495" y="150" fill="#010101" fill-opacity=".3" transform="scale(.1)" textLength="290">2.9.6</text><text x="495" y="140" transform="scale(.1)" textLength="290">2.9.6</text></g> </svg>版本所总结的知识笔记，主要帮助团队成员快速理解技术关键词汇与重点难点。各关键点会在后续独立成一篇研究课题。

## webpack的使用
`webpack` 有一个比较大的用处就是将浏览器不能直接识别的语言转换成浏览器能够识别的语言。

语法：
```copy
webpack index.js builde.js          //将 `index.js` 打包成 `build.js`
```

## commonjs
`commonjs` 的存在主要是为了弥补<b>js没有模块化</b>的概念。

在 `commonjs` 的规范中：
* 一个文件就是一个模块，拥有单独的作用域，不会污染全局作用域；
* 普通方式定义的变量、函数、对象都属于这个模块内；
* 模块通过 `require` 的方式加载； 
* 模块可以通过 `exports` 和 `module.exports` 来暴露模块中的内容；

## 各种各样的export
`export`
`export default`
`exports`
`modules.exprots`

`export` 是 `nodejs` 里面模块化的概念。

## sass的使用
要使用 `sass` 需要安装一下依赖才可以：
* node-sass
* sass-loader

```copy
npm install node-sass sass-loader -D
```

#### 内部sass
我们可以直接在 `vue` 的组件里面书写 `sass`。

```copy
<style lang="scss">             //要设置 `lang="scss"`
    $bg:blue;
    body{
        background:$bg;
    }
</style>
```


#### 外部sass
```copy
<style lang="scss">             //要设置 `lang="scss"`
@import "@/assets/scss/index.scss"
</style>
```
