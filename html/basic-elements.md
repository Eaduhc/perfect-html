# 基础元素

> 首先介绍一些与段落文字相关的基本元素。

创建 `epigrams.html` 并用编辑器打开，将下面的代码写到编辑器中：

```html
<!DOCTYPE html>
<html>
    
<head>
    <title>Epigrams on Programming</title>
</head>
    
<body>
    One man's constant is another man's variable.
</body>
    
</html>
```

## 段落元素 `<p>`

HTML 对于任何数量的空白字符都会被转换为一个空格，所以像下面代码一样使用空白行是不能实现分段效果的：

```html
<!-- 不能实现分段 -->
<body>
    One man's constant is another man's variable.

    吾之常量，彼之变量。
</body>
```

`<p>` 元素的作用就是将文字标记为段落：

```html
<p>这是一个段落</p>
```

使用 `<p>` 元素给我们的代码分段如下：

```html
<body>
    <p>One man's constant is another man's variable.</p>
    <p>吾之常量，彼之变量。</p>
</body>
```

## 标题元素 `<h1>`-`<h6>`

如果想给页面中的内容加标题，可以使用 `<h1>` 到 `<h6>` 的标题元素，`<h1>` 的级别最高，`<h6>` 的级别最低。浏览器中主要表现为 `<h1>` 最大，`<h6>` 最小：

```html
<h1>一级标题</h1>
<h2>二级标题</h2>
<h3>三级标题</h3>
<h4>四级标题</h4>
<h5>五级标题</h5>
<h6>六级标题</h6>
```

可以给我们的代码中加入一些标题和段落来丰富页面的内容：

```html
<body>
    <h1>Epigrams on Programming 编程警句</h1>
    <h2>Preface 前言</h2>
    <p>
        The phenomena surrounding computers are diverse and yield a surprisingly rich base for launching metaphors at individual and group activities. Conversely, classical human endeavors provide an inexhaustible source of metaphor for those of us who are in labor within computation. Such relationships between society and device are not new, but the incredible growth of the computer's influence (both real and implied).lends this symbiotic dependency a vitality like a gangly youth growing out of his clothes within an endless puberty.
    </p>
    <p>
        The epigrams that follow attempt to capture some of the dimensions of this traffic in imagery that sharpens, forcuses, clarifies, enlarges and beclouds our view of this most remarkable of all roans' artifacts, the computer.
    </p>
    <h2>Epigrams 警句</h2>
    <p>One man's constant is another man's variable.</p>
    <p>吾之常量，彼之变量。</p>
</body>
```

## 无序列表 `<ul>` `<li>`

编程警句有很多条，我们当然可以像之前一样继续一段一段的写下去，但还可以用更好的方法去实现。

`<ul>` 是无序列表元素，可以用来在 HTML 中添加一个无序列表，用 `<li>` 表示列表中的每一项：

```html
<p>这是一个无序列表：</p>
<ul>
  <li>首先添加一个 "ul" 元素</li>
  <li>再给列表的每一项添加一个 "li" 元素</li>
  <li>最后在 "li" 元素中添加内容</li>
</ul>
```

利用无序列表多添加几条警句到页面中：

```html
<h2>Epigrams 警句</h2>
<ul>
    <li>
        <p>One man's constant is another man's variable.</p>
        <p>吾之常量，彼之变量。</p>
    </li>
    <li>
        <p>Functions delay binding: data structures induce binding. Moral: Structure data late in the programming process.</p>
        <p>函数推迟绑定；数据结构导致绑定。</p>
    </li>
    <li>
        <p>Syntactic sugar causes cancer of the semi-colons.</p>
        <p>语法糖导致分号癌。</p>
    </li>
    <li>
        <p>Every program is a part of some other program and rarely fits.</p>
        <p>每个程序都是其他程序不合适的一部分。</p>
    </li>
    <li>
        <p>If a program manipulates a large amount of data, it does so in a small number of ways.</p>
        <p>如果一个程序用于处理大量数据，它就没几种选择了。</p>
    </li>
</ul>
```

## 有序列表 `<ol>` `<li>`

