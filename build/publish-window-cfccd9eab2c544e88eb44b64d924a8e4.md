---
title: Understanding the Publish Window
short_title: Understanding the Publish Window
description: Bilingual LanCarbon beginner tutorial.
authors:
  - name: Haojie Dai
keywords:
  - LanCarbon
  - Jupyter Book
  - MyST
label: lc-s4-window
---


# Understanding the Publish Window

![GitHub Publishing window](../assets/3bee86d6c17f86702948159c8df238e0589d3b83474d37c7150e41c91ed84d70.png)

The status cards are a checklist:

- **Git** and **GitHub CLI**: required programs and versions.
- **GitHub account**: authenticated account name.
- **GitHub API**: account services can be reached.
- **Book website build**: the saved website exists and matches the current Book.
- **Repository binding**: the connected `owner/repository` exists and is reachable.
- **Git HTTPS connection**: Git can download the publication branch.
- **GitHub Pages**: the public Pages configuration and URL.
- **Published website**: last publication time and commit.

Before the first connection, choose **Existing repository** or **New repository**:

- **Owner or organization** is the GitHub account or organization that owns the repository.
- **Repository name** becomes part of the URL; use letters, numbers, hyphens, periods, or underscores.
- **Publication branch** normally remains `gh-pages`.
- **Visibility** controls repository visibility. GitHub plan and Pages rules may affect private repositories.
- **Connect and Initialize Pages** checks or creates the repository, prepares the branch, configures Pages, and saves the binding.

After connection, the prominent action area appears above repository setup:

- **Update Website** publishes the latest current Build; when the Book changed, follow the rebuild prompt/workflow first.
- **Open Pages** opens the public website.
- **Open Repository** opens the GitHub file/history page.
- **Change repository setup** is an advanced action for connecting a different repository. It is not part of every update.
- **Refresh Checks** reruns environment and connection checks.
- **Close** leaves the panel.

Read the small proxy reminder before operations that contact GitHub. A red error card blocks or explains the affected action; fix that specific prerequisite rather than reconnecting an already valid repository.

---



# 理解 Publish 窗口

![GitHub Publishing 窗口](../assets/3bee86d6c17f86702948159c8df238e0589d3b83474d37c7150e41c91ed84d70.png)

状态卡片是一份检查清单：

- **Git** 与 **GitHub CLI**：必要程序及版本。
- **GitHub account**：已经认证的账号名称。
- **GitHub API**：能否连接账号服务。
- **Book website build**：保存的网站是否存在并与当前 Book 一致。
- **Repository binding**：绑定的 `owner/repository` 是否存在并可访问。
- **Git HTTPS connection**：Git 是否能下载发布分支。
- **GitHub Pages**：公开 Pages 配置和网址。
- **Published website**：上次发布时间与 commit。

第一次连接前，需要选择 **Existing repository** 或 **New repository**：

- **Owner or organization** 是仓库所属的 GitHub 账号或组织。
- **Repository name** 会成为网址的一部分，可使用字母、数字、连字符、句点或下划线。
- **Publication branch** 通常保留为 `gh-pages`。
- **Visibility** 控制仓库可见性。私有仓库能否使用 Pages 可能受 GitHub 套餐和规则影响。
- **Connect and Initialize Pages** 检查或创建仓库、准备分支、配置 Pages 并保存绑定。

连接完成后，主要操作区会出现在 repository setup 上方：

- **Update Website** 发布最新且与 Book 一致的 Build；Book 修改后，先按照界面提示/流程重新构建。
- **Open Pages** 打开公开网站。
- **Open Repository** 打开 GitHub 文件和历史页面。
- **Change repository setup** 是连接其他仓库的高级操作，不是每次更新都要做。
- **Refresh Checks** 重新执行环境与连接检查。
- **Close** 关闭面板。

执行联网操作前，请阅读界面中的代理小字提示。红色错误卡片会阻止或解释受影响的操作；应修复对应前置条件，不要在仓库绑定已经正确时反复重新连接。
