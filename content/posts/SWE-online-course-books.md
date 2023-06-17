+++
title = "转码上岸，我都学了些啥"
date = 2023-06-16 22:47:00
header_img = ""
toc = true
tags = ["码农", "学习", "科技"]
categories = []
series = []
comment = true
+++

全职做 SWE 一周年啦 🎉。回顾总结一下在转码和工作过程中，我都上了哪些课，读了哪些书。

## 网课/Bootcamp

### [Full Stack JavaScript](https://teamtreehouse.com/techdegree/full-stack-javascript) - Treehouse

主要学习了 Javascript、Node.js、 React、 Express、REST API 和 SQL 等， 总共做了 10 个项目，都需要 commit 在 GitHub 上。大约每周学习 10 小时左右。

课程老师讲的很细致，但我最喜欢的地方是每个章节后面都有一个大作业。大作业的要求非常详细，需要什么 function，每个 function 要做什么都会列出，并且没有标准答案，需要自己思考自己写。如果遇到困难，可以在 slack channel 上提问，并且鼓励学生之间互相答疑、互相帮助。

提交完大作业之后，会有老师或者其他已经完成该项目的学生来评分。在自己完成之后，也鼓励批改其他人的大作业，相当于模仿工作中的 PR reivew 了。

我能够免费参加 Treehouse 的这个课程，是因为它当时和一个公司联合搞了这个项目。目前需要付费，所以建议货比三家，选一个经济实惠、适合自己的。

### [The Complete 202X Web Development Bootcamp](https://www.udemy.com/course/the-complete-web-development-bootcamp/) - Udemy

当时我看到很多人都推荐 Angela Yu 的这个网课，于是就买来学了一下，还蛮喜欢的。内容比较基础，和 treehouse 的网课有很大的重叠，对我来说算是查漏补缺了。在 Database 方面两者稍微有点不同，treehouse 用的是 SQLite，Angela 用的是 MongoDB（NoSQL）。

课程在 udemy 打折时候买的，花了$18。

### [Code 15 react projects](https://www.youtube.com/watch?v=a_7Z7C_JCyo) - Youtube

象友推荐了 John Smilga 的这个课程，内容主要集中 React 上。讲得也非常清晰，如果有基础，可以先自己写一遍，如果遇到问题可以网上查查，再看他的解说。

### [Blind 75](https://neetcode.io/practice) - Neetcode

在 data structure and algorithm 上，很多人都推荐 Blind 75。做题的时候发现了 Neetcode 的 YouTube 频道，觉得他讲得相对清晰有条理，而且 75 题非常齐全。Neetcode 现在陆陆续续出了 Neetcode 150，Neetcode All 和一些付费网课。

### [AWS Cloud Practitioner](https://pages.awscloud.com/cloudup-for-her-cloud-practitioner.html) - AWS CloudUp for Her

在象上看到这个免费的 AWS 学习项目，就在上班之余学了一下。它针对女性开放，内容比较基础，不需要技术背景。主要介绍了 AWS 有哪些服务，这些服务项目是用来做什么的。很多公司都用 aws 的云端服务，在面试过程中也有被问到熟不熟悉 aws。学习并通过考试之后会有一个 certificate，不过主要优势还是在于能听得懂同事在说些什么，并能提供自己的观点了。

之后还有一个进阶版的 AWS Solutions Architect 项目，如果对 aws 有所了解可以直接学这个。我打算下半年学一下。

### [How to crack the whiteboard interview](https://www.youtube.com/watch?v=UOvB09u-8oc) - Youtube

这个视频主要讲的是 technical interview 的面试技巧和套路，看了之后很有收获。主要步骤就是

1. 问面试官问题确保理解题目意思，并问到 edge cases
2. 想面试官解释自己的思路，可以先从 brute force 开始，再进行优化。可以写一些 pseudocode。
3. 如果面试官肯定了你思路再开始写码
4. 用一个 test case 测试一遍
5. 分析 time & space complexity - optional

## 书籍

### [Cracking the Coding Interview](https://amzn.to/43LuTwX)\*

实习时候的 buddy 在我走之前给我列了一份大纲，教我如何准备 white board technical interview，用的是这个绿皮的 Cracking the Coding Interview。

顺序上，我先按照他列的知识点开始学习，主要有 Big O、Arrays、Strings、Linked Lists、Stack 、Queue、Tree 、Graph、OOD、Sorting、Searching 和 Testing，再开始做 Blind 75。这样更有系统性。尤其是 Linked Lists、Stack 和 Queue，如果不了解基础概念直接做题，容易云里雾里。

这本书网上资源很多，但我还是比较喜欢用纸质书学习。

### [Designing Data-Intensive Applications](https://amzn.to/3XdWsMH)\*

很多人都推荐读这本书来准备 system design interview，不过 junior 一般不用考虑这个问题。上班之后和同事一起 book club 开始读这本书，基本上两到三周读一章，花了大半年才读完。

收获比想象中要多一点，是一个 connecting 在我脑海中散落的 dots 的过程，当然也学到了很多新的概念。对我来说前面 5 章比较基础，从 database partitioning 开始变得复杂。无论如何，读了之后都对产品的 architecture 有了更多的了解，尤其是同事讲起一些名词的时候听得懂她们在说什么了。

### [Kotlin Design Patterns and Best Practices](https://amzn.to/3PjsftY)\*

Kotlin 是目前比较流行的语言，和 Java 类似，可以用 Java 的 library，但是比 Java 简洁。虽然自己工作中没有在写 Kotlin，但是想要了解和学习这门语言，有种将来会用上的感觉。

前面讲到的两本书的内容适用于各种语言，主要是概念性的。这本书比前面两本要轻松好读很多，内容只和 Kotlin 相关，有很多 code snippets 做例子，非常具体。

---

\*_提供的是我的 amazon affiliate links。_
_如果想要支持本地书店，我推荐[bookshop.org](https://bookshop.org/)。可以选择支持的书店，买书之后 bookshop 就会把部分收益捐赠给你选择的书店。_
