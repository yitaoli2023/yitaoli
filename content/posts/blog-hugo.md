+++
title = "我也自建博客啦 + 对教程的补充"
date = 2023-06-13 08:44:52
tags = [
    "博客",
    "hugo",
    "科技"
]
subtitle = ""
header_img = ""
toc = true
+++

## 为什么决定自建博客

由于不想认证身份，也无法收到国内手机号验证码，微信公众号和豆瓣都上不去了。作为内容的创作者，却要看平台脸色这种事情也是受够了，就决定搞一个博客。

## 工具选择

其实主流的工具都有所了解。

- 因为之前的工作原因，用过 WordPress。没有选择它是因为太慢，而且限制多，后台管理页面陈旧。

- 用 Wix 做过 portfolio，比 WordPress 简单易上手，拖拖拽拽就行。但是免费版本有 Wix 的广告。

- Notion 对我来说是一个做笔记和计划的工具，而非面向大众的阅读平台。

- 转码 Bootcamp 的时候用 Github Pages 做 portfolio 展示过自己做的一些项目，但是手写整个网站比较花时间。

原本想用 node 和 express 手写一个 static site，但是由于稍微有点麻烦，所以拖延了好一阵儿。最后吃了椒老师的[安利](https://blog.douchi.space/blog-migrate-wordpress-hugo/#gsc.tab=0)，决定试一下 Hugo template + Github Pages 的组合。

## Mac 配置环境

主要操作就是按照椒老师搜索到的[教程](https://levelup.gitconnected.com/build-a-personal-website-with-github-pages-and-hugo-6c68592204c7)，但是在第一步之前补充几点 command line 环境相关的背景。

1. 在安装 hugo 之前，先要安装[homebrew](https://brew.sh/)。打开 terminal 复制粘贴回车一行 code 就行。

2. 在安装 git 之前，先要安装 xcode。xcode 可以在 app store 上找到。
   之前虽然有安装 xcode，因为太久没有在自己的电脑上写码，检查 git version 的时候遇到了一个错误。

```bash
xcrun: error: invalid active developer path (/Library/Developer/CommandLineTools), missing xcrun at: /Library/Developer/CommandLineTools/usr/bin/xcrun
```

> 鸡汤时刻：
> 看不看得懂这个错误不是很要紧，关键是不要慌。把这个错误放到 google 里搜索一下就行。99%的情况就是别人也遇到过同样的问题，而且已经有了答案。这个心态适用于 junior 码农写码中遇到的 80%的问题。剩下的 20%可能是技术过于新颖/落后，或者解决问题需要 domain knowledge。

根据[这个](https://apple.stackexchange.com/questions/254380/why-am-i-getting-an-invalid-active-developer-path-when-attempting-to-use-git-a)问答，只走了第一步`xcode-select --install`，重新安装了一下，问题就解决了。

## 搭建博客

### 模版选择

我选择了这个[puppet theme](https://github.com/roninro/hugo-theme-puppet)，它有一个[demo](https://hugo-theme-puppet.netlify.app/)。具体如何添加自己的文章，如何根据自己的需求需改，还是要根据模版的 documentation 来。Puppet 大差不差能满足我的需求，但是局限性也有。博客上线之后，后续应该会做更加精细的修改。

### 搭建过程

主要就根据[教程](https://levelup.gitconnected.com/build-a-personal-website-with-github-pages-and-hugo-6c68592204c7)和我选择的[theme 的教程](https://hugo-theme-puppet.netlify.app/posts/getting-started/)，有几点注意：

1. Hugo version: 我的版本已经是 hugo v0.113.0，教程中的 config.toml 已经改为 hugo.toml。
<figure>
     <img style="max-width: 40%" src="/yitaoli/img/toml.png">
</figure>

2. Main vs Master: Github 将 master 改为 main, commit 的时候要注意。选择用
   `git push -u origin main`

3. 我选择的 theme 有两种添加方式， 一个是 clone，另一个是添加为 submodule。第一次选择了 clone 到 theme 文件夹，但是 commit 的时候还是要求将其添加为 submodule。建议直接选择添加为 submodule。
4. 我按照椒老师的建议 commit 整个 repo，选择了 Github Actions 来 build 网页。这样跳过了在本地 build 的步骤。source 选 Github Actions 之后，需要点击 Actions，搜索 Hugo， 按照提示添加 workflow。这样就可以自动 build 和 deploy。如果选择这种方式，需要将前面的 hugo.toml 改名为 config.toml。

### 如何在电脑登不上豆瓣的情况下阅读全文

前面讲到我已经登不上自己的豆瓣了，但是不甘心文章白白丢失，于是七搞八搞找到了几篇放到了这里。

如果你能有幸找到文章链接，会发现文章只显示开头一部分。此时选择右键 Inspect，并在 Dimensions 选择手机格式，就会发现“阅读全文”的按键。如果需要复制粘贴功能，就在点击该按钮后刷新，关掉 inspect，这样就可以复制粘贴全文了。

## 写在最后

这些年零零散散在各个平台上写了一些文章，最后散落天涯自己都找不到看不了了。目前准备实施的整理和规划是在 Notion 上写草稿，发布在 github 上面。

还没研究 RSS 是怎么回事，总之先放在这里 `https://yitaoli2023.github.io/yitaoli/index.xml`
