---
layout: post
title: 
categories: [笔记, 博客]
description:
keywords:
tags: [jekyll, github pages]
---

## 选择 Jekyll 主题

对主题的要求，至少需要以下特性：

- 右侧目录
- 全文搜索

对比了以下几个主题：

|                                        主题                                        | 目录 |                     全文搜索                     |      其他       |
| --------------------------------------------------------------------------------- | ---- | ----------------------------------------------- | --------------- |
| [mzlogin](https://github.com/mzlogin/mzlogin.github.io)                           | 支持 | 支持，实时，搜索结果仅显示标题，有时不太准确         | 功能丰富，无标签 |
| [jekyll-TeXt-theme](https://github.com/kitian616/jekyll-TeXt-theme)               | 支持 | 仅支持搜索标题，搜索结果仅显示标题                 | 功能强大         |
| [professordeng/simple](https://github.com/professordeng/simple)                   | 支持 | 支持，搜索结果仅显示标题                          | 简洁            |
| [Huxpro/huxpro.github.io](https://github.com/Huxpro/huxpro.github.io)             | 支持 | 仅支持搜索标题，实时，搜索结果仅显示标题            |                 |
| [cotes2020/jekyll-theme-chirpy](https://github.com/cotes2020/jekyll-theme-chirpy) | 支持 | 支持，实时，搜索结果能展示搜索到的文字，有时不太准确 | 功能丰富         |

目前找到的支持全文搜索的主题，在搜索中文时并不太准确，经常无法搜索出来。

主题使用记录：

- [Jekyll Theme Mzlogin 主题配置](http://1057.pub/jekyll-theme-mzlogin/posts/config-jekyll-theme-mzlogin/)
- [Jekyll Theme Chirpy 主题配置](http://1057.pub/jekyll-theme-chirpy/posts/config-jekyll-theme-chirpy/)

备选主题

- https://github.com/TMaize/tmaize-blog 简洁，全文搜索（实时且搜索结果能展示搜索到的文字），缺点：不支持目录，默认夜间模式

## Logo & Favicon & Avatar

- 从 [RealFaviconGenerator](https://realfavicongenerator.net/) 生成 Logo & Favicon
- Avatar：http://1057.pub/ghcos/images/avatar01.jpg

## 使用 VNote 管理博客文章

1. 【笔记本】-【从文件夹新建笔记本】，将该仓库作为外部文件夹纳入管理
2. 更新 `.gitignore`

```
_v_recycle_bin
vx.json
vx_notebook/
vx_recycle_bin/
```

## 图片管理

> 目前 VNote 3 已支持 GitHub 图床，后续将直接使用 VNote 的功能保存图片，不再使用 PicGo（除非需要提升访问速度，再迁移腾讯云 COS）。

### 设置 GitHub 图床

单独创建一个 GitHub 仓库 [pysense/ghcos](https://github.com/pysense/ghcos) 用于存储图片，并设置启用 GitHub Pages。

![](https://raw.githubusercontent.com/pysense/ghcos/master/blog/_posts/2021-08-01-start-blog-with-jekyll.md/543331417229582.png)

### 通过 PicGo 上传图片到 GitHub

配合 [Molunerfinn/PicGo](https://github.com/Molunerfinn/PicGo) 上传图片

![](https://raw.githubusercontent.com/pysense/ghcos/master/blog/_posts/2021-08-01-start-blog-with-jekyll.md/301712017237615.png)

### 通过 VNote 上传图片到 GitHub（当前采用此方法）

1）配置 GitHub 图床

![](https://raw.githubusercontent.com/pysense/ghcos/master/blog/_posts/2021-08-01-start-blog-with-jekyll.md/533962517226839.png)

2）在编辑器工具栏选择图床为 GitHub，之后粘贴到 VNote 的图片将自动上传到配置好的 GitHub 仓库。

## 介绍 Jekyll 的文章

- [我的Jekyll博客 \| 开放笔记](https://goooooouwa.fun/productivity/2021/03/29/blog-setup.html)

