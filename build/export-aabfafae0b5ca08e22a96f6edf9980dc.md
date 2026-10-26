---
title: Exporting Source Copies and Page PDFs
short_title: Exporting Source Copies and Page PDFs
description: Bilingual LanCarbon beginner tutorial.
authors:
  - name: Haojie Dai
keywords:
  - LanCarbon
  - Jupyter Book
  - MyST
label: lc-s2-export
---


# Exporting Source Copies and Page PDFs

**Export** creates a separate Jupyter Book source project for backup, inspection, or external editing. It is optional. Build reads the current Book directly from LanCarbon, so the normal update path does not require Export.

## Export safely

1. Wait for **All changes saved**.
2. Select **Export**.
3. Choose a new, empty folder.
4. Wait for the success message, then inspect the folder.

LanCarbon requires an empty destination because it must not overwrite files that you may have edited externally. If the folder is not empty, create another folder or move its existing contents yourself after checking them.

The exported project normally contains Markdown pages, a `myst.yml` configuration, required managed resources under `assets/`, and supporting theme files. Only Resources referenced by this Book are included. Nested page links are adjusted for their exported locations.

## Export the current page as PDF

Select **Export PDF** in the page header from Edit or Preview, choose a filename and destination (default: the page title), and save. The default PDF destination is the **PDFs** folder beside Exports under the LanCarbon root. Installation or startup creates it automatically; you can still choose another destination. Exports remains for Book source copies, and existing PDFs are not moved. Export saves the latest edits first and needs no optional tools. It uses a white reading layout without editor controls or line numbers. Book home pages, Sections and Child Pages are exported individually. Links to omitted Book pages and attachments remain readable labels, not embedded content. Preview limitations also apply to PDF; check export notices and inspect the result. Existing PDFs require overwrite confirmation; canceling or a failed export leaves the previous file intact. The sidebar **Export** still creates the entire Book source copy.

PDF export supports Markdown Book home pages, Sections and Child Pages, but does not include descendants or other pages. It preserves supported math, managed images and tables, with A4 page numbers. Same-page references and external web links remain clickable. Missing or damaged managed resources must be repaired before export. Application themes do not change the white PDF background.

## Keep the roles separate

| Copy | Owner | Used by Build? | Safe expectation |
|---|---|---:|---|
| Book inside LanCarbon | LanCarbon | Yes | Continue editing here for the normal workflow. |
| Exported source folder | You | No | A separate snapshot that LanCarbon will not silently overwrite. |
| Build folder | LanCarbon workflow | Yes, as generated output | Choose once; rebuilds replace the managed website safely. |

Editing only the exported files does not update the Book stored in LanCarbon. If external changes matter, copy them back into the corresponding LanCarbon pages manually.

---



# 导出源文件副本与页面 PDF

**Export** 会创建一份独立的 Jupyter Book 源项目，用于备份、检查或在外部编辑。它是可选操作。Build 会直接读取 LanCarbon 内当前 Book，因此正常更新流程不要求先 Export。

## 安全导出

1. 等待 **All changes saved**。
2. 点击 **Export**。
3. 选择一个新建的空文件夹。
4. 等待成功提示，然后检查文件夹内容。

LanCarbon 要求目标目录为空，是为了避免覆盖你可能已经在外部修改的文件。如果目录不为空，请新建另一个目录，或在自行检查后移动现有内容。

导出的项目通常包含 Markdown 页面、`myst.yml` 配置、`assets/` 下当前 Book 所需的受管理资源，以及主题支持文件。只会导出这本 Book 实际引用的 Resources；嵌套页面的链接会根据导出位置自动调整。

## 将当前页面导出为 PDF

在 Edit 或 Preview 中点击页面顶部的 **Export PDF**，选择文件名和保存位置（默认为页面标题），然后保存。PDF 默认保存位置为 LanCarbon 根目录下与 Exports 同级的 **PDFs** 文件夹，安装或启动时会自动创建；仍可自行选择其他保存位置。Exports 继续用于 Book 源文件副本，已有 PDF 不会自动搬移。导出前会先保存最新修改，不需要额外工具。PDF 使用白底阅读排版，不包含编辑工具栏和行号。Book 首页、Section 和 Child Page 均可单独导出。指向未导出 Book 页面的链接和附件保留为可读文字，不会嵌入目标内容。Preview 的支持范围同样适用于 PDF，请检查导出后的注意事项和生成结果。覆盖已有 PDF 需要确认；取消或导出失败不会破坏原有文件。侧边栏的 **Export** 仍用于导出整本 Book 的源文件副本。

PDF 可导出 Markdown Book 首页、Section 和 Child Page，但不包含其子页面或其他页面；保留受支持公式、受管理图片和表格，并添加 A4 页码。当前页面内部引用和外部网页链接仍可点击；缺失或损坏的受管理资源需要修复后才能导出。软件主题不会改变 PDF 的白底。

## 分清三种副本

| 副本 | 管理者 | Build 是否使用 | 正确理解 |
|---|---|---:|---|
| LanCarbon 内的 Book | LanCarbon | 是 | 正常流程中继续在这里编辑。 |
| 导出的源文件夹 | 用户 | 否 | 独立快照，LanCarbon 不会悄悄覆盖。 |
| Build 文件夹 | LanCarbon 工作流 | 是，作为生成结果 | 第一次选择；后续 rebuild 会安全替换受管理网站。 |

只修改导出文件不会更新 LanCarbon 中保存的 Book。如果外部修改需要保留，请手动复制回对应的 LanCarbon 页面。
