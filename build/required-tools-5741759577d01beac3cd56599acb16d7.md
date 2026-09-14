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


# Tools Required from Writing to Publishing

## Managed installation with Environment Setup

Open **Environment Setup** from the sidebar, Build or Publish. It reports the detected version, executable location and compatibility of Python, Node.js, Jupyter Book 2, Git and GitHub CLI, plus GitHub sign-in and connectivity. Compatible system tools are marked **Using existing** and have no Install button. For a missing or incompatible tool, select **Install managed copy**. Installing Jupyter Book 2 also prepares missing managed Python and Node.js dependencies. LanCarbon shows download, verification, deployment and post-install progress, installs only below `LanCarbon\Tools`, and checks it again. Managed Python is portable and cannot update a registered system Python; Cancel stops work and removes partial files. Use **Instructions** instead if you prefer a manual system installation.

If an installation or environment check reports an error, open [Troubleshooting Common Problems](../04-publish/troubleshooting.md) directly; you do not need to wait until the later publishing chapter.

Managed tools do not require a system PATH change. A compatible system installation is still accepted and is not removed or overwritten. Installation details are saved in the Environment Setup log. If GitHub downloads fail, enable the proxy application's system proxy or TUN mode and retry.

## 使用 Environment Setup 进行受管理安装

从侧边栏、Build 或 Publish 打开 **Environment Setup**。页面会显示 Python、Node.js、Jupyter Book 2、Git、GitHub CLI 的版本、可执行文件位置与兼容性，并检查 GitHub 登录和网络。系统中已有的兼容工具显示 **Using existing**，不提供 Install 按钮。缺失或不兼容时可点击 **Install managed copy**；安装 Jupyter Book 2 时也会自动准备缺失的受管理 Python 和 Node.js。LanCarbon 会显示下载、校验、部署和复检进度，只安装到 `LanCarbon\Tools` 下。受管理 Python 是便携版，不会更新已注册的系统 Python；Cancel 会停止任务并清理未完成文件。如果希望自行安装到系统，请使用 **Instructions**。

如果安装或环境检查报错，可以直接打开[常见问题处理（Troubleshooting Common Problems）](../04-publish/troubleshooting.md)，无需等到后面的发布章节。

受管理工具不要求修改系统 PATH。系统中已有的兼容版本仍会被接受，LanCarbon 不会删除或覆盖它。安装详情保存在 Environment Setup 日志中。如果 GitHub 下载失败，请开启代理软件的系统代理或 TUN 模式后重试。


LanCarbon is the writing and workflow application. Several independent tools perform the website and GitHub work. You do not need every tool merely to write.

| Stage | Requirement | Purpose | Account needed? |
|---|---|---|---|
| Write and Preview | LanCarbon | Stores and edits your Book | No |
| Build | Python 3 | Runs the Jupyter Book package | No |
| Build | Node.js | Runs the MyST engine used by Jupyter Book 2 | No |
| Build | Jupyter Book 2 CLI | Converts MyST/Markdown into a website | No |
| Publish | Git | Downloads and updates the publication branch | No |
| Publish | GitHub account | Owns the repository and Pages site | Yes |
| Publish | GitHub CLI (`gh`) | Lets LanCarbon authenticate and use GitHub services | Yes |
| Publish | Internet access | Reaches GitHub API, Git HTTPS, and Pages | — |

## Why Python, Node.js and Jupyter Book are required

LanCarbon creates a Jupyter Book 2 project from the Book stored inside the app. Python runs the Jupyter Book package, while Node.js runs its MyST engine; both are required to validate the project and produce HTML. The simplest route is **Environment Setup**: select **Install managed copy** for a missing item, or install Jupyter Book 2 and let LanCarbon prepare any missing managed Python and Node.js dependencies automatically. For manual system installations, use [python.org](https://www.python.org/downloads/), the [Node.js download page](https://nodejs.org/en/download/), and the [Jupyter Book installation guide](https://jupyterbook.org/stable/get-started/install/). A common Jupyter Book command is:

```powershell
python -m pip install "jupyter-book>=2,<3"
```

The **Build** window checks Python, Node.js and Jupyter Book CLI and displays their detected versions. Managed copies work without changing the system PATH. Restart LanCarbon after a manual system installation so the app receives the updated command search path.

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



# 从写作到发布所需的工具

LanCarbon 是写作和流程管理软件，另有几项独立工具负责生成网站及连接 GitHub。仅仅撰写内容时，不需要提前安装全部工具。

| 阶段 | 必需项目 | 用途 | 是否需要账号 |
|---|---|---|---|
| Write 与 Preview | LanCarbon | 保存和编辑 Book | 否 |
| Build | Python 3 | 运行 Jupyter Book 软件包 | 否 |
| Build | Node.js | 运行 Jupyter Book 2 使用的 MyST 引擎 | 否 |
| Build | Jupyter Book 2 CLI | 把 MyST/Markdown 转换成网站 | 否 |
| Publish | Git | 下载并更新发布分支 | 否 |
| Publish | GitHub 账号 | 拥有仓库和 Pages 网站 | 是 |
| Publish | GitHub CLI（`gh`） | 让 LanCarbon 使用已登录的 GitHub 身份 | 是 |
| Publish | 可访问 GitHub 的网络 | 连接 GitHub API、Git HTTPS 和 Pages | — |

## 为什么 Build 需要 Python、Node.js 和 Jupyter Book

LanCarbon 会把软件内保存的 Book 转换成 Jupyter Book 2 项目。Python 负责运行 Jupyter Book 软件包，Node.js 负责运行其中的 MyST 引擎；两者共同完成项目检查和 HTML 网站生成。最简单的方法是使用 **Environment Setup**：对缺失项点击 **Install managed copy**；也可以直接安装 Jupyter Book 2，由 LanCarbon 自动准备缺失的受管理 Python 和 Node.js。希望手动安装到系统时，请使用 [Python 官网](https://www.python.org/downloads/)、[Node.js 下载页](https://nodejs.org/en/download/)和 [Jupyter Book 官方安装说明](https://jupyterbook.org/stable/get-started/install/)。常用的 Jupyter Book 命令为：

```powershell
python -m pip install "jupyter-book>=2,<3"
```

**Build** 窗口会检查 Python、Node.js 和 Jupyter Book CLI，并显示检测到的版本。受管理副本不需要修改系统 PATH；手动安装系统版本后，请重启 LanCarbon，使软件重新读取系统命令路径。

## 为什么 Publish 需要 Git、GitHub 与 GitHub CLI

Git 负责记录并传输一组网站文件；GitHub 用仓库存放这些文件；GitHub Pages 把仓库中的指定分支作为网站提供；GitHub CLI 让 LanCarbon 使用已经登录的 GitHub 账号，而不需要在 LanCarbon 中保存密码。

- 从 [Git for Windows 官方页面](https://git-scm.com/install/windows)安装 Git。
- 在 [github.com](https://github.com/)创建个人账号。
- 从 [GitHub CLI 官方页面](https://cli.github.com/)安装 GitHub CLI。
- 账号认证会在后面的 LanCarbon Publish 窗口中完成。

GitHub Desktop 是可选工具，不能替代 LanCarbon 所检查的 Git 和 GitHub CLI。

## 网络说明

写作和大多数本地 Build 不需要连接 GitHub。登录账号、创建或检查仓库、下载发布分支、发布网站和打开公开 Pages 网站都需要能够访问 GitHub。如果所在网络需要代理，仅对浏览器生效的代理可能无法覆盖 Git 或 GitHub CLI。请先开启代理软件的 **系统/全局代理** 或 **TUN 模式**，再重试相关检查。
