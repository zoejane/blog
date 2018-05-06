
---
title: "Issue 创建指南"
date: 2017-04-08T11:23:18+08:00
categories: ["Tech", "Tutorial"]
---

**Link**

- [[WIKI] Issue 创建指南 反馈征集 · Issue #21 · DebugUself/du4proto](https://github.com/DebugUself/du4proto/issues/21)
- [HbUsageIssue · DebugUself/du4proto Wiki](https://github.com/DebugUself/du4proto/wiki/HbUsageIssue)

## 背景
GitHub Issue 是帮助我们进行协助的利器。与我们日常生活中更熟悉的论坛有所不同，它不仅仅只是一个供大家交流的场所，更是我们协作并推进项目进行的场所。  
那么如何更好的使用 Issue 呢？

## 步骤

- 提前规划：从作品角度出发进行思考
- 内容书写：清楚地交待清楚来龙去脉
- 任务管理：积极地对任务跟进和维护
- 任务结束：形成可复用的作品和成果

## Step 1 提前规划

Issue 发布之前，提前对 Issue 做一个初步规划。

- 你希望通过这个 Issue 达成什么任务
- 是否可以进一步的将它输出为对应的 成果/作品
- 如何方便后期能在此基础上进行 积累/复用/提升

比如

- 你提出了一个技术问题，并在大家的帮助下得到了解决，那么，是否可以写成一篇小小的教程，让以后碰到类似情况的小伙伴也能从中受益？
- 你号召大家进行了一次聚会，收获颇多，那么，是否可以放出现场的 录音/照片/视频 ，共同分享这次聚会的收获，让没有到场的小伙伴也能共同体验？
- 你在协作的过程中发现了一些不方便的地方，大家进行了热烈探讨，那么，是否可以根据讨论，逐个改进，并形成新的协作流程，彻底的改变原来的不便之处？

从作品输出复用的角度提前思考，能让你真正感受到用 Issue 进行团队协作，不断成长的快乐。  
事隔多年后，当你回想，你所记得的不仅仅是散落各处的帖子，更有凝聚力与队友一起成长的作品，传承下去，承载了你们曾共同共事的时光。

## Step 2 内容书写

### 标题

形式 - `时限`(可选) + `[关键词]` + `Issue 主题`

- 使用前缀（`时限` + `[关键词]`），方便进行快速识别  
    - 前缀类型:
        - `[ANN]` ~ 通告
        - `[ASK]` + 时限 ~ 提问
        - `[DUW]` + 时限~ 怼周刊投稿
        - `[LOG]` ~ 日志
        - `[TASK]` + 时限 ~ 任务
        - `[WIKI]` + 时限~ 文档草案
        - `[CHAOS]` ~ 其它
- 尽可能简洁的概括 Issue 主题

>如 `42h[TASK]为什么要 fork ? `

- `42h` - 所有任务都应该有合理的死线
- `[TASK]` - 关键词前缀，用来快速提示此主题属于一个任务
- `为什么要 fork ?` - 概括 Issue 的主题

以现有 Issues 举例，进行前缀的重新梳理

- [DU1wd6zoom]预约 --> `ANN` 通告
- [chk]提问自检清单 厘定 --> `WIKI` 可转为协作文档
- [DU] 竹子事件 回顾 --> 从 `LOG`（记录） 转为 `WIKI`（协作文档）
- [OT]小密圈 怼集 --> 从 `LOG`（记录） 转为 `WIKI`（协作文档）
- [DU]自怼圈是什么?以及大家如何自处  --> `WIKI` 可转为协作文档
- [投稿怼周刊]仓库故事还原追查法 --> [DUW]仓库故事还原追查法

### 正文

#### 主题

一次只说一个主题，方便后期有针对性的讨论。

#### 内容

交待清楚来龙去脉，减少来回确认信息的沟通成本，提升协作的效率。

[大妈建议](http://blog.zhgdg.org/2014-09/gdg-writer-guider/)，尽可能的包含足够的信息，比如

- 缘起 ~ 背景历史 
- 现象 ~ 问题描述 
- 尝试 ~ 自个儿探索过程/思路/关键代码... 
- 分析 ~ 将问题分析为几个关键子问题,进行逐一分析,解释 
- 解决 ~ 最终方案的具体实施过程 
- 要点 ~ 过程中,必须注意的操作,容易出错的地方 
- 总结 ~ 从整体上回顾问题/解决/思路,对同类问题进行建议 
- 参考 ~ 收集过程中各种给予自个儿有力帮助的资源/文章/代码

![](http://i2.muimg.com/567571/059763f36c34348b.png)

#### 提问

参考经典文章 

- [How To Ask Questions The Smart Way - Eric Steven Raymond](http://www.catb.org/~esr/faqs/smart-questions.html)
- [提问的智慧 - 简体中文版](https://github.com/ryanhanwu/How-To-Ask-Questions-The-Smart-Way/blob/master/README-zh_CN.md)

#### 格式

使用 Markdown 进行清晰的展示，参见 [Mastering Markdown - GitHub Guides](https://guides.github.com/features/mastering-markdown/)

## Step 3 任务管理

### 任务分配 Assignee

你可以指派专人负责这个项目的推进与落实，对任务进行维护。可以指派给自己，或者你觉得更适合的人选。  
使用 Issue 自带的 Assignee 功能，能方便的对任务进行分配。在 Issue 主题列表上，也可以清晰的看到每个任务相应的对接人。

![2bf0a02978822faa.png (1008×409)](http://i4.buimg.com/567571/2bf0a02978822faa.png)

### 分类检索 Label

标签有利于 Issue 主题的识别。后期，也可以让你非常方便的根据不同的标签筛选出相同类型的 Issue，而不用在一大堆的  Issue 中逐个去搜索。

![8eb30cdaf2456e1b.png (1004×545)](http://i1.piimg.com/567571/8eb30cdaf2456e1b.png)

比如

- `bug` 你发现的项目中存在的一些需要解决的缺陷
- `enhancement` 你对项目进行改进和提升的建议 
- `question` 提出你的疑问和困惑

### 宏观把控 Project & Milestone

Project & Milestone 有助于你对整个协作过程的宏观把控。这也需要你提前对整个项目的发展蓝图有所了解。

GitHub 中集成了 Projects 看板，你可以很方便的从整个项目的角度进行追踪，根据 Issue 的推进情况，及时维护项目的进展。在创建 Issue 的同时，你也可以为 Issue 指派对应的 Project。

![a5e4fb2f9b911f27.png (1023×664)](http://i1.piimg.com/567571/a5e4fb2f9b911f27.png)

一个项目的推进并不是一蹴而就的，常常需要制定一些阶段性目标。这时可以使用 Milestone。在这里可以直观的展示出每个 Milestone 下关闭了的 Issue (已经解决了的 Issue) 数量占所有 Issue 总数的比例。让你能从宏观的角度把控各个阶段性目标的推进情况。

![db2f3698b864920c.png (1035×636)](http://i4.buimg.com/567571/db2f3698b864920c.png)

### Step 4 任务结束

正如大妈所说，`Issue 永远只是暂时性任务的追踪/提醒/讨论`。  
Issue 最终还是为了推进我们的行动，并形成最终可以 积累/复用/改进 的 作品和成果。在热烈的讨论过后，更需要你真正的去改变，去创作。  
当一个 Issue 完成了它的历史使命时，点击 Close issue。在 close 的同时，记得也在 comment 中附上相关说明或链接，这样任何人看到这个 Issue ，都能一目了然的知道这个任务的进展。

![](http://i2.muimg.com/567571/00a3a02d9b84ad79.png)

## 流程小结

- 初步规划 Issue 的 目的/成果
- 写下简洁的标题
- 写下尽量包含完整信息的 Issue 正文
- 指派对应的 `Assignee` 对接
- 选择对应的 `Labels` 方便检索 
- 根据项目蓝图和阶段性目标，选择和维护 Issue 的 `Project` / `Milestone`
- `Assignee` 跟进并推进 Issue 解决，同时根据实际情况对 Issue 进行维护和调整
- 讨论/行动 后形成新的 决议/作品/代码
- 将 Issue 的 解决情况/链接 以 `Comment` 的形式写在 Issue 下方，并 `Close issue`

## 共同增补渠道

- 你可在 [HbUsageIssue - Wiki](https://github.com/DebugUself/du4proto/wiki/HbUsageIssue) Web 页面直接进行增补
- 你可以[将 Wiki 克隆到本地](https://github.com/DebugUself/du4proto.wiki.git)，在本地修订并提交更新
- 你可在[[WIKI] Issue 创建指南 反馈征集 · Issue #21 · DebugUself/du4proto](https://github.com/DebugUself/du4proto/issues/21) 提交你的反馈和建议

## Changelog

- 170408 zoejane 三稿修订 70 mins
- 170407 zoejane 三稿初稿 70 mins
- 170406 zoejane 二稿文字修订 20 mins
- 170406 zoejane 二稿完成，增补了一个故事 60 mins
- 170405 zoejane 二稿尝试，改成案例故事的形式 40 mins
- 170405 zoejane 完成全文初稿，对文字进行了进一修订 50 mins
- 170405 zoejane 主体部分初稿，根据大妈的建议和框架重写，并附上相关图片  70 mins
- 170403 zoejane 草稿，列出初步提纲 20 mins

## References

- [Mastering Issues · GitHub Guides](https://guides.github.com/features/issues/)
- [Issues · DebugUself/du4proto](https://github.com/DebugUself/du4proto/issues)
- [珠海GDG 社区知识管理 指南](http://blog.zhgdg.org/2014-09/km4gdg-guider/)
- [珠海GDG 社区文章 撰写指南](http://blog.zhgdg.org/2014-09/gdg-writer-guider/)


