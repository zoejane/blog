
---
title: "想参与心仪的开源项目？开始你的 Pull Request 吧"
date: 2017-06-15T11:23:20+08:00
categories: ["Tech", "Tutorial"]
---

**Link**

- [72h [DUW] 想参与心仪的开源项目？开始你的Pull Request 吧 · Issue #145 · DebugUself/du4proto](https://github.com/DebugUself/du4proto/issues/145)


- 170615 已更新至 Wiki [如何提交 Pull Request · DebugUself/du4proto Wiki](https://github.com/DebugUself/du4proto/wiki/How2PR)
欢迎小伙伴们共同增补 @DebugUself/du4all

## 人生第一个 Pull Request

- **发现** - 最近一直在捣鼓怎么用 [Google Magenta](https://github.com/tensorflow/magenta) 写音乐，也是在阅读文档时无意中发现有几处小小的错误，忽然想到，既然项目是放在 GitHub 上，也许我可以试试为他们修正这几处小小错误并提交过去呢。
- **尝试** - 怀着又兴奋又忐忑的心情，开始动手啦。我尝试着看看别人在 [Magenta 项目 的 Pull Requests](https://github.com/tensorflow/magenta/pulls) 是怎么做的，然后对照着 [GitHub Help](https://help.github.com/) 开始做。Fork仓库，修订代码，提交 Pull Request [fix typos in improv_rnn readme](https://github.com/tensorflow/magenta/pull/709)，然后，等了一天后，发现自己的代码真的接受啦！
- **开心** - 人生中第一个真正意义上的 Pull Request，虽然只是给Google Magenta 项目改了几个 typos ，不过能给自己喜欢的项目做小小贡献感觉特别开心哇！顿时觉得这些项目离我也不是那么遥远了。GitHub真的好棒！把这件事情变得这么简单。

## 快速行动指南

想不想现在就开始行动？

### 视频版指南

- 自己尝试着为小伙伴们录制了视频版指南，欢迎来  [反馈](https://github.com/DebugUself/du4proto/issues/146) 喔
    - [How to Pull Request in GitHub - YouTube](https://www.youtube.com/watch?v=mtVYWfawl3c) 
    - 国内镜像地址 [如何在 GitHub上进行Pull Request - Youku](http://v.youku.com/v_show/id_XMjgyNTgxNDY4OA==.html?spm=a2h3j.8428770.3416059.1)

### 指令清单
这里附上简单版本的指令清单给你参考  
（以 DebugUself 的 [playground](https://github.com/DebugUself/playground)  仓库为例）

- 系统环境说明
    - macOS 10.12.2
    - git 2.10.1 
- Fork 想参与的仓库 [playground](https://github.com/DebugUself/playground)
- `git clone git@github.com:zoejane/playground.git` 
    - `git@github.com:zoejane/playground.git` 替换成 你 Fork 后的仓库地址
- `cd playground`
- `git remote add upstream git@github.com:DebugUself/playground.git` 
    - `git@github.com:DebugUself/playground.git` 替换成项目原始仓库地址
- `git fetch upstream`
- `git branch -u upstream/master master` 
- `git checkout -b pr-test` 
    - `pr-test`更换成你自己使用的分支名
- 本地修订代码
- `git add .`  
- `git commit -m 'pr test'` 
    - `pr test` 更换成你自己的 commit message
- `git fetch upstream`
- `git merge upstream/master`
- `git push -u origin pr-test`
    - `pr-test`更换成你自己使用的分支名
- 去原始仓库界面，点击 `New pull request` ，点击 `compare across forks`，在左边的 `base` 部分选择你想更新的原始仓库和分支，右边的 `head` 部分选择自己 Fork 仓库中的分支，填写描述，点击 `Create pull request`

### 更多资源

- GitHub 已经为我们提供了非常详尽的文档 [Creating a pull request from a fork - User Documentation](https://help.github.com/articles/creating-a-pull-request-from-a-fork/)
- Kent C. Dodds 为我们提供的详细的视频教程 [How to Contribute to an Open Source Project on GitHub](https://egghead.io/courses/how-to-contribute-to-an-open-source-project-on-github)

## A Step-by-Step Guide 

如果你想要更详细的步骤，可以阅读这里。

- 系统环境说明
    - macOS 10.12.2
    - git 2.10.1 

### Fork 仓库 并 Clone 到本地

- Fork 想参与的仓库 (以 DebugUself 的 [playground](https://github.com/DebugUself/playground)  仓库为例)
    - 在你想要参与的仓库界面上，点击 `Fork`
- 获取你 Fork 后的仓库地址 
    - 打开你自己 Fork 后的仓库界面，点击 `Clone or download`, 复制仓库地址
- 将仓库 Clone 到本地
    - `git clone git@github.com:zoejane/playground.git`
        - `git@github.com:zoejane/playground.git` 替换成 你 Fork 后的仓库地址 
        - 如果之前没有配置 SSH ，也可以用 HTTPS 地址。
            - 点击 `Use HTTPS` 切换到 HTTPS 地址
            - `git clone https://github.com/DebugUself/playground.git`
    - `cd playground`

### 与原始仓库保持同步

- 去原始仓库的主页，点击 `Clone or download`, 复制仓库地址
- 添加远程仓库 `git remote add upstream git@github.com:DebugUself/playground.git`
    - `git@github.com:DebugUself/playground.git` 替换成项目原始仓库地址 
- 获取远程仓库信息 `git fetch upstream`
- 将本地仓库的主分支(master)代码与远程仓库保持更新 `git branch --set-upstream-to=upstream/master master` 
     - `git branch —set-upstream-to=<远程仓库名称>/<远程分支名称> <本地分支名称>`
     - 完成后，你会看见提示 `Branch master set up to track remote branch master from upstream.`

### 开始修订

- 新建修订分支，这里以 `pr-test` 为例
    - `git checkout -b pr-test`  
    - 也可以缩写为 `git co -b pr-test`
- 开始修订自己的本地代码
- 将修改提交到自己的仓库中
    - `git add .`  
        - 此处`.` 也可以替换成你想提交的修订了的文件名
    - 可以随时用 `git status` 检查仓库的状态
    - `git commit -m '...'` 
        - 写上你具体修订的内容，引号里面 `...` 部分就是你的 commit message
        - commit message 可以用 `<type>(<scope>): <subject>` 的形式)
- 合并最近的原始仓库的主分支内容
    - `git fetch upstream`
    - `git merge upstream/master`
- 将代码更新至我们自己 Fork 的仓库中 `git push -u origin pr-test` 
    - `-u` 告诉 Git 记得我们的参数
    - 这样以后只要用 `git push` 命令就可以将 `pr-test` 分支中的代码直接更新到我们的仓库中
    - 你可以看到提示 `Branch pr-test set up to track remote branch pr-test from origin.`

### 提交 Pull Request

- 在原始代码仓库，点击白色的 `New pull request` 按钮
- 点击蓝色的 `compare across forks` 链接
- 将 `head fork` 改成你自己的 fork 仓库，并将 `compare` 后的分支改成你自己刚刚修订的分支 `pr-test`
- 系统会为你自动生成一个 Pull Request 界面，标题部分默认就是我们写的 commit message，可以在内容部分写上更详细的说明或者自己遇到的问题
- 等待原始仓库维护者的反馈和确认，代码合并。
- 代码合并成功后，你会看到一段提示 `Pull request successfully merged and closed. You’re all set—the zoejane:pr-test branch can be safely deleted.` 这时，你可以放心的删除修订分支`pr-test`啦。

## 小结

- 不妨现在就开始动手试试吧
- 小练习
	- Fork DebugUself 的 [playground](https://github.com/DebugUself/playground)  仓库
	- 修订代码并上传到自己的仓库中
	- 提交 Pull Request
	- 试试通过自己的 Pull Request（在 DebugUself 里，每个人都有通过Pull Request 的权限的）
	-  合并完成后，删除自己仓库的修订分支
- 练习完成后， GitHub 广阔的开源项目等着你玩耍啦。试着参与你心仪的开源项目吧 ^_^

## Changelog

- 170615 zoejane 文字修订
- 170615 zoejane 更新视频地址
- 170613 zoejane 全文第一稿完成
- 170612 zoejane 主体部分初稿




