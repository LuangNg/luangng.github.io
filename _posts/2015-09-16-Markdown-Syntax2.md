##Introduction
###What is markdown?

##Get Start

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