和无序列表类似，HTML 也提供了添加有序列表的方法。

`<ol>` 是有序列表元素，可以在页面中添加一个有序列表，列表中的每一项也用 `<li>` 元素表示：

```html
<p>这是一个有序列表：</p>
<ol>
  <li>首先添加一个 "ol" 元素</li>
  <li>再给列表的每一项添加一个 "li" 元素</li>
  <li>最后在 "li" 元素中添加内容</li>
</ol>
```

现在我们把警句代码中的无序列表换成有序列表：

```html
<h2>Epigrams 警句</h2>
<ol>
	...
</ol>
```

## 强调元素 `<em>`

`<em>` 元素将文本标记为强调格式，通常在浏览器中表现为斜体：

```html
<em>这是要强调的内容</em>
```

使用强调元素将警句的英文标记：

```html
<h2>Epigrams 警句</h2>
<ol>
    <li>
        <p><em>One man's constant is another man's variable.</em></p>
        <p>吾之常量，彼之变量。</p>
    </li>
    <li>
        <p><em>Functions delay binding: data structures induce binding. Moral: Structure data late in the programming process.</em></p>
        <p>函数推迟绑定；数据结构导致绑定。</p>
    </li>
    <li>
        <p><em>Syntactic sugar causes cancer of the semi-colons.</em></p>
        <p>语法糖导致分号癌。</p>
    </li>
    <li>
        <p><em>Every program is a part of some other program and rarely fits.</em></p>
        <p>每个程序都是其他程序不合适的一部分。</p>
    </li>
    <li>
        <p><em>If a program manipulates a large amount of data, it does so in a small number of ways.</em></p>
        <p>如果一个程序用于处理大量数据，它就没几种选择了。</p>
    </li>
</ol>
```

## Strong 元素 `<strong>`

`<strong>` 元素表示文本十分重要，通常在浏览器中表现为粗体：

```html
<strong>这是十分重要的内容</strong>
```

可以使用 `<strong>` 元素标记警句的翻译：

```html
<h2>Epigrams 警句</h2>
<ol>
    <li>
        <p><em>One man's constant is another man's variable.</em></p>
        <p><strong>吾之常量，彼之变量。</strong></p>
    </li>
    <li>
        <p><em>Functions delay binding: data structures induce binding. Moral: Structure data late in the programming process.</em></p>
        <p><strong>函数推迟绑定；数据结构导致绑定。</strong></p>
    </li>
    <li>
        <p><em>Syntactic sugar causes cancer of the semi-colons.</em></p>
        <p><strong>语法糖导致分号癌。</strong></p>
    </li>
    <li>
        <p><em>Every program is a part of some other program and rarely fits.</em></p>
        <p><strong>每个程序都是其他程序不合适的一部分。</strong></p>
    </li>
    <li>
        <p><em>If a program manipulates a large amount of data, it does so in a small number of ways.</em></p>
        <p><strong>如果一个程序用于处理大量数据，它就没几种选择了。</strong></p>
    </li>
</ol>
```

## 空元素

在此之前遇到的 HTML 元素都有开始和结束标签可以把其他的元素和内容包起来。除此之外，在 HTML 中还有一些没有结束标签、不能包住其他元素和内容的元素叫做空元素。下面介绍几种常见的空元素。

### 换行元素 `<br>`

`<br>` 元素在文本中生成一个换行符号，可以在需要换行的地方使用：

```html
这是第一行<br>
这是第二行
```

可以在所有警句的最后添加一个空行：

```html
<h2>Epigrams 警句</h2>
<ol>
	...
</ol>
<br>
```

### 主题分割元素 `<hr>`

`<hr>` 元素可以表示不同主题内容的转换，通常在浏览器中表现为一条水平线：

```html
<p>主题内容1</p>
<hr>
<p>主题内容2</p>
```

在警句最后添加一点脚标信息并利用空行和水平线来分割内容：

```html
<h2>Epigrams 警句</h2>
<ol>
	...
</ol>
<br>
<hr>
<br>
<p>Created by Eaduhc</p>
```

到这里，与段落文字相关的常见元素的介绍和编程警句的页面就都完成了。