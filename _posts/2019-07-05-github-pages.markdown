---
layout: post
title:  "Build your own Blog"
categories: Github-Pages
tags: Github-Pages
---

* content
{:toc}

Github Pages搭建简要说明





## Github+Jekyll搭建静态博客

### 1.网站托管

#### 	1）注册Github账号

#### 	2）新建仓库

​		仓库名称格式为：用户名.github.io(<u>用户名必须为Github账号名</u>)，<u>仓库类型必须是Public</u>(虽然

​		Private已经免费)，选上Initialize this respository with a README，下面两项默认None。

​		进入**[Settings]**找到**[Github Pages]**如果出现：

> ​		Your site is published at https://用户名.github.io/

​		说明仓库已创建成功，可以通过上面网址访问示例网站

### 2.搭建开发和调试网站环境

#### 	1）安装Jekyll

​		Jekyll工具可以进行本地网站开发和快速预览调试。

​		先安装Ruby，Jekyll依赖于Ruby，需要提前安装，安装过程可以参看Ruby官网，接着安装

​		RubyGems，由于安装Ruby时自带安装可省略这一步，最后安装Jekyll(终端输入`gem install `

​		`jekyll`)

​		注：由于网站用到分页功能，在 Jekyll 3 中，需要在gems中安装`jekyll-paginate` 插件(终端输入

​		命令`gem install jekyll-paginate`安装)，并添加到你的 `Gemfile`和 `_config.yml` 文件中。在 

​		Jekyll 2 中，分页是标准功能，无需添加`jekyll-paginate`插件。具体添加方式：`Gemfile`文件中

​		添加`gem "jekyll-paginate"`，`_config.yml`文件中添加`plugins: [jekyll-paginate]`和

​		`paginate: 6`

#### 2）安装Typora

​		方便编写markdown

#### 3）本地编写和调试网站

​		**获取网站主题框架**

​		为了节省开发时间，直接从Github下载别人的主题框架源码过来

​		**运行Jekyll**

​		终端输入`gem install bundler jekyll`安装bundler jekyll，再输入`jekyll new my-awesome-`

​		`site`，`my-awesome-site`是存放本地网站代码的目录，将之前下载的框架源码移动到这个目录

​		下，注意重复文件的处理，之后输入`cd my-awesome-site`到项目目录下，输入`bundle exec `

​		`jekyll serve --watch`通过浏览器输入http://127.0.0.1:4000或http://localhost:4000运行项目

​		**编写Blog内容**

​		在项目_posts目录下按规范的命名方式新建markdown文件，通过Typora编写Blog内容

#### 4）发布网站到Github

​		直接拖拽上传项目文件，或者通过Git工具		