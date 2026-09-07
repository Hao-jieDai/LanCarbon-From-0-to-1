---
title: Installing and Starting LanCarbon
short_title: Installing and Starting LanCarbon
description: Bilingual LanCarbon beginner tutorial.
authors:
  - name: Haojie Dai
keywords:
  - LanCarbon
  - Jupyter Book
  - MyST
label: lc-s1-install
---

## English

# Installing and Starting LanCarbon

## Before installation

Download LanCarbon only from the project page or another source identified by the maintainer. The Windows installer has a name similar to `LanCarbon-x.y.z-x64-Setup.exe`; `x.y.z` is the version number. Keep the installer until you have confirmed that the application starts correctly.

## Install and launch

1. Close any older LanCarbon window.
2. Run the installer and choose a destination. Installing over an older version is the normal upgrade method.
3. Start LanCarbon from the Start menu or the installation folder.
4. On first launch, wait for the main workspace to appear.
5. Select **Data Location** at the bottom of the sidebar and note the displayed folder.

LanCarbon stores Notes, Books, page order, Book settings, and managed Resources in that data location. Installing a new application version does not intentionally remove that folder. Before a major upgrade, copy the entire data folder to a safe backup location while LanCarbon is closed.

## What LanCarbon does

LanCarbon combines four tasks in one desktop interface:

- Write ordinary Notes or structured Books.
- Author Markdown and MyST with toolbar assistance.
- Build a Book into a local Jupyter Book website.
- Publish and later update that website through GitHub Pages.

LanCarbon works locally for writing. An account is not required until you publish. The current workflow is designed for Markdown/MyST pages; executable notebook editing and execution are outside this version's main workflow.

## Safe first-launch check

Create a temporary Note, type one sentence, wait for **All changes saved**, close LanCarbon, and reopen it. If the sentence remains, local saving works. Delete the temporary Note afterward.

---

## 中文

# 安装并首次启动 LanCarbon

## 安装前

请只从项目主页或开发者明确提供的位置下载 LanCarbon。Windows 安装包名称类似 `LanCarbon-x.y.z-x64-Setup.exe`，其中 `x.y.z` 是版本号。在确认软件能够正常启动前，建议保留安装包。

## 安装与启动

1. 关闭所有旧版本 LanCarbon 窗口。
2. 运行安装包并选择安装位置。升级时直接覆盖旧版本是正常方式。
3. 从开始菜单或安装目录启动 LanCarbon。
4. 第一次启动时，等待主工作区完整显示。
5. 点击侧边栏底部的 **Data Location**，记下显示的数据目录。

LanCarbon 会在 Data Location 中保存 Notes、Books、页面顺序、Book 设置和受管理的 Resources。安装新版软件不会主动删除这个目录。进行重要升级前，请先关闭 LanCarbon，再把整个数据目录复制到安全位置作为备份。

## LanCarbon 能做什么

LanCarbon 在一个桌面界面中整合了四项工作：

- 撰写普通 Notes 或具有目录结构的 Books。
- 借助工具栏撰写 Markdown 和 MyST。
- 把 Book 构建成本地 Jupyter Book 网站。
- 通过 GitHub Pages 在线发布，并在以后更新网站。

写作本身完全在本地完成，不需要账号。只有 Publish 时才需要 GitHub。当前主要工作流面向 Markdown/MyST 页面；可执行 Notebook 的编辑与运行不属于这一版本的主要范围。

## 安全的首次启动检查

新建一篇临时 Note，输入一句话，等待顶部显示 **All changes saved**，关闭再重新打开 LanCarbon。如果句子仍然存在，说明本地保存正常。检查完成后可以删除这篇临时 Note。
