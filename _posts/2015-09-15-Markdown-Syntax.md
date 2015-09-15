##概述

**宗旨**

Markdown 的目标是实现「易读易写」。

 可读性，无论如何，都是最重要的。一份使用 Markdown 格式撰写的文件应该可以直接以纯文本发布，并且看起来不会像是由许多标签或是格式指令所构成。Markdown 语法受到一些既有 text-to-HTML 格式的影响，包括 Setext、atx、Textile、reStructuredText、Grutatext 和 EtText，而最大灵感来源其实是纯文本电子邮件的格式。

总之， Markdown 的语法全由一些符号所组成，这些符号经过精挑细选，其作用一目了然。比如：在文字两旁加上星号，看起来就像*强调*。Markdown 的列表看起来，嗯，就是列表。Markdown 的区块引用看起来就真的像是引用一段文字，就像你曾在电子邮件中见过的那样。

**兼容 HTML**

Markdown 语法的目标是：成为一种适用于网络的书写语言。

Markdown 不是想要取代 HTML，甚至也没有要和它相近，它的语法种类很少，只对应 HTML 标记的一小部分。Markdown 的构想不是要使得 HTML 文档更容易书写。在我看来， HTML 已经很容易写了。Markdown 的理念是，能让文档更容易读、写和随意改。HTML 是一种发布的格式，Markdown 是一种书写的格式。就这样，Markdown 的格式语法只涵盖纯文本可以涵盖的范围。

不在 Markdown 涵盖范围之内的标签，都可以直接在文档里面用 HTML 撰写。不需要额外标注这是 HTML 或是 Markdown；只要直接加标签就可以了。

要制约的只有一些 HTML 区块元素――比如 &lt;div&gt;、&lt;table&gt;、&lt;pre&gt;、&lt;p&gt; 等标签，必须在前后加上空行与其它内容区隔开，还要求它们的开始标签与结尾标签不能用制表符或空格来缩进。Markdown 的生成器有足够智能，不会在 HTML 区块标签外加上不必要的 &lt;p&gt; 标签。

#一级标题
##二级标题
###三级标题
####四级标题
#####五级标题
######六级标题

一级标题
========
二级标题
--------

**文本加粗**
*斜体*
***加粗倾斜***

---

***
___


- 无序列表项一
 - 子列表项一
 - 子列表项二
- 无序列表项二
- 无序列表项三

1. 有序列表项一
2. 有序列表项二

> 引用文字

```js
function a(){
	...
}
```
```java
class A
{
	...
}
```

超链接[baidu](https://www.baidu.com/)
图片![alt text](https://www.baidu.com/img/baidu_jgylogo3.gif?v=40661608.gif "baidu")

<table>
    <tr>
        <th>表格头1</th>
        <th>表格头2</th>
    </tr>
    <tr>
        <td>表格内容1</td>
        <td>表格内容2</td>
    </tr>
</table>


> This is a blockquote with two paragraphs. Lorem ipsum dolor sit amet,
> consectetuer adipiscing elit. Aliquam hendrerit mi posuere lectus.
> Vestibulum enim wisi, viverra nec, fringilla in, laoreet vitae, risus.
> 
> Donec sit amet nisl. Aliquam semper ipsum sit amet velit. Suspendisse
> id sem consectetuer libero luctus adipiscing.
  
> This is the first level of quoting.
>
> > This is nested blockquote.
>
> Back to the first level.


