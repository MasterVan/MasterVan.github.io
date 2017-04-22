---
title: Hexo个人博客搭建教程
tags: [Hexo]
categories: [系统与环境搭建]
date: 2017-04-21 23:26:13
---

# 依赖包安装#
## 1. git安装##
在ubuntu系统下，直接在命令行输入
```
sudo apt-get install git-core
```

## 2. node.js安装##

直接从官网下载的预编译安装包，解压后需要设置全局变量，按着网上教程，最后在安装完Hexo后，系统找不到Hexo命令
推荐使用Hexo官网的方法来，首先安装nvm

cURL:
```
$ curl https://raw.githubusercontent.com/creationix/nvm/master/install.sh | sh
```
Wget:
```
$ wget -qO- https://raw.githubusercontent.com/creationix/nvm/master/install.sh | sh
```
然后用nvm安装
```
$ nvm install stable
```
## 3. Hexo安装## 
利用npm安装
```
$ npm install -g hexo-cli
```

# 初始化设置#
cd到博客安装的文件夹，执行
```
hexo init
npm install
```
可以看到博客初始化完成了，接着可以新建博客了，在博客根目录下执行
```
hexo new “My First Blog”
```
此时在 blog/source/_post/ 文件夹下生成了My First Blog.md文件，以后写博文都是在文件里进行的，然后执行
```
hexo generate
hexo server
```
在浏览器打开 localhost://4000 可查看博客页面
如果需要重新发布，按顺序执行
```
hexo clean
hexo g
hexo s
```
初步搭建就完成了，下一步可进行个性化设置，比如主题更改和链接到Github



