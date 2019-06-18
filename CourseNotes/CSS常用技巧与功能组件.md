@[TOC](目录)

# 常用技巧
## 透明度的兼容方案
```css
.transparent_class {  
    filter:alpha(opacity=50);// IE
    -moz-opacity:0.5; // old moz
    -khtml-opacity: 0.5; // old safari
    opacity: 0.5; // modern 
}
```

## 限制文本宽度、不换行、超过的文本以...结束 
```css
max-width: 200px;          // 设定宽度
overflow: hidden;          // 超过设定宽度时隐藏
white-space: nowrap;       // 超过设定宽度时候不换行
text-overflow: ellipsis;   // 超过设定文本宽度时以...结束
```
## 图片垂直居中的技巧
```html
<div class="img_wrap bgBlack">
    <span></span>
    <img src="http://images2015.cnblogs.com/blog/735803/201610/735803-20161009100152788-1795831908.png" alt="" />
</div>
<style>
    .img_wrap span {
        display: inline-block;
        height: 100%;
        vertical-align: middle;
    }
    .img_wrap img {
        vertical-align:middle;
    }
</style>
```
## 弹性宽度与固定列


```html
<style>
    #d6_1 {
        width: 100%;
        float: left;
    }
    #d6_1_1 {
        margin-right: 160px;
    }
    #d6_2{
        float:left;
        margin-left: -160px;
        width: 160px;
    }
</style>
<div class="clear">
    <div id="d6_1">
        <div id="d6_1_1" class="bgGray">xxx</div>
    </div>
    <div id="d6_2" class="bgBlack">xxx</div>
</div>
```



## 文字环绕图片

```html
<div id="d4">
    <img src="http://images2015.cnblogs.com/blog/735803/201610/735803-20161009100152788-1795831908.png" width="100" />测试文字fjksdjfksdjfkdsj测试文字fjksdjfksdjfkdsj测试文字fjksdjfksdjfkdsj
</div>
<style>
    #d4{
        width:200px;
        word-break: break-all;
    }
    #d4 img{
        float: left;
    }
</style>
```
## 文本居中

```html
<div id="d3" class="borderRed">
    <p>juzhong</p>
</div>
<style>
    #d3 p {
        line-height: 200px;
        text-align: center;
    }
</style>
```
## 图片居中
```html
<div class="img_wrap bgBlack">
    <span></span>
    <img src="http://images2015.cnblogs.com/blog/735803/201610/735803-20161009100152788-1795831908.png" alt="" />
</div>
<style>
    .img_wrap {
        width: 500px;
        height: 500px;
        text-align: center;
    }
    .img_wrap span {
        display: inline-block;
        height: 100%;
        vertical-align: middle; 
    }
    .img_wrap img {
        vertical-align:middle;
    }
</style>
```
## 块元素居中

* 对于正常文档流的元素：利用margin:auto

* 对于绝对定位和固定定位的元素：利用top和left设置成50%且margin-left和margin-top设置成对应宽高的一半

```html
<div id="d2">
    <div id="d2_1" class="borderRed" > </div>
</div>
<style>
    #d2{
        position: relative;
        height: 200px;
    }
    #d2_1{
        position: absolute;
        top:50%;
        left:50%;
        margin-left: -50px;
        margin-top: -50px;
        width:100px;
        height:100px;
        box-sizing: border-box;
        background: darkblue;
    }
</style>
```
## 清除浮动



```html
<div id="d1" class="clear">
    <div id="d1_1"></div>
    <div id="d1_2"></div>
</div>
<style>
    .clear:after{
        content:'';
        display:block;
        clear:both;
        height:0;
        overflow:hidden;
        visibility:hidden;
    }
    .clear{zoom:1;}
    #d1 {
        background-color: #cccccc;
        border: 2px solid red;
    }
    #d1_1 {
        background-color: #aaaaaa;
        border: 2px solid yellow;
        width: 100px;
        height: 100px;
        float: left;
    }
    #d1_2 {
        background-color: #888888;
        border: 2px solid green;
        width: 100px;
        height: 100px;
        float: left;
    }
</style>
```
## 弹性宽度与固定列



```html
<div id="d6" class="clear">
    <div id="d6_1">
        <div id="d6_1_1" class="bgGray">xxx</div>
    </div>
    <div id="d6_2" class="bgBlack">xxx</div>
</div>
<style>
    #d6_1 {
        width: 100%;
        float: left;
    }
    #d6_1_1 {
        margin-right: 160px;
    }
    #d6_2{
        float:left;
        margin-left: -160px;
        width: 160px;
    }
</style>
```
## 下拉菜单隐藏与显示

利用伪类元素切换显示属性

```html
<ul id="d5">
    <li>
        <a href="#">li-1</a>
    </li>
    <li>
        <a href="#">li-2</a>
        <ul>
            <li><a href="#">li-2-1</a></li>
            <li><a href="#">li-2-2</a></li>
        </ul>
    </li>
</ul>
<style>
    #d5>li{
        position: relative;
		float:left;
        width: 40%;
        height: 96px;
        background: lightgreen;
    }
    #d5 li a{
        display: inline-block;
        width: 100%;
        text-align: center;
        line-height: 96px;
    }
    #d5>li ul {
        position: absolute;
        left: 0;
        top: 96px;
    }
    #d5 ul {
        width: 100%;
        display: none;
    }
    #d5 li ul li{
        width: 100%;
        height: 96px;
        background: green;
        text-align: center;
        line-height: 96px;
    }
    #d5 a:hover{
        background: yellow;
    }
    #d5>li:hover ul{
        display: block;
    }
</style>
```

