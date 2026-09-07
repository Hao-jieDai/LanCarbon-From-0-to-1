---
title: Images, Attachments, Citations, and Resources
short_title: Images, Attachments, Citations, and Resources
description: Bilingual LanCarbon beginner tutorial.
authors:
  - name: Haojie Dai
keywords:
  - LanCarbon
  - Jupyter Book
  - MyST
label: lc-s2-resources
---


# Images, Attachments, Citations, and Resources

LanCarbon copies imported files into its managed data folder. This protects the Book from breaking when the original file is moved or deleted.

## First toolbar row

- **Insert image** chooses a PNG, JPEG, GIF, or WebP file and inserts a managed Markdown image reference.
- **Image settings** edits a selected managed image: width, left/center/right alignment, alternative description, and optional caption.
- **Attach file** imports a non-image file and inserts a download link.
- **Resources** lists every managed file and where it is used.
- **Citations** imports and manages bibliography data and inserts citation keys supported by the Book.
- Dropping a file or pasting a screenshot into the editor imports it through the same managed system.

Always write meaningful alternative text for informative images. Use a caption to explain why the figure matters; do not repeat all visible pixels.

## Resources panel

![Resources panel](../assets/3b9a49d527c5cd4a12abac80bdc4f4d72053f0ef9c8eb3b877e8631c80fcc866.png)

- **Find a resource** filters by filename.
- **Show resources** limits the list to all items, Notes, Books, one Book, or another available scope.
- **Select visible** selects the current filtered results for batch deletion.
- **Insert** places a reference to the resource at the editor cursor.
- **Save a copy** exports one managed file to a location you choose.
- **Delete** removes the managed file and, after confirmation, its references. Review every listed usage first.
- Expand the reference row to see all Notes and Book pages that use the item.

Removing Markdown text from one page does not delete the managed file. Deleting from Resources is global and can affect multiple Books.

## Citations

Import a valid bibliography file from **Citations**, then insert entries by citation key. Keep citation keys unique across all bibliography sources attached to one Book. Preview provides a writing check; Build uses the official Jupyter Book engine for final citations and bibliography output.

## Backups

A complete manual backup includes `notes.json`, `assets.json`, and the `assets` folder from Data Location. Copy them together while LanCarbon is closed.

---



# 图片、附件、引用与 Resources

LanCarbon 会把导入的文件复制到受管理的数据目录中。因此即使原始文件被移动或删除，Book 中的受管理副本仍然可以使用。

## 第一行工具栏

- **Insert image** 选择 PNG、JPEG、GIF 或 WebP 文件，并插入受管理的 Markdown 图片引用。
- **Image settings** 修改选中的受管理图片：宽度、左/中/右对齐、替代说明和可选 caption。
- **Attach file** 导入非图片文件并插入下载链接。
- **Resources** 列出所有受管理文件及其使用位置。
- **Citations** 导入和管理参考文献数据，并插入当前 Book 支持的引用键。
- 把文件拖入编辑器或粘贴截图，也会通过相同的受管理资源系统导入。

信息型图片应填写有意义的替代文字。Caption 用来说明这张图为什么重要，不必逐像素重复画面内容。

## Resources 面板

![Resources 面板](../assets/3b9a49d527c5cd4a12abac80bdc4f4d72053f0ef9c8eb3b877e8631c80fcc866.png)

- **Find a resource** 按文件名筛选。
- **Show resources** 把列表限制为全部、Notes、Books、某一本 Book 或其他可用范围。
- **Select visible** 选择当前筛选结果，用于批量删除。
- **Insert** 在编辑器光标处插入资源引用。
- **Save a copy** 把一个受管理文件导出到你选择的位置。
- **Delete** 删除受管理文件，并在确认后清除它的引用。操作前请检查列出的全部使用位置。
- 展开 references 行，可以查看使用该资源的全部 Notes 和 Book 页面。

只删除某一页中的 Markdown 引用，不会删除受管理文件。从 Resources 中删除则是全局操作，可能影响多本 Book。

## Citations

从 **Citations** 导入有效的参考文献文件，再按 citation key 插入条目。同一本 Book 关联的全部参考文献源中，引用键必须唯一。Preview 用于写作检查；Build 会使用官方 Jupyter Book 引擎生成最终引用和参考文献列表。

## 备份

完整手动备份应同时包含 Data Location 中的 `notes.json`、`assets.json` 和 `assets` 文件夹。请关闭 LanCarbon 后一起复制。
