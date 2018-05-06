---
title: "DU Weekly 怼周刊小站 项目 - 自述原案"
date: 2018-03-29T11:23:18+08:00
categories: ["Tech"]
---

**Link**

- [[RDD]DU Weekly 怼周刊小站 项目，自述原案 · Issue #365 · DebugUself/du4proto](https://github.com/DebugUself/du4proto/issues/365)


**Update - 20180413**

小站已迁移至怼圈内部, 后续进展将更新至

- 小站 - [DU Weekly 小站](https://duw.zoomquiet.io/)
- 仓库 - [Github 仓库](https://github.com/DebugUself/duw)
- Issue - [3d [ANN] DU Weekly 小站迁移至怼圈内部 , 欢迎小伙伴一起来更新 · Issue #380 · DebugUself/du4proto](https://github.com/DebugUself/du4proto/issues/380)

---

## Background

- @ZoomQuiet 发起 - [10d[RDD]为怼圈重启:完善常设项目:自述 · Issue #357](https://github.com/DebugUself/du4proto/issues/357)
- 怼周刊到现在已经累计到 50 多期了，希望能为它建立一个小站，能让我们更方便的查询和阅读，也让它后续能有更多的发展空间

## 项目 Demo


- [DU Weekly 小站](https://duw.zoomquiet.io/)
    - [Github 仓库](https://github.com/DebugUself/duw)
    
![duw1](https://user-images.githubusercontent.com/1319356/38078781-f14251ac-336f-11e8-970d-de780329bfb2.png)


- 采用的是 Hugo + Netlify + Git + Disqus
- 采用 Hugo 来生成静态网站，是觉得它比 Jekyll 更好看。
- Netlify 可以完成自动化部署和发布，无需在本地一遍遍用 Hugo 来生成静态网站，直接 push 到 GitHub 就可以实现网站的发布。
- 评论系统最后还是选了 Disqus，虽然国内常常打不开，不过一般情况下把它折叠了，也不会造页面不流畅。

## 备选方案

[DU Weekly 怼周刊 @GitBook](https://duw.zoejane.net/)

- 用 GitBook 做出的怼周刊也很清秀
- 尤其是后续维护非常简单，只要把 DUW 的原始 markdown 文件拷贝过去，只需更新 Summary 目录文件就可以啦
- 不过考虑到后续的拓展性的话，还是觉得 Hugo 生成的小站会更方便一点

## 需要的帮助

### 问题一

想把这个项目放到 DU 里来协同，无奈发现 Netlify 似乎只支持个人创建的 repo 的自动化部署， DU 组织里创建的项目识别不出来。 

### 方案尝试打算

- 试试 [Automated deployments with Wercker - Hugo中文文档](http://www.gohugo.org/doc/tutorials/automated-deployments/) 里的方式，看是不是可以绕开这个限制
- 找找 Jekyll 有没有适合这个项目的模板，这样 GitHub 自身就可以完成发布了
- 项目里 master 只放源代码，调试的时候本地调试，Hugo 自动生成的 html相关文件不上传上来，或者上传到 gh-pages 里。

### 问题二

小站还有什么需要提升的吗？或者小站还有什么更多玩法吗？
还请小伙伴们多多参与，有什么想法也都可以在 Issue 里讨论 :)

## 进展

- 180413 DU Weekly 小站 启用新域名 http://duw.zoomquiet.io
- 180412 [DU Weekly 小站](https://duw.zoejane.net/) 迁移至 [怼圈内部 repo](https://github.com/DebugUself/duw), 并启用新域名 https://duw.zoejane.net
- 180329 [DU Weekly 小站](https://duw.zoejane.net/) 上线
- 180329 在 [du.zoomquiet.io](http://du.zoomquiet.io/) 右上角添加了 怼周刊 小站链接
- 180329 测试了将 duw 的文章直接放入 [du.zoomquiet.io](http://du.zoomquiet.io/) ，显示有错位，需要进一步调整模板了才能用这种方式

## Changelog

- 180329 zoejane init

