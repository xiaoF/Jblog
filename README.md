Just Blog
----------
jekyll 静态博客模板

####系统设置####

代码高亮

    pygments: true

每页显示数目

    paginate: 5

    relative_permalinks: false

生成的文件夹格式

    permalink: /:year/:month/:day/:title/

如博文太长在markdown 文档加入以下字符便可控制列表概述显示内容

    excerpt_separator: <!--more--> 

分页

    paginate_path: "page:num"

CNAME文件

设置二级域名或顶级域名



单篇博文模板
----------
####注意":" 后面紧跟着一个空格####

####以下模版头属性必填可扩展####


    ---
    layout: blogs_item
    title: "标题"
    author: 作者
    categories: 分类
    day: 日
    month: 月
    year: 年
    ---
    
    正文第一段（并且在博文列表显示概要）
    
    <!--more--> 
    
    正文第二段（只在详细中可见，概要不可见）

## 文章文件夹

所有的文章都在`_posts`文件夹中。
这些文件可以用[Markdown](http://daringfireball.net/projects/markdown/) 编写，
也可以用[Textile](http://textile.sitemonks.com/) 格式编写。只要文件中有
[YAML头信息](../frontmatter/)，它们就会从源格式转化成 HTML 页面，从而成为
你的静态网站的一部分。

### 创建文章的文件

发表一篇新文章，你所需要做的就是在`_posts`文件夹中创建一个新的文件。
文件名的命名非常重要。Jekyll 要求一篇文章的文件名遵循下面的格式：
`
年-月-日-标题.MARKUP
`
在这里，`年`是4位数字，`月`和`日`都是2位数字。`MARKUP`扩展名代表了这篇文章
是用什么格式写的。下面是一些合法的文件名的例子：
`
2011-12-31-new-years-eve-is-awesome.md
`



### 内容格式

所有博客文章顶部必须有一段[YAML头信息](../frontmatter/)(YAML front- matter)。
在它下面，就可以选择你喜欢的格式来写文章。Jekyll支持2种流行的标记语言格式：
[Markdown](http://daringfireball.net/projects/markdown/) 和
[Textile](http://textile.sitemonks.com/). 这些格式都有自己的方式来标记文章中不
同类型的内容，所以你首先需要熟悉这些格式并选择一种最符合你需求的。

## 引用图片和其它资源

很多时候，你需要在文章中引用图片、下载或其它数字资源。尽管 Markdown 和 Textile
在链接这些资源时的语法并不一样，但你只需要关心在站点的哪些地方保存这些文件。

由于 Jekyll 的灵活性，有很多方式可以解决这个问题。一种常用做法是在工程的根目录下
创建一个文件夹，命名为`assets` 或者 `downloads`，将图片文件，下载文件或者其它的
资源放到这个文件夹下。然后在任何一篇文章中，它们都可以用站点的根目录来进行引用。
这和你站点的域名/二级域名和目录的设置相关，下面有一些例子（Markdown格式）
来演示怎样利用`site.url`变量来解决这个问题。

在文章中引用一个图片

`
… 从下面的截图可以看到：
![有帮助的截图]({{ site.url }}/assets/screenshot.jpg)
`

链接一个读者可下载的 PDF 文件：

`
… 你可以直接 [下载 PDF]({{ site.url }}/assets/mydoc.pdf).
`

<div class="note">
  <h5>提示™: 链接只使用站点的根URL</h5>
  <p>
    如果你<strong>确信</strong>你的站点只在域名的根 URL 下做展示，你可以不使用
     <code>{{ site.url }}</code>变量。在这种情况下，
     直接使用<code>/path/file.jpg</code>即可。
  </p>
</div>


###多说评论###

请申请多说评论，用通用代码替换js/main.js中多说字段

###百度统计###

请百度统计，用通用代码替换js/main.js中百度字段

未完待续...
