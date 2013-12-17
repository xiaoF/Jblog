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


###多说评论###

请申请多说评论，用通用代码替换js/main.js中多说字段

###百度统计###

请百度统计，用通用代码替换js/main.js中百度字段

未完待续...
