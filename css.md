### CSS编码规范

#### 空格

需要空格的情况：

* 属性值前
* 多个规则的分隔符`,`后
* `!important`的!前
* 选择器`+ > ~`前后

示例：

```css
/* 注释 */
.element,
.dialog {
    color: red !important;
    background-color: rgba(0, 0, 0, .5);
}

.element > .dialog{
    ...
}
```

#### 注释

注释`/*  */`内，前后有空格，勿使用`//`注释

示例：

```css
/* 
 * 多行注释 
 * 多行注释
 */
.element,
.dialog {
  /* 单行注释 */
  ···
}
```

#### 引号

* 最外层统一使用双引号
* url的内容要用引号
* 属性选择器中的属性值需要引号

示例：

```css
.element::after {
  content: "";
  background-image: url("logo.png");
}

li[data-type="single"] {
  ...
}
```

#### 命名

* 类名使用小写字母，以中划线分隔
* id采用驼峰式命名

示例：

```css
/* class */
.element-content {
  ...
}

/* id */
#myDialog {
  ...
}
```

#### 颜色

* 颜色16进制用小写字母
* 颜色16进制尽量用简写

示例：

```css
.element {
  color: #abcdef;
  background-color: #000;
}
```



