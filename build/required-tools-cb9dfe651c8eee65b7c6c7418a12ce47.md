---
title: Tools Required from Writing to Publishing
short_title: Tools Required from Writing to Publishing
description: Bilingual LanCarbon beginner tutorial.
authors:
  - name: Haojie Dai
keywords:
  - LanCarbon
  - Jupyter Book
  - MyST
label: lc-s1-tools
---

## English

# Tools Required from Writing to Publishing

LanCarbon is the writing and workflow application. Several independent tools perform the website and GitHub work. You do not need every tool merely to write.

| Stage | Requirement | Purpose | Account needed? |
|---|---|---|---|
| Write and Preview | LanCarbon | Stores and edits your Book | No |
| Build | Python 3 | Runs the Jupyter Book package | No |
| Build | Jupyter Book 2 CLI | Converts MyST/Markdown into a website | No |
| Publish | Git | Downloads and updates the publication branch | No |
| Publish | GitHub account | Owns the repository and Pages site | Yes |
| Publish | GitHub CLI (`gh`) | Lets LanCarbon authenticate and use GitHub services | Yes |
| Publish | Internet access | Reaches GitHub API, Git HTTPS, and Pages | — |

## Why Python and Jupyter Book are required

LanCarbon creates a Jupyter Book 2 project from the Book stored inside the app. Python runs the official Jupyter Book command-line tool, which validates the project and produces HTML. Install Python 3 from [python.org](https://www.python.org/downloads/) and ensure the `python` or `py` command is available. Then install Jupyter Book 2 following the [official installation guide](https://jupyterbook.org/stable/get-started/install/). A common installation command is:

```powershell
python -m pip install "jupyter-book>=2.0.0"
```

The **Build** window checks both Python and Jupyter Book CLI and displays their detected versions. Restart LanCarbon after installing or updating them so the app receives the updated command search path.

## Why Git, GitHub, and GitHub CLI are required

Git records and transfers a set of website files. GitHub hosts a repository. GitHub Pages serves one branch of that repository as a website. GitHub CLI connects LanCarbon to your signed-in GitHub account without asking LanCarbon to store your password.

- Install Git from the [official Git for Windows page](https://git-scm.com/install/windows).
- Create a personal account at [github.com](https://github.com/).
- Install GitHub CLI from the [official installation page](https://cli.github.com/).
- Authentication is completed later from LanCarbon's Publish window.

GitHub Desktop is optional and does not replace the Git and GitHub CLI checks used by LanCarbon.

## Network note

Writing and most local Builds do not need GitHub. Signing in, creating or checking a repository, downloading its publication branch, publishing, and opening the public Pages site do need access to GitHub. On networks that require a proxy, a browser-only proxy may not cover Git or GitHub CLI. Enable the proxy's **system/global proxy** or **TUN mode** before those operations, then retry the check.

---

## 中文

# 从写作到发布所需的工具

LanCarbon 是写作和流程管理软件，另有几项独立工具负责生成网站及连接 GitHub。仅仅撰写内容时，不需要提前安装全部工具。

| 阶段 | 必需项目 | 用途 | 是否需要账号 |
|---|---|---|---|
| Write 与 Preview | LanCarbon | 保存和编辑 Book | 否 |
| Build | Python 3 | 运行 Jupyter Book 软件包 | 否 |
| Build | Jupyter Book 2 CLI | 把 MyST/Markdown 转换成网站 | 否 |
| Publish | Git | 下载并更新发布分支 | 否 |
| Publish | GitHub 账号 | 拥有仓库和 Pages 网站 | 是 |
| Publish | GitHub CLI（`gh`） | 让 LanCarbon 使用已登录的 GitHub 身份 | 是 |
| Publish | 可访问 GitHub 的网络 | 连接 GitHub API、Git HTTPS 和 Pages | — |

## 为什么 Build 需要 Python 和 Jupyter Book

LanCarbon 会把软件内保存的 Book 转换成 Jupyter Book 2 项目。Python 负责运行官方 Jupyter Book 命令行工具，后者检查项目并生成 HTML 网站。请从 [python.org](https://www.python.org/downloads/) 安装 Python 3，并确保系统可以找到 `python` 或 `py` 命令。随后按照 [Jupyter Book 官方安装说明](https://jupyterbook.org/stable/get-started/install/)安装 Jupyter Book 2。常用命令为：

```powershell
python -m pip install "jupyter-book>=2.0.0"
```

**Build** 窗口会同时检查 Python 和 Jupyter Book CLI，并显示检测到的版本。安装或更新它们后，请重启 LanCarbon，使软件重新读取系统命令路径。

## 为什么 Publish 需要 Git、GitHub 与 GitHub CLI

Git 负责记录并传输一组网站文件；GitHub 用仓库存放这些文件；GitHub Pages 把仓库中的指定分支作为网站提供；GitHub CLI 让 LanCarbon 使用已经登录的 GitHub 账号，而不需要在 LanCarbon 中保存密码。

- 从 [Git for Windows 官方页面](https://git-scm.com/install/windows)安装 Git。
- 在 [github.com](https://github.com/)创建个人账号。
- 从 [GitHub CLI 官方页面](https://cli.github.com/)安装 GitHub CLI。
- 账号认证会在后面的 LanCarbon Publish 窗口中完成。

GitHub Desktop 是可选工具，不能替代 LanCarbon 所检查的 Git 和 GitHub CLI。

## 网络说明

写作和大多数本地 Build 不需要连接 GitHub。登录账号、创建或检查仓库、下载发布分支、发布网站和打开公开 Pages 网站都需要能够访问 GitHub。如果所在网络需要代理，仅对浏览器生效的代理可能无法覆盖 Git 或 GitHub CLI。请先开启代理软件的 **系统/全局代理** 或 **TUN 模式**，再重试相关检查。
