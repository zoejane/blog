
---
title: "ReportBot 报告生成小助手发布"
date: 2018-04-06T11:23:18+08:00
categories: ["Tech", "Programming"]
---

**Link**

- [5d [ANN] ReportBot 报告生成小助手发布 (附彩蛋:大妈嗯哼合集) · Issue #373 · DebugUself/du4proto](https://github.com/DebugUself/du4proto/issues/373)

# ReportBot

ReportBot 报告生成小助手 v.18.4.5 发布，请小伙伴们来试玩啦 @DebugUself/du4all 
自己测试了一下，生成一份 7 天的 周报，根据 commits 的多少和网络情况可能会需要 1 - 3 分钟，所以可以先开着运行一会儿

### 体验

- 用编程解决自己真正想解决的问题，好开心
- 即使没有合适的官方 Demo 和教程指导，跟着 Google,  跟着文档 一步步探索未知问题，一样是可以搞定的，也算是积累了自己探索未知领域信心啦
- 即使很久没有编程忘得差不多了，即使每天没有很多时间，把 MVP 用上来，不断迭代，原来觉得很难的问题就不知不觉一个个解决了。哪怕只是写了一行代码，实现了一个很小的新功能，也是一个 MVP。记录下来，积累，迭代。
- 动手写代码是最好的学习，中间经历的很多磕磕绊绊会让人成长，比看书、看教程来的体验深很多。当然看书、看教程能够更好地梳理和发现自己的漏洞，但是动手写代码的时间一定要多。

## Background

- 想回顾一下自己过去这一周都做了什么？
- 想把自己在 Issue 和 Comments 中写过的文字都保留一份存档？
- 想追踪自己感兴趣的人，比如 @ZoomQuiet 这一年来都做了些什么？
- ...

手工查阅好麻烦，能不能一键生成 Markdown 文档呢？

编程已经荒废很久，感觉快要失忆了，发现自己既然有这个需求，就尝试用 PyGithub 开发一个小助手来帮我吧。

## Usage

~ du4proto 仓库 -> DU_tools 分支 -> ReportBot 目录
[Link](https://github.com/DebugUself/du4proto/blob/DU_tools/ReportBot/repobot.py)

`$ python3 repobot.py`

- 输入你感兴趣的人的 Github Username, 如 `zoejane`
- 输入你想追踪的多少天, 比如 `7`

ReportBot 小助手就会自动在你运行程序的目录下，生成三份 Markdown 格式的报告啦

- username-commits-report.md
- username-issues-report.md
- username-commit-comments-report.md

运行需要 PyGithub 支持 

`$ pip3 install PyGithub`

## 需要改进的

- 如何调用 st 统计接口服务，更方便快捷的获取数据
- 遍历所有 branch 获取 commits 的速度很慢，如何加速
- 非 orphan 的分支下，会有好些重复的 commits, 如何加不大幅拖慢运行速度的情况下，用 SHA 去重
- access token 有没有更好的加密方式
- ...

@ZoomQuiet  [回复](https://github.com/DebugUself/du4proto/commit/34c95d3431a18f84dee66da1ed97990d2be551ac#commitcomment-28432108)

```
是也乎,(￣▽￣)
事实上, @zoejane 在写的工具, 
当前已经完成了哪, 集成在 Heroku 的 st 统计接口服务中,
参考:

- 整体设计过程参考:[README.md](https://github.com/DebugUself/du4proto/blob/DU_tools/st/README.md)
- 具体接口: [du4proto/st.py at ZQ4mDjango · DebugUself/du4proto](https://github.com/DebugUself/du4proto/blob/ZQ4mDjango/heroku/st.py#L31)

另外, 这种工具要考虑和检测的东西比较多,
最好先规划好, 再逐一完成,
否则, 容易在 coding 过程中迷失...
```

## 彩蛋

大妈 @ZoomQuiet 过去一年 (截止到2018.4.4.) 在怼圈的的各种嗯哼，里面可以发掘出超多大妈给的隐藏任务喔 :)


## Changelog

- 180405 zoejane 发布 v18.4.5
- 180401 zoejane 启动 ReportBot 项目



