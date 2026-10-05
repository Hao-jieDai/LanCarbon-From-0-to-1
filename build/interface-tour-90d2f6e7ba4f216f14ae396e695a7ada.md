---
title: Touring the LanCarbon Interface
short_title: Touring the LanCarbon Interface
description: Bilingual LanCarbon beginner tutorial.
authors:
  - name: Haojie Dai
keywords:
  - LanCarbon
  - Jupyter Book
  - MyST
label: lc-s1-interface
---


# Touring the LanCarbon Interface

![LanCarbon main workspace](../assets/2de495e4aed7eca98ea1cfbe93ff676026cc958d049bcddb5065b40f0e00e4d9.png)

The main workspace has four areas.

## 1. Sidebar

- **Notes / Books** switches between independent notes and structured Books. Press **Ctrl+Q** to switch quickly while keeping the selected Note or Book page; a **Q** hint is embedded at the right of the Books tab, with **Ctrl+Q** shown on hover and does not switch workspaces while a dialog is open.
- **Sort by** orders the Notes list or Book selector by **Last modified**, **Date created** (newest first) or **Name (A–Z)**. Pinned Notes stay first. Notes and Books remember their sorting choices independently across restarts. A Book's last-modified time also includes edits to its pages; sorting the selector does not change the Book's table of contents or export order.
- The Book selector opens a different Book; the plus button creates one.
- **+ Section** creates a top-level organizing page. **+ Child Page** creates a page under the current selection.
- **Settings**, **Export**, **Build**, **Publish**, and **Delete** operate on the selected Book.
- The tree is the Book's table of contents. Select a title to edit it. Click the separate triangle before a page to expand or collapse its children. Each Book remembers its folded branches across restarts. Navigating to a page from Preview or Build checks, or creating a child, automatically reveals its ancestors.
- **Light / Dark** changes the application theme only.
- **Data Location** shows or moves the application data folder.

## 2. Page header

**All changes saved** confirms that the latest text is on disk. **Edit / Preview** switches between Markdown source and rendered reading view. Press **Ctrl+E** on Windows or **Cmd+E** on macOS to switch quickly. **Export PDF** saves only the current Note or Markdown Book page as an A4 PDF, without its children. The default PDF destination is the **PDFs** folder beside Exports under the LanCarbon root. Installation or startup creates it automatically; you can still choose another destination. Exports remains for Book source copies, and existing PDFs are not moved. **Page Properties** opens export and page metadata. **Remove from Book** keeps the Note but removes it from this Book. The pin and trash controls pin or delete the current item.

## 3. Writing tools and editor

The first toolbar row manages files and citations: **Insert image**, **Image settings**, **Attach file**, **Resources**, and **Citations**. Files can also be dropped or pasted into the editor.

The second row changes Markdown/MyST source: Undo, Redo, paragraph/heading, Bold, Italic, Underline, Strikethrough, superscript, subscript, alignment, abbreviation, keyboard key, lists, quote, link, code, table, math, thematic break, and directives. Most tools act on selected text; some insert a template at the cursor.

The editor shows line numbers and stores plain Markdown text. The tag box below the editor adds searchable Note tags. The bottom status area shows character and line counts and autosave state.

## 4. A useful habit

After a large edit, pause until **All changes saved** appears before closing the application, changing Data Location, or starting a Build.

---



# 认识 LanCarbon 主界面

![LanCarbon 主工作区](../assets/2de495e4aed7eca98ea1cfbe93ff676026cc958d049bcddb5065b40f0e00e4d9.png)

主界面可以分成四个区域。

## 1. 侧边栏

- **Notes / Books** 用于切换普通独立笔记和结构化 Book。按 **Ctrl+Q** 可以快速切换，并保留原来选中的 Note 或 Book 页面；Books 按钮内部右侧显示 **Q** 提示，悬停可查看 **Ctrl+Q**，打开对话框时不会切换工作区。
- **Sort by** 将 Notes 列表或 Book 下拉框按 **Last modified**（修改时间）、**Date created**（创建时间，时间均为最新在前）或 **Name (A–Z)**（名称）排序。置顶 Notes 始终优先；两个工作区分别记住排序选择，重启后仍保留。Book 修改时间也会计入其页面正文的修改；下拉框排序不会改变 Book 内部目录和导出顺序。
- Book 下拉框用于切换不同 Book，旁边的加号用于新建 Book。
- **+ Section** 新建顶层组织页面；**+ Child Page** 在当前所选项目下新建子页面。
- **Settings**、**Export**、**Build**、**Publish** 和 **Delete** 针对当前选中的 Book 操作。
- 下方树形目录就是 Book 的目录。点击标题开始编辑；点击页面前独立的三角形展开或折叠子页面。每本 Book 分别记住折叠状态，重启后仍保留；从 Preview 或 Build 检查跳转到页面，或新建子页面时，会自动展开其上级目录。
- **Light / Dark** 只改变软件界面主题。
- **Data Location** 用于查看或迁移软件数据目录。

## 2. 页面顶部

**All changes saved** 表示最新文字已经写入磁盘。**Edit / Preview** 在 Markdown 源文和阅读预览之间切换。在 Windows 上按 **Ctrl+E**，在 macOS 上按 **Cmd+E** 可以快速切换。**Export PDF** 将当前 Note 或 Markdown Book 页面保存为 A4 PDF，不包含子页面。PDF 默认保存位置为 LanCarbon 根目录下与 Exports 同级的 **PDFs** 文件夹，安装或启动时会自动创建；仍可自行选择其他保存位置。Exports 继续用于 Book 源文件副本，已有 PDF 不会自动搬移。 **Page Properties** 打开导出路径和页面元数据设置。**Remove from Book** 会把页面移出当前 Book，但保留对应 Note。图钉和垃圾桶分别用于置顶与删除当前项目。

## 3. 写作工具与编辑区

第一行工具负责文件和引用：**Insert image**、**Image settings**、**Attach file**、**Resources** 与 **Citations**。也可以把文件拖入编辑器，或直接粘贴截图。

第二行工具修改 Markdown/MyST 源文：撤销、重做、段落/标题、粗体、斜体、下划线、删除线、上标、下标、对齐、缩写、键盘按键、列表、引用、链接、代码、表格、数学公式、分隔线和 Directives。多数工具会作用于选中的文字，另一些会在光标位置插入模板。

编辑区带有行号，保存的是纯 Markdown 文本。下方标签框用于添加可搜索的 Note 标签。最底部状态区显示字符数、行数和自动保存状态。

## 4. 一个实用习惯

完成较大修改后，先等待 **All changes saved** 出现，再关闭软件、修改 Data Location 或开始 Build。
