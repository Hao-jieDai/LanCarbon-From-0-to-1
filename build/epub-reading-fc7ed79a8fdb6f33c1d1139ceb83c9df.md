---
title: Reading EPUB and Switching Files
short_title: EPUB and File Tabs
keywords:
  - EPUB
  - Reading
  - Tabs
label: lc-s6-epub
---

# EPUB Reading and File Tabs

Open an EPUB in Library with **Open** or a double-click, or open its attachment from Note/Book **Preview** or **Resources → Read EPUB**. The reader uses local EPUB 2/3 chapters and navigation, with selectable text, embedded images and tables. **Contents** jumps to chapters or headings; previous/next buttons switch chapters. **Find in EPUB** (Ctrl+F) searches the book and lists up to 250 matches. Font size, line spacing and reading width are adjustable. Reading follows LanCarbon's theme and common text layout; publisher-specific styles, scripts, audio/video, external resources, DRM and fixed-layout publications are not supported. Unsupported books can use **Open externally**.

Enable **Translate** (Ctrl+Alt+T) to translate selected English using the existing translation configuration and Usage records. Reading itself is offline and does not call AI. Chapter, scroll position and typography are saved by stable document ID in **Data/Library/epub-reading.json**, shared by Library and linked Note/Book attachments. Rename/move and restart preserve progress. A newer external version offers **Reload latest version**. The file remains unchanged; no extracted-book cache is written to disk.

PDFs and EPUBs share a top tab bar with up to **10 files**. Opening the same document from another location activates its existing tab. Select a tab to return to its saved position; the active tab scrolls into view. **Workspace** returns to writing or Library without closing the tabs. The **×** on a tab closes only that file; closing the active tab selects a neighboring one. At the limit, close a tab before opening another. Arrow keys, Home and End switch tabs when a tab has keyboard focus. Tabs and the active file are restored after restart; only the active document body is loaded.


The reader uses two toolbar rows: file tabs and the sidebar toggle at the top, followed by reading controls. **Open externally** is beside the search box. The file name appears in its tab; **Workspace** returns to the previous writing or Library view while keeping file tabs open. When files are open, the sidebar toggle stays at the left of the tab row, including when the tabs are scrolled.

---

# EPUB 阅读与文件标签

在 Library 中点击 **Open** 或双击 EPUB，或从 Note／Book 的 **Preview** 附件和 **Resources → Read EPUB** 打开。阅读器在本地读取 EPUB 2／3 的章节和目录，支持选取文字、内嵌图片与表格。**Contents** 跳转章节或标题，前后按钮切换章节；**Find in EPUB**（Ctrl+F）搜索全书并列出最多 250 条匹配。可调整字号、行距和阅读宽度。正文采用 LanCarbon 主题和统一文字排版；不支持出版物专用样式、脚本、音视频、外部资源、DRM 和固定版式书籍。无法内置阅读的书籍可使用 **Open externally**。

开启 **Translate**（Ctrl+Alt+T）后，选取英文即可沿用翻译配置与 Usage 统计。阅读本身离线运行，不调用 AI。章节、滚动位置和文字样式按稳定文档 ID 保存在 **Data/Library/epub-reading.json**，Library 与 Note／Book 的关联附件共用；改名、移动或重启后保留进度。外部保存新版后提供 **Reload latest version**。阅读不修改原件，不在磁盘建立解压后的书籍缓存。

PDF 与 EPUB 共用顶部标签栏，最多同时打开 **10 个文件**。从不同位置打开同一文献会切换到已有标签；切换后恢复各自位置，当前标签会自动滚动到可见处。**Workspace** 返回写作／Library，同时保留文件标签；标签上的 **×** 只关闭该文件，关闭当前标签后切换到相邻文件。达到上限后需先关闭一个标签。标签获得键盘焦点时，可用方向键、Home、End 切换。重启后恢复标签和当前文件，正文只加载当前文件。


阅读区使用两行工具栏：上方为文件标签和侧栏开关，下方为阅读操作；**Open externally** 位于搜索框左侧。文件名只在标签中显示，点击 **Workspace** 返回先前的写作或 Library 页面并保留文件标签。打开文件后，侧栏开关固定在标签行左侧，横向滚动标签时仍可操作。
