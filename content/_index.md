---
title: "GoClub"
---

# GoClub

GoClub 是一个面向技术面试准备与系统复习的内容站点，重点整理高频面试真题、常见八股总结、优质资料视频、项目推荐，以及视频配套文章。

这个项目使用 Hugo 生成静态页面，通过 GitHub Pages 对外发布，当前主题为 `hugo-book`。整体目标不是做传统博客，而是沉淀一套更适合面试复习、查漏补缺和系统整理的知识内容库。

## 投稿入口

想给 GoClub 投稿、补充内容，或者修正文档问题，可以直接查看这里：

- [投稿与提交流程]({{< relref "/docs/blog/提交流程.md" >}})

## 想投稿或补充内容？

想给 GoClub 补充面试题、八股、配套文章，或者修正文档问题，可以直接查看 [投稿与提交流程]({{< relref "/docs/blog/提交流程.md" >}})。

PR 被合并后，站点会自动部署，你也会出现在 [贡献者]({{< relref "/docs/contributors/_index.md" >}}) 页面。

- Fork 仓库并新建分支
- 在 `content/docs` 对应目录下添加或修改文档
- 同步更新对应目录的 `_index.md`
- 本地运行 `hugo server` 检查页面
- 提交 PR 等待合并

## 站点栏目

GoClub 目前主要覆盖以下内容：

- [面试真题](./docs/interview/)
- [八股总结](./docs/baguwen/)
- 资源荟萃
- [配套文章](./docs/companion/)
- [技术博客](./docs/blog/)
- [贡献者](./docs/contributors/)

## 快速入口

- [内容导航](./docs/)
- [投稿与提交流程](./docs/blog/提交流程/)
- [面试真题](./docs/interview/)
- [八股总结](./docs/baguwen/)
- [配套文章](./docs/companion/)
- [技术博客](./docs/blog/)
- [贡献者](./docs/contributors/)

## 当前技术方案

- 静态站点生成器：Hugo
- 部署平台：GitHub Pages
- 页面主题：hugo-book
- 内容格式：Markdown

如果你是第一次进入这个站点，可以先从任意栏目开始浏览，后续内容会逐步补全。
