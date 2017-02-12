# Markdown 编辑器语法指南
## 标题 / 粗斜体
### 文章内容较多时，可以用标题分段：

## 大标题 ##
### 小标题 ###
粗体 / 斜体

*斜体文本*    _斜体文本_
**粗体文本**    __粗体文本__
***粗斜体文本***    ___粗斜体文本___

## 代码
如果你只想高亮语句中的某个函数名或关键字，可以使用 `function_name()` 实现

通常我们会根据您的代码片段适配合适的高亮方法，但你也可以用 ``` 包裹一段代码，并指定一种语言

```javascript
$(document).ready(function () {
    alert('hello world');
});
```
支持的语言：actionscript, apache, bash, clojure, cmake, coffeescript, cpp, cs, css, d, delphi, django, erlang, go, haskell, html, http, ini, java, javascript, json, lisp, lua, markdown, matlab, nginx, objectivec, perl, php, python, r, ruby, scala, smalltalk, sql, tex, vbscript, xml

您也可以使用 4 空格缩进，再贴上代码，实现相同的的效果

    def g(x):
        yield from range(x, 0, -1)
        yield from range(x)

## 链接
常用链接方法

文字链接 [链接名称](http://链接网址)
网址链接 <http://链接网址>
高级链接技巧

这个链接用 1 作为网址变量 [Google][1].
这个链接用 yahoo 作为网址变量 [Yahoo!][yahoo].
然后在文档的结尾为变量赋值（网址）

  [1]: http://www.google.com/
  [yahoo]: http://www.yahoo.com/
  
  ## 图片
  跟链接的方法区别在于前面加了个感叹号 !，这样是不是觉得好记多了呢？

![图片名称](http://图片网址)
当然，你也可以像网址那样对图片网址使用变量

这个链接用 1 作为网址变量 [Google][1].
然后在文档的结尾位变量赋值（网址）

  [1]: http://www.google.com/logo.png
  
  ## 换行 / 分隔符
  如果另起一行，只需在当前行结尾加 2 个空格

在当前行的结尾加 2 个空格  
这行就会新起一行
如果是要起一个新段落，只需要空出一行即可。

如果你有写分割线的习惯，可以新起一行输入三个减号 -：

---

## 列表 / 引用
普通列表

- 列表文本前使用 [减号+空格]
+ 列表文本前使用 [加号+空格]
* 列表文本前使用 [星号+空格]
带数字的列表

1. 列表前使用 [数字+空格]
2. 我们会自动帮你添加数字
7. 不用担心数字不对，显示的时候我们会自动把这行的 7 纠正为 3
引用

> 引用文本前使用 [大于号+空格]
> 折行可以不加，新起一行都要加上哦

## 符号转义
如果你的描述中需要用到 markdown 的符号，比如 _ # * 等，但又不想它被转义，这时候可以在这些符号前加反斜杠，如 \_ \# \* 进行避免。

\_不想这里的文本变斜体\_
\*\*不想这里的文本被加粗\*\*
