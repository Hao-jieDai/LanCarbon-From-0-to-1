---
title: What Build Means and How It Differs from Export
short_title: What Build Means and How It Differs from Export
description: Bilingual LanCarbon beginner tutorial.
authors:
  - name: Haojie Dai
keywords:
  - LanCarbon
  - Jupyter Book
  - MyST
label: lc-s3-meaning
---


# What Build Means and How It Differs from Export

Build has three jobs:

1. Check Book structure, paths, links, resources, and supported content.
2. Generate a managed Jupyter Book project from the current in-app Book.
3. Run the official engine and save a complete HTML website.

Build does **not** read your optional Export folder. After changing a page in LanCarbon, wait for it to save and select **Rebuild Website**. You do not need to delete old source files or Export again.

| Feature | Preview | Export | Build |
|---|---|---|---|
| Main purpose | Fast page check | Independent source copy | Complete local website |
| Source | Current page | Current Book | Current Book |
| Requires Python/Jupyter Book | No | No | Yes |
| Checks full navigation and official output | No | No | Yes |
| Required before Publish | Helpful | No | Yes |

The first successful Build asks where to store the managed result. Later Builds reuse that location. **Change Build Location** moves future managed output to another parent folder; it does not change Data Location or an Export folder.

Publish uses the latest successful Build only when it matches the current Book. If content has changed, the Publish workflow marks the build as outdated and asks for or performs a fresh rebuild.

---



# Build 的含义及其与 Export 的区别

Build 完成三项工作：

1. 检查 Book 结构、路径、链接、资源和受支持内容。
2. 从软件内当前 Book 生成一个受管理的 Jupyter Book 项目。
3. 运行官方引擎并保存完整 HTML 网站。

Build **不会**读取可选的 Export 文件夹。在 LanCarbon 中修改页面后，等待保存，然后点击 **Rebuild Website** 即可。不需要删除旧源文件，也不需要重新 Export。

| 功能 | Preview | Export | Build |
|---|---|---|---|
| 主要目的 | 快速检查单页 | 创建独立源文件副本 | 生成完整本地网站 |
| 内容来源 | 当前页 | 当前 Book | 当前 Book |
| 是否需要 Python/Jupyter Book | 否 | 否 | 是 |
| 是否检查完整导航和官方输出 | 否 | 否 | 是 |
| Publish 前是否需要 | 有帮助 | 否 | 是 |

第一次成功 Build 会要求选择受管理结果的保存位置。后续 Build 会继续使用该位置。**Change Build Location** 只改变以后生成内容的上级目录，不会修改 Data Location，也不会修改 Export 目录。

Publish 只会使用与当前 Book 一致的最新成功 Build。内容发生变化后，Publish 会把旧结果标为 outdated，并要求或执行新的 rebuild。
