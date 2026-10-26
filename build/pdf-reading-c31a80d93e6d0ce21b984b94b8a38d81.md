---
title: Reading PDF Documents
short_title: Reading PDFs
keywords:
  - PDF
  - Reading
label: lc-s6-pdf
---

# Reading PDFs

Open a PDF from Library with **Open** or a double-click. In a Note or Book, click its attachment in **Preview**, or use **Resources → Read PDF**. **Workspace** in the tab bar returns to the original writing or Library view. **Open externally** retains default-app editing and file versions; Other ordinary files use their default apps.

Use page numbers, previous/next, **Fit width**, **Fit page**, zoom, or **Pages / Contents** for on-demand thumbnails and the document's own outline. **Find in PDF** (Ctrl+F) searches the document with previous/next matches. Reading position and zoom are saved by document ID in **Data/Library/reading.json**, so rename/move and linked writing attachments share progress. The currently open PDF is an immutable reading snapshot; a new externally saved version offers **Reload latest version**.

Enable the existing **Translate** switch (Ctrl+Alt+T), then select short English text in the PDF. Existing translation settings, cache and usage accounting apply. Scanned pages use local English/Chinese OCR. The OCR menu provides Recognize page, Recognize PDF and Stop OCR; recognized text supports selection, search and existing translation. Reading is local and does not call AI or change the file. Password-protected files prompt locally without saving the password. PDF scripts and editing are disabled. Annotation creation remains separate. The reader loads page data as needed and releases the open snapshot when closed; recognized text and coordinates are cached up to 64 MB; temporary page images and thumbnails are not saved to disk.

---

# PDF 阅读

在 Library 中点击 **Open** 或双击 PDF。在 Note／Book 的 **Preview** 点击 PDF 附件，或通过 **Resources → Read PDF** 打开；标签栏的 **Workspace** 返回原来的写作或文件列表。**Open externally** 保留默认程序编辑和文件版本功能，其他普通文件继续使用默认程序。

使用页码、前后翻页、**Fit width**、**Fit page**、缩放，以及 **Pages / Contents** 中按需生成的缩略图和原文目录。**Find in PDF**（Ctrl+F）提供全文搜索与前后匹配。阅读位置和缩放按文档 ID 保存在 **Data/Library/reading.json**；改名、移动及写作附件共用进度。正在阅读的内容保持为打开时的版本，外部保存新版后，可选择 **Reload latest version**。

开启现有 **Translate**（Ctrl+Alt+T），选取 PDF 中的短英文即可翻译，沿用翻译配置、缓存和用量统计。扫描页使用本地中英文 OCR；OCR 菜单提供 Recognize page、Recognize PDF 和 Stop OCR，识别文字支持选词、搜索及现有翻译。阅读本身离线运行，不调用 AI、不修改原件。加密文件在本地输入密码，密码不保存；禁用 PDF 脚本和编辑。新建批注另行提供。页面按需读取，关闭后释放打开快照，识别文字与坐标缓存最多 64 MB，不长期保存整页图片或缩略图。

