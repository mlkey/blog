---
title: Markdown Syntax for this Blog
updated: 2018-04-19 22:24
---

> 这篇博文用来展示适用于本博客的 **Markdown** 语法规则及排版规范，备查。本博客使用的 Markdown 解析器为 [kramdown](https://kramdown.gettalong.org/).

<div class="divider"></div>

## 标题 {#id1}
```md
# 一级标题
## 二级标题
### 三级标题
#### 四级标题
##### 五级标题
###### 六级标题
```
<h1>一级标题</h1>
<h2>二级标题</h2>
<h3>三级标题</h3>
<h4>四级标题</h4>
<h5>五级标题</h5>
<h6>六级标题</h6>
Markdown 是一种轻量级标记语言，它允许人们使用易读易写的纯文本格式编写文档，然后转换成格式丰富的 HTML 页面。Markdown 的理念是，能让文档更容易读、写和随意改。HTML 是一种发布的格式，Markdown 是一种书写的格式。就这样，Markdown 的格式语法只涵盖纯文本可以涵盖的范围。

<div class="divider"></div>

## 目录 {#id2}
```md
* TOC
{:toc}
```
* TOC
{:toc}

<div class="divider"></div>

## 强调 {#id3}
```md
*斜体文字*，**加粗文字**，***粗斜体***，~~删除线~~，`行内代码高亮`，
[超链接](http://lowshi.com/blog)，[回到顶部](#)
```
*斜体文字*，**加粗文字**，***粗斜体***，~~删除线~~，`行内代码高亮`，[超链接](http://lowshi.com/blog)，[回到顶部](#)

<div class="divider"></div>

## 尾注
```md
这里有一段文字，其中有一个注释引用标记[^2]，这是另一个[^xyz]，又一个[^1]，
其对应的注释文本将在文档末尾列出，常用于标注参考文献引文出处等。

[^1]: 文档末尾的注释文本。
```
这里有一段文字，其中有一个注释引用标记[^2]，这是另一个[^xyz]，又一个[^1]，其对应的注释文本将在文档末尾列出，常用于标注参考文献引文出处等。

<div class="divider"></div>

## 引用
```md
> 写作是为了更好的思考。如果一件事情你不能讲清楚，十有八九你还没有完全理解。
> <div align="right">————刘未鹏</div>
```
> 写作是为了更好的思考。如果一件事情你不能讲清楚，十有八九你还没有完全理解。
> <div align="right">————刘未鹏</div>

**NOTE:** 本博客不支持嵌套引用。为了实现文本居右我容易吗😂

<div class="divider"></div>

## 列表
```md
1. 有序列表1
2. 有序列表2
   1. 嵌套1
   2. 嵌套2
      - 继续嵌套
3. 有序列表3
   - 你可以用*
   - 或者用-
   - 也可以用+
     - 继续嵌套
```
1. 有序列表1
2. 有序列表2
   1. 嵌套1
   2. 嵌套2
      - 继续嵌套
3. 有序列表3
   - 你可以用*
   - 或者用-
   - 也可以用+
     - 继续嵌套

<div class="divider"></div>

## 代码
本博客采用的代码高亮库是纯 Ruby 实现的 [rouge](https://github.com/jneen/rouge)。
```
```javascript
// JavaScript template using Windows Script Host
var WSHShell = WScript.CreateObject("WScript.Shell");
WSHShell.Popup( "Hello World!" );
\```
```
```javascript
// JavaScript template using Windows Script Host
var WSHShell = WScript.CreateObject("WScript.Shell");
WSHShell.Popup( "Hello World!" );
```

```python
def HelloWorld():
	print "Hello World!"

if __name__=="__main__":
    HelloWorld()
```

<div class="divider"></div>

## 公式
```md
kramdown 支持 [MathJax](https://www.mathjax.org/)，行内公式如 $$ax^2 + bx + c = 0$$ ，以及更复杂的公式块如 $$\eqref{eq:1}$$ 所示：
$$
\begin{align}
\nabla \times \vec{\mathbf{B}} -\, \frac1c\, \frac{\partial\vec{\mathbf{E}}}{\partial t}  &= \frac{4\pi}{c}\vec{\mathbf{j}} \\   
\nabla \cdot \vec{\mathbf{E}} &= 4 \pi \rho \tag{1} \label{eq:1}\\
\nabla \times \vec{\mathbf{E}}\, +\, \frac1c\, \frac{\partial\vec{\mathbf{B}}}{\partial t}  &= \vec{\mathbf{0}} \\
\nabla \cdot \vec{\mathbf{B}}  &= 0\\
\end{align}
$$
数学公式 $$\eqref{eq:2}$$：
$$ \Phi=\frac{a_{n-1}}{a_n}=\frac{\sqrt{5}-1}{2}=0.6180339887 \tag{2}\label{eq:2} $$
化学方程式 $$\eqref{eq:3}$$：
$$
2H_2+O_2 \Rightarrow 2H_2O \\
(NH_4)_2SO_4+Ba(OH)_2 \Rightarrow BaSO_4 \downarrow +2NH_3\uparrow +2H_2O \\
2HgO \stackrel{\Delta}{\Leftrightarrow} 2Hg + O^2 \uparrow \tag{3} \label{eq:3}\\
2H^+ + CO_2^{-3} \Rightarrow H_2O + CO_2 \uparrow
$$
```
kramdown 支持 [MathJax](https://www.mathjax.org/)，行内公式如 $$ax^2 + bx + c = 0$$ ，以及更复杂的公式块如 $$\eqref{eq:1}$$ 所示：
$$
\begin{align}
\nabla \times \vec{\mathbf{B}} -\, \frac1c\, \frac{\partial\vec{\mathbf{E}}}{\partial t}  &= \frac{4\pi}{c}\vec{\mathbf{j}} \\   
\nabla \cdot \vec{\mathbf{E}} &= 4 \pi \rho \tag{1} \label{eq:1}\\
\nabla \times \vec{\mathbf{E}}\, +\, \frac1c\, \frac{\partial\vec{\mathbf{B}}}{\partial t}  &= \vec{\mathbf{0}} \\
\nabla \cdot \vec{\mathbf{B}}  &= 0\\
\end{align}
$$
数学公式 $$\eqref{eq:2}$$：

$$ \Phi=\frac{a_{n-1}}{a_n}=\frac{\sqrt{5}-1}{2}=0.618 \tag{2}\label{eq:2} $$

化学方程式 $$\eqref{eq:3}$$：

$$
2H_2+O_2 \Rightarrow 2H_2O \\
(NH_4)_2SO_4+Ba(OH)_2 \Rightarrow \\
BaSO_4 \downarrow +2NH_3\uparrow +2H_2O \\
2HgO \stackrel{\Delta}{\Leftrightarrow} 2Hg + O^2 \uparrow \tag{3} \label{eq:3}\\
2H^+ + CO_2^{-3} \Rightarrow H_2O + CO_2 \uparrow
$$

<div class="divider"></div>

## 表格

### Table 1: 对齐排版
```md
| No. |  列A   | 列B  |
| --- |:------:| ----:|
|  1  |  居中  | 居右 |
|  2  |   x    |  y   |
|  3  |   z    |  e   |
```

| No. |  列A   | 列B  |
| --- |:------:| ----:|
|  1  |  居中  | 居右 |
|  2  |   x    |  y   |
|  3  |   z    |  e   |

### Table 2: 更少的符号
```md
col.1 | col.2 | col.3
--- | --- | ---
*斜体* | `高亮` | **加粗**
123 | 666 | 888
```

col.1 | col.2 | col.3
--- | --- | ---
*斜体* | `高亮` | **加粗**
123 | 666 | 888

<div class="divider"></div>

## 分割线

以下三种方式均可划出分割线:

* `___`: 3个下划线
* `---`: 3个连字符
* `***`: 3个星号

如下所示：

___

一般我更喜欢用`<div class="divider"></div>`,样式更好看。

<div class="divider"></div>

## 多媒体

### 图片
```md
![img](/blog/assets/img/2018/041900.png)
```
![img](/blog/assets/img/2018/041900.png)

### 音乐
以网易云音乐为例：
```html
<iframe frameborder="no" border="0" marginwidth="0" 
marginheight="0" width="330" height="86" 
src="//music.163.com/outchain/player?type=2&id=456869610&
auto=1&height=66"></iframe>
```
<iframe frameborder="no" border="0" marginwidth="0" marginheight="0" width="330" height="86" src="//music.163.com/outchain/player?type=2&id=456869610&auto=1&height=66"></iframe>

### 视频
以优酷为例：
```html
<iframe width="560" height="315" 
src="http://player.youku.com/embed/XMzI0ODU0NTc5Ng==" 
frameborder="0" allowfullscreen></iframe>
```
<iframe width="560" height="315" 
src="http://player.youku.com/embed/XMzI0ODU0NTc5Ng==" 
frameborder="0" allowfullscreen></iframe>

## 新增功能

### Header ID
```md
## Header1 {id1}
### Header2 {#id2}

[Go2H1](#id1),[Go2H2](#id2)
```
回到[目录](#id2)

### Abbreviations 缩略语
```md
*[HTML]: Hyper Text Markup Language
```
HTML

*[HTML]: Hyper Text Markup Language

### 注释
```md
{::comment}注释1{:/comment}
{::comment}注释2{:/}
<!--当然也是可以的-->
```

{::comment}注释1{:/comment}
{::comment}注释2{:/}
<!--当然也是可以的-->

## 不支持

- ==不支持==  
- ++不支持++  
- **emoji** 表情 :smile: 但是可以直接输入 Unicode emoji 表情😄

<div class="divider"></div>

## Reference

[^1]: 尾注一，可见数字不重要，标记不重要，唯一起作用的是顺序。
[^2]: 尾注二
[^xyz]: 尾注三