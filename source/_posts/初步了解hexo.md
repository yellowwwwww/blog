---
title: 初步了解hexo,及部署到github
---
最近想使用下博客记录下自己遇到的问题，及新学的知识点。同时梳理下自己的知识体系。然后这个博客就建立起来了

## 什么是Hexo?
hexo是一款博客框架，能够快速建立起一个博客。
## 安装
我使用的是全局安装
``` bash
npm i hexo -g
```
## 初始化

``` bash
Hexo init
```
## 装依赖
``` bash
 npm install
```
## 本地运行
``` bash
 npm run server
```
这样一个基本的博客就就跑起来了。可以在_confgi.yml设置自己的博客title，自定义菜单等等。

## 部署到github
首先在github创建一个仓库，本地将项目build一下，会出现一个public的文件夹，这样可以使用git上传到github，然后点击github的setting，下拉到github pages栏目，在sources下点击save按钮，就差不多完成了。然后刷新页面，再次下拉到github pages 栏目 会出现一个链接，这个就是你的博客链接。






