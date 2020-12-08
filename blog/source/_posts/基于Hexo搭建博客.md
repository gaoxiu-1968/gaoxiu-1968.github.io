---
title: 基于Hexo搭建博客
date: 2020-12-08 20:45:02
tags: 博客
categories: 成果
cover: https://imgedu.lagou.com/2024393-20200511143556231-530215527.png
---
# 博客搭建

> 框架: hexo 
>
> 主题: butterfly
>
> 服务器: githubPage
>
> 域名: blog.zhangmingke.top



## HEXO

> 前提: 
>
> node.js
>
> git



### 安装hexo

全局安装:

```bash
npm install -g hexo-cli
```

### 指令

#### init

> 新建网站,一般一个网站只是用一次

```bash
hexo init [folder(文件夹路径,没有指定这个该参数,默认在当前文件夹下)]


├── _config.yml 网站的配置信息
├── package.json 应用程序信息
├── scaffolds 模板文件夹
├── source
|   ├── _drafts 草稿文章目录
|   └── _posts 发布文章目录
└── themes 主题
```

#### new

> 新建文章

```bash
hexo new [layout]<title>
# 不指定layout默认是用_config.yml指定的defaultlayout,一般是post
# 默认有三个布局,post,page,draft
# 我只需要post
```

#### generate

> 生成静态文件

```bash
hexo generate
可以省略为 hexo g
也可以添加参数,在生成静态文件的同时部署项目,比如 hexo g -d
```

#### publish

> 发表草稿

```bash
hexo publish <filename>
```

#### deploy

> 部署项目

```bash
hexo deploy
可以省略为hexo d
```

#### clean

```bash
hexo clean
清除缓存文件 (db.json) 和已生成的静态文件 (public)。
在某些情况（尤其是更换主题后），如果发现您对站点的更改无论如何也不生效，您可能需要运行该命令
```

#### server

```bash
hexo server
本地启动服务,可以查看具体的样子
```



## 主题

> hexo 所有主题都要遵守hexo主题结构要求
>
> 所以配置信息的所在位置是相通的!

### butterfly主题

#### 安装

> butterfly提供两种安装方法:
>
> ​	通过下载主题文件到theme文件下
>
> ​	npm安装,可以到node_modules\hexo-theme-butterfly修改文件进行魔改

具体安装可以参照butterfly官网安装教程

```
https://butterfly.js.org/posts/21cfbf15/#%E5%AE%89%E8%A3%9D
```

#### 文章封面

```
cover: 图片地址(在编写markdown页面的时候使用)
```

