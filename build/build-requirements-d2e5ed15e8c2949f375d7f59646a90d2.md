---
title: Preparing the Build Environment
short_title: Preparing the Build Environment
description: Bilingual LanCarbon beginner tutorial.
authors:
  - name: Haojie Dai
keywords:
  - LanCarbon
  - Jupyter Book
  - MyST
label: lc-s3-prepare
---


# Preparing the Build Environment

Open **Build**. The top cards check:

- **Python**: a working Python 3 command and its version.
- **Jupyter Book CLI**: a working Jupyter Book version 2 command and its version.

Both cards must pass. If Python is missing, install it from [python.org](https://www.python.org/downloads/). If Jupyter Book is missing or version 1 is found, follow the [Jupyter Book 2 installation guide](https://jupyterbook.org/stable/get-started/install/). Restart LanCarbon afterward.

The preflight summary reports errors and warnings. Errors block the Build because the output would be incomplete or ambiguous. Warnings deserve review but may allow the Build to continue. Select an issue to locate the page when the interface offers that action.

Common preflight problems include duplicate export paths or labels, missing pages, broken local links, missing or damaged managed Resources, malformed image/directive syntax, and invalid Book metadata.

Network access is normally unnecessary for the bundled website theme and local content. Remote images, remote includes, third-party plugins, or package installation can still require internet access. Prefer managed local Resources when you want a reproducible offline Build.

---



# 准备 Build 环境

打开 **Build**。顶部卡片会检查：

- **Python**：可以运行的 Python 3 命令及版本。
- **Jupyter Book CLI**：可以运行的 Jupyter Book 2 命令及版本。

两项都必须通过。Python 缺失时，从 [python.org](https://www.python.org/downloads/)安装；Jupyter Book 缺失或检测到版本 1 时，按照 [Jupyter Book 2 安装说明](https://jupyterbook.org/stable/get-started/install/)处理。安装后重启 LanCarbon。

Preflight 汇总会显示 errors 和 warnings。Error 会阻止 Build，因为结果可能不完整或存在歧义。Warning 需要检查，但可能仍允许继续。界面提供定位操作时，可以点击问题跳转到对应页面。

常见 preflight 问题包括：Export Path 或 Label 重复、页面缺失、本地链接失效、受管理资源缺失或损坏、图片/Directive 语法不完整，以及 Book 元数据无效。

使用软件内置网站主题和本地内容时，通常不需要网络。远程图片、远程 include、第三方插件或安装软件包仍可能要求联网。希望离线稳定 Build 时，优先使用受管理的本地 Resources。
