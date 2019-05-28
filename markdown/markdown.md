# 段落和换行
    一个以上的空行或<br/>

# 标题
> This is an H1
> ===
> This is an H2
> ---

> # 这是 H1
> ## 这是 H2
> ###### 这是 H6

> # 这是 H1 #
> ## 这是 H2 ##
> ### 这是 H3 ######

# 区块引用
> This is a blockquote with two paragraphs. Lorem ipsum dolor sit amet,
> consectetuer adipiscing elit. Aliquam hendrerit mi posuere lectus.
> Vestibulum enim wisi, viverra nec, fringilla in, laoreet vitae, risus.
> 
> Donec sit amet nisl. Aliquam semper ipsum sit amet velit. Suspendisse
> id sem consectetuer libero luctus adipiscing.

> This is a blockquote with two paragraphs. Lorem ipsum dolor sit amet,
consectetuer adipiscing elit. Aliquam hendrerit mi posuere lectus.
Vestibulum enim wisi, viverra nec, fringilla in, laoreet vitae, risus.

> Donec sit amet nisl. Aliquam semper ipsum sit amet velit. Suspendisse
id sem consectetuer libero luctus adipiscing.

 This is the first level of quoting.
>
> > This is nested blockquote.
>
> Back to the first level.

> # 这是一个标题。
> 
> 1.   这是第一行列表项。
> 2.   这是第二行列表项。
> 
> 给出一些例子代码：
> 
>     return shell_exec("echo $input | $markdown_script");

# 列表
*   Red
*   Green
*   Blue
+   Red
+   Green
+   Blue
-   Red
-   Green
-   Blue
1.  Bird
2.  McHale
3.  Parish

# 代码区块
这是一个普通段落：

    这是一个代码区块。

# 分隔线
>* * *
>***
>*****
>- - -
>-------------------------------------

# 链接
This is [an example](http://example.com/ "Title") inline link.

[This link](http://example.net/) has no title attribute.

See my [About](/docker01.md) page for details.

[id]: http://example.com/  "Optional Title Here"

This is [an example][id] reference-style link.

# 强调
*single asterisks*

_single underscores_

**double asterisks**

__double underscores__

# 代码
Use the `printf()` function.

``There is a literal backtick (`) here.``

A single backtick in a code span: `` ` ``

A backtick-delimited string in a code span: `` `foo` ``

Please don't use any `<blink>` tags.

`&#8212;` is the decimal-encoded equivalent of `&mdash;`.

# 图片
![提示](./markdown.jpg)

![提示](./markdown.jpg "Optional title")

# 反斜杠
\*literal asterisks\*

Markdown 支持以下这些符号前面加上反斜杠来帮助插入普通的符号：

    \   反斜线
    `   反引号
    *   星号
    _   底线
    {}  花括号
    []  方括号
    ()  括弧
    #   井字号
    +   加号
    -   减号
    .   英文句点
    !   惊叹号


# 自动链接
* <http://example.com/>
* <address@example.com>
