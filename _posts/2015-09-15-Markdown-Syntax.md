##Introduction
###What is markdown?

Markdown is a lightweight markup language with plain text formatting syntax designed so that it can be converted to HTML and many other formats using a tool by the same name.Markdown is often used to format readme files, for writing messages in online discussion forums, and to create rich text using a plain text editor.

###Purpose

*"Easy read and write."*

可读性，无论如何，都是最重要的。一份使用 Markdown 格式撰写的文件应该可以直接以纯文本发布，并且看起来不会像是由许多标签或是格式指令所构成。Markdown 语法受到一些既有 text-to-HTML 格式的影响，包括 Setext、atx、Textile、reStructuredText、Grutatext 和 EtText，而最大灵感来源其实是纯文本电子邮件的格式。

总之， Markdown 的语法全由一些符号所组成，这些符号经过精挑细选，其作用一目了然。比如：在文字两旁加上星号，看起来就像*强调*。Markdown 的列表看起来，嗯，就是列表。Markdown 的区块引用看起来就真的像是引用一段文字，就像你曾在电子邮件中见过的那样。

**兼容 HTML**

Markdown 语法的目标是：成为一种适用于网络的书写语言。

Markdown 不是想要取代 HTML，甚至也没有要和它相近，它的语法种类很少，只对应 HTML 标记的一小部分。Markdown 的构想不是要使得 HTML 文档更容易书写。在我看来， HTML 已经很容易写了。Markdown 的理念是，能让文档更容易读、写和随意改。HTML 是一种发布的格式，Markdown 是一种书写的格式。就这样，Markdown 的格式语法只涵盖纯文本可以涵盖的范围。

不在 Markdown 涵盖范围之内的标签，都可以直接在文档里面用 HTML 撰写。不需要额外标注这是 HTML 或是 Markdown；只要直接加标签就可以了。

要制约的只有一些 HTML 区块元素――比如 &lt;div&gt;、&lt;table&gt;、&lt;pre&gt;、&lt;p&gt; 等标签，必须在前后加上空行与其它内容区隔开，还要求它们的开始标签与结尾标签不能用制表符或空格来缩进。Markdown 的生成器有足够智能，不会在 HTML 区块标签外加上不必要的 &lt;p&gt; 标签。

##Getting started

###Syntax

####Blockquotes
Put ">" before every line.

>This is a blockquote

####Lists
Markdown supports ordered(numbered) and unordered(bulleted) lists.Like this:
For unordered lists, you just start with \*, \- or \+ and put a blankspace right behind it.
+ Red
+ Green
+ Blue

For ordered lists, pls start with a number and a dot and a blankspace.

1. Bird
2. McHale
3. Parish

####Code Blocks
Markdown requires wrapping a code block in both &lt;pre&gt;and&lt;code&gt;tags.To produce a code in markdown doc, you should simply indent every line of the block at least 4 spaces or 1 tab.Like below:

This is a normal paragraph

    This is a code block

Markdown parser will generate HTML code like this:
&lt;p&gt;This is a normal paragraph :&lt;/p&gt;
&lt;pre&gt;
    &lt;code&gt;This is a code block .&lt;/code&gt;
&lt;/pre&gt;

A code block continues until it reaches a line that is not intended(or the end of the article).

Within a code block(which is intended), all the HTML tags will be converted into HTML entities.However, regular markdown syntax is not processed within code blocks.This means it's easy to use markdown to write about Markdown's own syntax.

However, it's better to surounded by "```[type of lang]".Like this:

```javascript
    function(){
        do sth...
    }
```

####Horizontal Rules
In MD files, you can produce a horizontal rule tag(&lt;bt /&gt;) by placing three or more "*", "-"(recommended) or "_".

---

####Span Elements
Markdown just supports two style of links: inline and reference.
The link text is delimited by [square brackets].Use a set of regular parentheses immediately to create an inline link after the link text.And the "title" is optional. eg.

This is an [example](http://example.com/ "Title") inline link.

Reference-style links use a second set of square brackets, inside which you place a label of your choosing to identify the link:

This is an [example][id] reference - style link.

Then, anywhere in the document, you define your link label like this, on a line by itself:
[id]:http://example.com/ "Optional Title Here"

####Emphasis
Markdown treats asterisks(*) and underscores(_) as indicators of emphasis.Text wrapped with one * or _ will be wrapped with HTMl &lt;em&gt; tag; double * or _ will be wrapped with an HTML&lt;Strong&gt;

*single asterisks* _single asterisks_

**double underscores** __double underscores__

If you want to use charactor "*", suround with spaces would be handle it.Backslash escape it is recommended. 

####Code
To indicate a span of code, wrap it with backtick quotes(').HTML tags will be treat as character strings. Check below:

Use the `printf()` function.

####Image
![baidu logo](https://www.baidu.com/img/baidu_jgylogo3.gif "baidu")

####Table
| Left align | Right align | Center align |
|:-----------|------------:|:------------:|
| This       |        This |     This     |     
| column     |      column |    column    |
| will       |        will |     will     |
| be         |          be |      be      |
| left       |       right |    center    |
| aligned    |     aligned |   aligned    |

####Miscellaneous
#####Automatic Links
Simply surround the URL or email address with angle brackets(&lt;&gt;). Like this:

<http://luangng.github.io/>

#####Backslash Escapes
You'd better to backclash escape any charactor you want to use. 
