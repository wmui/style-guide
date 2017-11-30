### HTML规范

#### 语法

* 属性值使用双引号非单引号
* 属性值全小写，中划线分割
* 属性值使用英文全称书写，特殊情况可使用拼音，不可拼音加英文混合使用

示例：

```html
<!DOCTYPE html>
<html lang="zh">
<head>
  <meta charset="UTF-8">
  <title>Document</title>
</head>
<body>
  <div class="hello-world"> hello world </div>
</body>
</html>
```

#### IE兼容模式

示例：

```html
<!DOCTYPE html>
<html lang="zh">
<head>
  <meta http-equiv="X-UA-Compatible" content="IE=Edge">
  <meta charset="UTF-8">
  <title>Document</title>
</head>
<body>
  <div class="hello-world"> hello world </div>
</body>
</html>
```

#### CSS, JS文件的引入

根据HTML5规范, 在引入CSS和JS时不需要指明`type`，因为`text/css`和`text/javascript`

示例：

```html
<!-- 外联css -->
<link rel="stylesheet" href="code_guide.css">

<!-- 内联css -->
<style>
    ...
</style>

<!-- 外链js -->
<script src="code_guide.js"></script>

<!-- 内联js -->
<script>
    ...
</script>
```

#### 属性顺序

特定顺序的属性排列使可读性更好

* `class`
* `id`
* `name`
* `data-*`
* `src`,`for`,`type`,`href`,`value`,`max-length`,`max`,`min`,`patter`
* `placeholder`,`title`,`alt`

示例：

```html
<a class="..." id="..." data-modal="toggle" href="#">Example link</a>

<input class="form-control" type="text">

<img src="..." alt="...">
```

### Boolean属性

boolean属性指不需要声明取值的属性，boolean属性的存在表示取值为true，不存在则表示取值为false

示例：

```html
<input type="text" disabled>

<input type="checkbox" value="1" checked>

<select>
  <option value="1" selected>1</option>
</select>
```



