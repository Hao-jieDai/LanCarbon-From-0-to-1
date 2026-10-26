---
title: Reading PDF and EPUB
short_title: Reading PDF and EPUB
description: Reading PDF and EPUB
authors:
  - name: Haojie Dai
keywords:
  - LanCarbon
label: lc-s6-pdf
---

# Reading PDF and EPUB

## Opening documents and switching tabs

In Library, double-click a PDF or EPUB, or choose **Open**. You can also open a linked document from a Note or Book's **Preview** or **Resources** panel. The same document shares its reading position across these entry points.

Up to **ten documents** can remain open in the top tab bar. Click a tab to switch, or its close button to release it. Opening the same document selects its existing tab. If ten tabs are already open, close one before opening another. **Workspace** returns to the previous writing or Library page without closing your tabs. The menu button at the left shows or hides the main sidebar.

## PDF navigation and search

Use the page number and previous/next controls to move through the document. **Pages / Contents** gives you thumbnails and the document's own outline, where available. **Fit width**, **Fit page** and zoom adapt the page to the reading area. **Find in PDF**, also available with **Ctrl+F**, searches readable text and moves between matches.

Select text to copy it or use translation. Reading position and zoom are remembered for the document. Renaming or moving it within Library keeps that identity. If an external edit produces a new version while the document is open, use **Reload latest version** when you are ready to read the changed contents.

## Text recognition in scanned PDFs

A scanned page is an image rather than selectable text. When an opened page has no usable text layer, LanCarbon recognizes English and Simplified Chinese locally. Use the **OCR** menu for additional control:

| Action | When to use it |
| --- | --- |
| **Recognize page** | Retry the current page, or replace an incorrect embedded text layer with recognition results for reading. |
| **Recognize PDF** | Prepare the document for search and selection, up to 500 pages. Readable embedded text and completed recognition results are reused. |
| **Stop OCR** | Stop the current reading task; completed pages remain available. |

After recognition, select or copy text and use **Find in PDF** as usual. To search an entire scanned document, recognize the PDF first: image text on unprocessed pages cannot yet be searched. Document questions also prepare selected scans automatically. If Chat prepared pages after the reader was opened, reopen the PDF or use **Recognize PDF** to refresh the text layer.

OCR resources are included with LanCarbon. Recognition needs no additional API Key and uses no model tokens. It does not rewrite your PDF. Recognition can misread numbers, tables, formulas or unusual layouts, so compare important details with the original page. It is text recognition, not a complete reconstruction of table or formula structure.

## EPUB navigation and display

Use **Contents** to choose a chapter or heading. Previous/next buttons switch chapters; **Find in EPUB** searches the book. Adjust font size, line spacing and reading width for comfortable reading. Text, images and tables use LanCarbon's reading theme.

The reader supports reflowable EPUB 2/3 documents. DRM, fixed-layout books, scripts, audio and video are not supported by this reader. Use **Open externally** if a book needs its original reader or publisher-specific presentation.

## Translation while reading

Configure translation once in [Translation Settings](../07-workshop/translation.md), then turn on **Translate** or press **Ctrl+Alt+T**. Selecting an English word, phrase or short passage displays its Chinese translation. The source and translation scroll separately inside the floating panel. Close the panel or turn off Translate when you want ordinary selection without translation requests.

## Opening files in external applications

**Open externally**, beside the reader's search field, uses the system's default application. This is also how ordinary resources such as images, TXT and Word files are opened. External edits are handled as described under [External editing and file versions](management.md).

---

# 阅读 PDF 与 EPUB

## 打开文档与切换文件

在 Library 中双击 PDF 或 EPUB，或点击 **Open**。也可以从 Note、Book 的 **Preview** 附件链接或 **Resources** 面板打开。不同入口打开的同一文档共用阅读进度。

顶部标签栏最多同时保留 **十个文档**。点击标签切换，点击关闭按钮关闭该文件。重复打开同一文档会转到已有标签；已有十个标签时，先关闭一个再打开新文件。**Workspace** 返回此前的写作或 Library 页面，不关闭标签。左侧菜单按钮用于展开或收起主侧栏。

## PDF 导航与搜索

使用页码和前后翻页按钮移动到目标页面。**Pages / Contents** 显示缩略图以及文档自身提供的目录。**Fit width**、**Fit page** 与缩放用于调整阅读大小。**Find in PDF** 或 **Ctrl+F** 搜索可读取的文字，并在匹配位置之间跳转。

选中文字后可以复制或翻译。软件会记住文档的阅读位置和缩放；在 Library 中改名、移动不会改变文档身份。阅读期间，如果外部编辑产生新版本，可以在需要时使用 **Reload latest version** 加载更新内容。

## 扫描 PDF 的文字识别

扫描页本质上是图片，不一定能直接选中文字。打开的页面没有可用文字层时，LanCarbon 会在本地识别英文和简体中文。**OCR** 菜单提供以下操作：

| 操作 | 适用情形 |
| --- | --- |
| **Recognize page** | 重新识别当前页，或用识别结果替代错误的内嵌文字层进行阅读。 |
| **Recognize PDF** | 为全篇搜索和选词准备文字，最多处理 500 页；复用可读的内嵌文字和已完成的识别结果。 |
| **Stop OCR** | 停止当前阅读识别任务，已完成页面仍可使用。 |

完成后可以像普通 PDF 一样选取、复制文字和使用 **Find in PDF**。搜索整份扫描文档前，先执行 Recognize PDF；尚未处理的图片文字还不能搜索。资料问答也会自动准备选定的扫描件。如果 Chat 在阅读器打开后识别了更多页面，可重新打开 PDF 或使用 Recognize PDF 刷新文字层。

OCR 识别资源随软件提供，不需要额外 API Key，也不消耗模型 tokens；识别不会改写 PDF 原件。数字、表格、公式或特殊版式可能识别不准，重要内容应对照原页。它提供文字识别，不保证完整还原表格和公式结构。

## EPUB 导航与显示

通过 **Contents** 选择章节或标题，前后按钮切换章节，**Find in EPUB** 搜索全书。可以调整字号、行距和阅读宽度。文字、图片和表格使用 LanCarbon 的阅读主题。

内置阅读器支持可重排的 EPUB 2／3，不支持 DRM、固定版式、脚本、音频和视频。需要专用阅读器或原出版社版式时，可使用 **Open externally**。

## 阅读时翻译

先在[翻译设置](../07-workshop/translation.md)完成一次配置，再开启 **Translate** 或按 **Ctrl+Alt+T**。选取英文单词、词组或短段落后，浮窗会显示中文；原文与译文分别滚动。只想普通选词时，关闭浮窗或 Translate，避免触发翻译请求。

## 使用外部软件

阅读器搜索框旁的 **Open externally** 使用系统默认程序。图片、TXT、Word 等普通资源也使用默认程序打开。外部修改的保存方式见[外部编辑与文件版本](management.md)。
