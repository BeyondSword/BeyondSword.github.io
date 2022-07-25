---
title: MinimalMistakes主题指南
layout: single
toc: true
excerpt: "使用jekyll主题MinimalMistakes搭建博客"
tags: jekyll指南
categories: 建站
header:
  overlay_color: "#333"
---
## 概述
[官方文档](https://mmistakes.github.io/minimal-mistakes/docs/quick-start-guide/)
{: .notice--warning}

## 快速开始
### Sample
获取MinimalMistakes主题的仓库。
```
$git clone https://github.com/mmistakes/minimal-mistakes.git
```
仓库本身是一个 jekyll 仓库, 可以在本地调试运行：
```
$bundle install
$bundle exec jekyll serve
```
访问 http://127.0.0.1:4000 可以看到网站已经加载成功，可以测试各项功能。

**jekyll**: 一个用于搭建静态博客的网站生成器。<br>
**jekyll主题**: 基于 jekyll 进行快速建站的一些主题， 可以理解为基于 jekyll 的框架。
{: .notice--info}

### _config.yml
这是 jekyll 的核心配置文件，后续一系列的配置工作都在这里展开。如果你已经运行了 Sample, 可以在仓库根目录下发现该文件。

### 目录结构
略

### layout布局
从头开始进行博客页面开发效率是很低的，效果可能也不会很好。因此需要使用一些框架提供的标准模板(layout)来加快建站的速度。这里翻译成布局。布局分为了很多类型。
#### Default layout
在该主题中，default.html为根布局（一般大部分情况下也都是如此），一般被其他模板所继承。适合配置一些对所有页面生效的模块。
格式还是参考[_config.yml](https://github.com/mmistakes/minimal-mistakes/blob/master/_config.yml)。
warning: 本地调试时对[_config.yml]的改动不能实时生效，需要重启服务器。
#### single.html
最常用的布局
#### Archive layout

#### posts.html
这是主题的按时间归档模板，一般要配合导航栏使用。

#### 插件jekyll-archives
快速解决文章归档问题。

#### Home page layout
这里进行主页的布局。

#### Splash page layout

#### Search page layout
搜索页。 对中文的搜索似乎存在一些问题。

#### Headers
添加一些标题图片,增加视觉冲击力。
#### Header overlay
在标题图片覆盖文字的一些方案。

#### layout: posts
该布局将文章按时间进行归类。

#### SideBars 侧边栏
设置展示在页面左侧的一些内容。默认情况下这部分是空白的。
一些选择：
1. 作者信息
2. 自定义内容
3. 侧边导航菜单

#### 社交网络链接的分享
这部分暂时先略过，国内外环境不同。



文章右上方的索引栏，通过在front matter中加入 ```toc:true``` 即可开启


归档页面要怎么配置？
新建_pages然后在._config.yml中将其include进去。

#### 添加评论栏
1. 需要有编辑器模块
2. 需要有评论内容的增删改查


左侧要放文章导航， 右侧放导览


围绕_config.yml 展开，此为网站的核心配置文件