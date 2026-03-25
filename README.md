# GoClub

GoClub 是一个围绕技术面试准备与系统复习搭建的内容站点，主要整理面试真题、八股总结、资料视频、项目推荐，以及视频配套文章等内容。

当前站点基于 Hugo 构建，部署在 GitHub Pages，自定义域名为 `blockblog.top`。

## 内容定位

GoClub 目前重点整理以下方向：

- 面试真题
- 八股知识总结
- 资料与视频推荐
- 项目推荐
- 视频配套文章

目标是把零散、重复、难以检索的内容，整理成更适合复习和查阅的知识库。

## 技术栈

- Hugo
- hugo-book
- GitHub Pages
- Cloudflare

## 本地运行

安装 Hugo 后，在项目根目录执行：

```bash
hugo server
```

默认访问地址通常为：

```text
http://localhost:1313/
```

## 构建

```bash
hugo --minify
```

## 项目结构

```text
content/
  _index.md            # 站点首页
  docs/
    _index.md          # 文档分区首页
    project.md         # 项目介绍

.github/workflows/
  static.yml           # GitHub Pages 自动部署
```

## 部署说明

仓库推送到 `main` 后，会通过 GitHub Actions 自动构建并发布到 GitHub Pages。

站点当前使用自定义域名：

```text
https://blockblog.top
```

## 后续规划

- 补充高频面试真题专题
- 按主题整理八股知识
- 增加资料与视频索引
- 增加项目推荐与项目解析
- 为视频内容补充文字版文章
