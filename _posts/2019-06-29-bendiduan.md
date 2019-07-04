---
layout: page
title: "线上修改易错又易乱？简单学会本地端修改"
categories:
  - 网站设计
---

### 从线上到本地端

- Jekyll网站结构严谨，修改时需要小心谨慎，且相较于只需要一个CSS文件、一个img文件及一个index.html文档构成的静态页面所需要的文件数要更多且复杂。我们在gitee及github网站上进行修改时，在完成每一个文件保存时都必须要提交一次commit，但对于复杂的Jekyll网站而言，很多时候仅仅修改一处并不能达到我们想要的效果，又或是不小心修改错误，这在线上就很难撤回了。
- 这个时候，在本地端修改就能其重要的作用了。以下是如何把线上转移到线下的参考过程。

1.首先，我们需要下载[Github Desktop](https://desktop.github.com/)和[HBuilder](http://www.dcloud.io/hbuilderx.html)并打开。

![Github Desktop](https://assets.gitee.com/jiayichen/jiayichen/raw/5295a5f7abf4cb194eda49ec243a510431a679d3/assets/images/Github%20Desktop-url.png)

![HBuilder](https://assets.gitee.com/jiayichen/jiayichen/raw/5295a5f7abf4cb194eda49ec243a510431a679d3/assets/images/HBuilder-url.png)


2.然后，我们回到我们的gitee项目仓库中，复制url。

![复制gitee链接](https://assets.gitee.com/jiayichen/jiayichen/raw/5295a5f7abf4cb194eda49ec243a510431a679d3/assets/images/gitee-url.png)

3. 打开下载安装好的Github Desktop，点击File下的Clone a repository。

![Clone a repository](https://assets.gitee.com/jiayichen/jiayichen/raw/5295a5f7abf4cb194eda49ec243a510431a679d3/assets/images/Clone%20a%20repository-anniu.png)

4. 打开后点击URL，在上面的输入框（URL or usermane/repository）贴上刚刚在仓库复制的url,在下面的输入框(Local path)选择保存项目的本地地址。

![URL输入](https://assets.gitee.com/jiayichen/jiayichen/raw/5295a5f7abf4cb194eda49ec243a510431a679d3/assets/images/URL-input.png)

5. 等待下载完成后，我们可以在下图处选择我们要进行的分支。

![修改分支](https://assets.gitee.com/jiayichen/jiayichen/raw/5295a5f7abf4cb194eda49ec243a510431a679d3/assets/images/xiugaifenzhi.png)

6. 然后我们打开HBuilder，点击文件导入，从本地问目录导入，找到刚刚下载的项目文件，就可以把整个项目加载到HBuilder左边栏啦，接下来我们就可以对其进行修改啦。

![导入文件](https://assets.gitee.com/jiayichen/jiayichen/raw/5295a5f7abf4cb194eda49ec243a510431a679d3/assets/images/daoruwenjian.png)

![选择文件](https://assets.gitee.com/jiayichen/jiayichen/raw/5295a5f7abf4cb194eda49ec243a510431a679d3/assets/images/Choice.png)

![成功添加](https://assets.gitee.com/jiayichen/jiayichen/raw/5295a5f7abf4cb194eda49ec243a510431a679d3/assets/images/chenggongtianjia.png)

7. 在HBuilder修改完成后保存，返回Github Desktop，我们能选择我们一个或多个修改进行commit提交。

![选择commit](https://gitee.com/jiayichen/jiayichen/raw/5295a5f7abf4cb194eda49ec243a510431a679d3/assets/images/Choice-commit.png)

8. 最后把commit提交到gitee上（可同时提交多个），便完成修改啦。

![Push](https://gitee.com/jiayichen/jiayichen/raw/gh-pages/assets/images/Push.png)


