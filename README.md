
Just Blog
----------
jekyll 静态博客模板

**系统设置**

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



未完待续...
