---
title: What Publish Means and How It Differs from Build
short_title: What Publish Means and How It Differs from Build
description: Bilingual LanCarbon beginner tutorial.
authors:
  - name: Haojie Dai
keywords:
  - LanCarbon
  - Jupyter Book
  - MyST
label: lc-s4-concepts
---


# What Publish Means and How It Differs from Build

Build creates and checks the website on your computer. Publish transfers that checked website to GitHub and makes a public URL available through GitHub Pages.

| Build | Publish |
|---|---|
| Uses Python and Jupyter Book 2 | Uses Git, GitHub CLI, a GitHub account, and network access |
| Produces a local HTML website | Updates a GitHub branch |
| Can work offline for local content | Must reach GitHub services |
| Should happen after meaningful edits | Happens after a current successful Build |

Important Git concepts for this workflow:

- A **repository** is the online container for files and their history.
- A **commit** is one recorded version. LanCarbon shows the short commit identifier after publishing.
- A **branch** is one line of versions. LanCarbon normally publishes website files to `gh-pages`.
- **GitHub Pages** serves the root of that branch as a website.

You do not need to type routine Git commands. LanCarbon creates, clones, updates, commits, pushes, and checks the publication branch through its workflow. Do not manually delete or rewrite `gh-pages` unless you understand the consequence.

Publishing does not upload the private LanCarbon data directory. It sends generated website files required by the public site. Still, review your Book for private text, images, attachment contents, metadata, and hidden pages before publishing.

---



# Publish 的含义及其与 Build 的区别

Build 在你的电脑上生成并检查网站；Publish 把检查过的网站传到 GitHub，再由 GitHub Pages 提供公开网址。

| Build | Publish |
|---|---|
| 使用 Python 和 Jupyter Book 2 | 使用 Git、GitHub CLI、GitHub 账号和网络连接 |
| 生成本地 HTML 网站 | 更新 GitHub 仓库中的分支 |
| 内容均为本地时可以离线完成 | 必须能够连接 GitHub 服务 |
| 有重要修改后执行 | 当前成功 Build 之后执行 |

本流程涉及的 Git 基本概念：

- **Repository（仓库）** 是在线存放文件和历史记录的容器。
- **Commit（提交）** 是一次被记录的版本。发布后 LanCarbon 会显示简短 commit 标识。
- **Branch（分支）** 是一条版本线。LanCarbon 通常把网站文件发布到 `gh-pages`。
- **GitHub Pages** 会把该分支根目录作为网站提供。

日常流程不要求你手工输入 Git 命令。LanCarbon 会在工作流中创建、下载、更新、提交、推送并检查发布分支。如果不了解后果，不要手动删除或重写 `gh-pages`。

Publish 不会上传整个 LanCarbon 私有数据目录，而是发送公开网站需要的生成文件。即便如此，发布前仍应检查 Book 中是否包含隐私文字、图片、附件内容、元数据或不希望公开的隐藏页面。
