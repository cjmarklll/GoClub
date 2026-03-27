# GoClub

GoClub 是一个围绕技术面试准备与系统复习搭建的内容站点，主要整理面试真题、八股总结、资料视频、项目推荐，以及视频配套文章等内容。

当前站点基于 Hugo 构建，部署在 GitHub Pages，自定义域名为 `blockblog.top`。

- 站点地址：https://blockblog.top
- 在线提交流程页：https://blockblog.top/docs/blog/%E6%8F%90%E4%BA%A4%E6%B5%81%E7%A8%8B/
- 仓库地址：https://github.com/LeoninCS/GoClub

## 如何提交内容

如果你想给 GoClub 补充面试题、八股、配套文章，或者修正文档中的错误，可以按下面这套流程提交。

### 1. Fork 仓库

先 Fork 这个仓库到你自己的 GitHub 账号下。

### 2. Clone 到本地

```bash
git clone https://github.com/<your-github-name>/GoClub.git
cd GoClub
```

### 3. 新建分支

不要直接在 `main` 上修改，先创建一个新分支：

```bash
git checkout -b docs/your-topic
```

分支名可以参考：

```text
docs/add-tencent-interview
docs/fix-companion-links
docs/update-mysql-notes
```

### 4. 添加或修改文档

把内容放到 `content/docs` 对应的栏目下面：

- `content/docs/interview/`：面试真题
- `content/docs/baguwen/`：八股总结
- `content/docs/companion/`：配套文章
- `content/docs/blog/`：实践经验或技术记录

如果你是新增页面，记得同步修改对应目录下的 `_index.md`，不然文章可能已经存在，但目录页里看不到入口。

### 5. 本地预览

安装 Hugo 后，在项目根目录执行：

```bash
hugo server
```

默认访问地址通常为：

```text
http://localhost:1313/
```

提交前建议至少检查这些内容：

- 页面能否正常打开
- 目录页能否点到新文章
- 标题、图片、代码块、链接是否正常显示
- 是否有明显错别字、断链或排版问题

### 6. 提交代码并推送

```bash
git add .
git commit -m "docs: add your topic"
git push origin docs/your-topic
```

### 7. 发起 Pull Request

回到 GitHub，在你 Fork 的仓库页面发起 PR，到上游仓库的 `main` 分支。

PR 描述里建议写清楚：

- 这次新增或修改了什么内容
- 文档放在哪个目录
- 是否同步更新了对应目录的 `_index.md`

### 8. 等待合并与部署

PR 被合并后，站点会通过 GitHub Actions 自动构建并发布。

如果你的 PR 被成功合并，部署完成后，你也会出现在贡献者页面中。

## 内容范围

GoClub 当前主要覆盖以下方向：

- 面试真题
- 八股知识总结
- 资料与视频推荐
- 项目推荐
- 视频配套文章

目标是把零散、重复、难以检索的内容，整理成更适合复习和查阅的知识库。

## 本地运行与构建

本地运行：

```bash
hugo server
```

构建静态文件：

```bash
hugo --minify
```

## 项目结构

```text
content/
  _index.md            # 站点首页
  docs/
    _index.md          # 文档分区首页
    interview/         # 面试真题
    baguwen/           # 八股总结
    companion/         # 配套文章
    blog/              # 技术博客与提交流程

.github/workflows/
  static.yml           # GitHub Pages 自动部署
```

## 补充说明

- 仓库推送到 `main` 后，会通过 GitHub Actions 自动构建并发布到 GitHub Pages
- 站点当前使用的主题是 `hugo-book`
- 如果你只是想快速查看详细步骤，也可以直接打开 [投稿与提交流程](content/docs/blog/提交流程.md)
