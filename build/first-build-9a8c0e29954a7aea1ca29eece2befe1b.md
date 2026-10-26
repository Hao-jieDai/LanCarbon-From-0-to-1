---
title: Your First Local Build
short_title: Your First Local Build
description: Bilingual LanCarbon beginner tutorial.
authors:
  - name: Haojie Dai
keywords:
  - LanCarbon
  - Jupyter Book
  - MyST
label: lc-s3-first
---


# Your First Local Build

![Build window before the first build](../assets/f7eed15a28d36a5313c9eff18be9bb2ad2d90cccd08c91d359d5e526ac4b3c2f.png)

1. Save the current page and select **Build** in the sidebar.
2. Confirm that Python and Jupyter Book CLI show check marks.
3. Read every preflight error or warning. Correct errors and reopen Build if needed.
4. Select **Choose Location and Build**.
5. Choose a parent folder where LanCarbon may create and manage a Book-specific build folder. Do not choose Data Location.
6. Wait for completion without closing LanCarbon.

The first window contains:

- Environment cards for Python and Jupyter Book CLI.
- Error/warning count and completion state of preflight.
- A detailed issue area, or **Preflight passed** when no issue is found.
- **Close**, which leaves without Building.
- **Choose Location and Build**, enabled only when required checks pass.

During Build, the application generates a temporary source, invokes the official CLI, and replaces the saved website only after success. A failed attempt leaves the previous successful website intact.

When the Build finishes, open the local website and inspect the home page, table of contents, every new page, images, downloads, citations, equations, and links. This is the closest local representation of what will be published.

---



# 第一次本地 Build

![第一次构建前的 Build 窗口](../assets/f7eed15a28d36a5313c9eff18be9bb2ad2d90cccd08c91d359d5e526ac4b3c2f.png)

1. 保存当前页面，然后点击侧边栏的 **Build**。
2. 确认 Python 和 Jupyter Book CLI 均显示通过标记。
3. 阅读所有 preflight error 或 warning。有错误时先修复，再重新打开 Build。
4. 点击 **Choose Location and Build**。
5. 选择一个允许 LanCarbon 创建并管理 Book 专属构建目录的上级文件夹。不要选择 Data Location。
6. 等待完成，期间不要关闭 LanCarbon。

首次窗口包含：

- Python 与 Jupyter Book CLI 环境卡片。
- Preflight 的 error/warning 数量和完成状态。
- 详细问题区域；没有问题时显示 **Preflight passed**。
- **Close**：直接关闭，不执行 Build。
- **Choose Location and Build**：只有必要检查通过后才可使用。

Build 期间，软件会生成临时源项目、调用官方 CLI，并且只在成功后替换保存的网站。失败时，上一次成功网站仍会保留。

Build 完成后，打开本地网站，检查首页、目录、新增页面、图片、附件下载、引用、公式和链接。这是发布前最接近在线效果的本地版本。
