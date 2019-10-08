---
title: 回顾html
date: 2019-10-08 12:28:11
tags: HTML
---

对html语言进行了回顾和再次学习。



## html样式

一些标签和属性都用html中的style属性所代替了。

#### 被抛弃的标签和属性

| 标签/属性                       | 描述              |
| ------------------------------- | ----------------- |
| \<center>                       | 定义居中的内容    |
| \<font>和\<basefont>            | 定义HTML字体      |
| \<s>和\<strike>(使用\<del>代替) | 定义删除线文本    |
| \<u>(使用样式\<ins>代替)        | 定义下划线文本    |
| align                           | 定义文本对齐方式  |
| bgcolor/color                   | 定义背景/文本颜色 |



## html折行

使用\<br />标签:

```html
<p>This is<br />a para<br />graph with line breaks</p>
```



## 文本格式化标签

| 标签      | 效果                      |
| --------- | ------------------------- |
| \<p>      | 正常                      |
| \<big>    | <big>大号</big>           |
| \<em>     | <em>着重</em>             |
| \<i>      | <i>斜体</i>               |
| \<small>  | <small>小号</small>       |
| \<b>      | <b>粗体</b>               |
| \<strong> | <strong>加强语气</strong> |
| \<sub>    | 正常<sub>下标</sub>       |
| \<sup>    | 正常<sup>上标</sup>       |
| \<ins>    | <ins>插入</ins>           |
| \<del>    | <del>删除</del>           |

#### “计算机输出“标签

| 标签    | 效果                  |
| ------- | --------------------- |
| \<code> | <code>prinf()</code>  |
| \<kbd>  | <kbd>space</kbd>      |
| \<pre>  | <pre>预格式文本</pre> |
| \<var>  | <var>变量</var>       |
| \<tt>   | <tt>打字机格式</tt>   |

\<code> 元素不保留多余的空格和折行，用\<pre>解决。

```
<code>
<pre>
var person = {
    firstName:"Bill",
    lastName:"Gates",
    age:50,
    eyeColor:"blue"
}
</pre>
</code>
```

效果：

<code>

<pre>
var person = {
    firstName:"Bill",
    lastName:"Gates",
    age:50,
    eyeColor:"blue"
}
</pre>
</code>

#### 引用和术语定义

| 标签                   | 效果                                                         |
| ---------------------- | ------------------------------------------------------------ |
| \<abbr>(缩写)          | <abbr title="etcetera">etc.</abbr>                           |
| \<acronym>(首字母缩写) | <acronym title="World Wide Web">WWW</acronym>                |
| \<q>                   | <q>引用，周围有引号</q>                                      |
| \<bdo>(dir="rtl")      | <bdo dir="rtl">Reverse</bdo>                                 |
| \<dfn>                 | <p><dfn title="World Health Organization">WHO</dfn> 成立于 1948 年。</p> |



## HTML 链接 - target 属性

下面的这行会在新窗口打开文档：

```
<a href="http://www.w3school.com.cn/" target="_blank">Visit W3School!</a>
```



## HTML 链接 - name 属性

首先，我们在 HTML 文档中对锚进行命名（创建一个书签）：

```
<a name="tips">基本的注意事项 - 有用的提示</a>
```

然后，我们在同一个文档中创建指向该锚的链接：

```
<a href="#tips">有用的提示</a>
```

您也可以在其他页面中创建指向该锚的链接：

```
<a href="http://www.w3school.com.cn/html/html_links.asp#tips">有用的提示</a>
```



## div与span的区别

div是块级元素，可以用于布局。
span是内联元素，多用于为部分文本设置不一样的样式。



## HTML文件路径

| 路径                             | 描述                                         |
| :------------------------------- | :------------------------------------------- |
| \<img src="picture.jpg">         | picture.jpg 位于与当前网页相同的文件夹       |
| \<img src="images/picture.jpg">  | picture.jpg 位于当前文件夹的 images 文件夹中 |
| \<img src="/images/picture.jpg"> | picture.jpg 当前站点根目录的 images 文件夹中 |
| \<img src="../picture.jpg">      | picture.jpg 位于当前文件夹的上一级文件夹中   |
