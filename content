title:通过Github Page搭建个人Blog
date:2014-02-08
***
**_WARMING:本文将介绍介绍如何使用Mac在Github Page上搭建个人Blog_**
***


通过一个晚上的的努力和折腾，终于把Gihub Page的个人Blog搭建好了。所以有了这第一篇Blog。
至于为什么在Github Page上搭建Blog的原因：


##准备阶段

* ###Github账号
因为要在Github Page上搭建Blog，所以你需要一个[Github](https://github.com)账号。

* ###Github Page
在[Github Page](http://pages.github.com/)上创建自己的主页，这时候会生成一个`your_git_hub_account/your_git_hub_account.github.io`的代码库和`username.github.io`的主页（可能需要等几分钟）。

* ###Ruby
因为以下所需要的一些工具是由[Ruby](https://www.ruby-lang.org/)写的，所以需要安装Ruby。由于本人使用自带Ruby的Mac系统，所以就没有经历这步。

* ###pelican
[pelican](http://blog.getpelican.com/)是一个静态网站生成工具，无需数据库以及服务器逻辑，所以拿来做Blog挺合适的。
通过`sudo easy-install pelican`进行安装。

* ###Markdown
Markdown是一种轻量级标记语言，我们就是用它来写Blog。你可能需要一个Markdown编辑器，Mac系统推荐使用[Mou](http://mouapp.com/)。通过`sudo easy-install markdown`进行安装。
用了两天，觉得还可以，能够马上看到效果。就是不知道有没有插件什么的。
![UI](https://photos-4.dropbox.com/t/0/AABNIVo8TjnJG42Lo9meBC_up4hDaJnIlCPxkfaIi9Zx2Q/12/228786831/png/1024x768/3/1393606800/0/2/mou.png/_R75xGqRvuGEPyn-zF1y20B892LPf0sqvO6D650cJk4)
***
##搭建Blog

###pelican-quickstart
首先创建一个pelican的工作目录文件夹`mkdir ~/Documents/MyBlog; cd ~/Documents/MyBlog`（这里一定不能用中文）。再通过`pelican-quickstart`创建pelican工作目录，这里会有一系列初始配置项需要设置，我的配置是这样的。

```
Where do you want to create your new web site? [.]
What will be the title of this web site? Your site title
Who will be the author of this web site? Your name
What will be the default language of this web site? [en] 
Do you want to specify a URL prefix? e.g., http://example.com   (Y/n) n
Do you want to enable article pagination? (Y/n) 
How many articles per page do you want? [10] 
Do you want to generate a Fabfile/Makefile to automate generation and publishing? (Y/n) 
Do you want an auto-reload & simpleHTTP script to assist with theme and site development? (Y/n) 
Do you want to upload your website using FTP? (y/N) 
Do you want to upload your website using SSH? (y/N) 
Do you want to upload your website using Dropbox? (y/N) 
Do you want to upload your website using S3? (y/N) 
Do you want to upload your website using Rackspace Cloud Files? (y/N)
```
这时改目录下按照你的配置创建出pelican的工作目录，介绍几个基本的文件

```
pelicanconf.py——用于生成html的配置文件，包含输出文件夹、主题等
publishconf.py——用于发布的配置文件
Makefile——make工具的执行脚本
content——存放你写的Blog用的
output——默认生成静态html的输出文件夹
```

###码字
使用Markdown编辑器写你第一篇Blog，并保存在content中。

###生成静态html
在终端`cd ~/Documents/MyBlog; make html`，这样pelican就会生成你Blog的静态html。

###本地测试效果
在终端`make serve`，然后通过浏览器访问`http://localhost:8000/`就可以看到效果了。

###clone你Blog的默认源码
在终端`cd ~/Documents/MyBlog; git clone git@github.com:your_git_hub_account/your_git_hub_account.github.io`， clone下你的Github Page默认源码。

###发布你的主页
将output文件夹的内容替换掉你clone下的默认源码`git commit -a -m 'upload blog html'; git push origin master`，这样你的Blog就已经上传到Github Page上了。通过`http://your_git_hub_account.github.io/`就可以访问了。

至此大功告成，打完收工。
***
##更多
当然上面发布的页面是十分丑陋的。你还可以添加主题、评论、社交账号什么的。这些设置也十分简单，可以自行搜索设置。
***
##引用
本人搭建过程中参考了许多其他人的教程，在此引用致谢。
http://www.lizherui.com/pages/2013/08/17/build_blog.html 
https://gist.github.com/josefjezek/6053301 
http://zonca.github.io/2013/09/automatically-build-pelican-and-publish-to-github-pages.html 
http://martinbrochhaus.com/pelican2.html  
http://ntanjerome.org/blog/how-to-setup-github-user-page-with-pelican 




