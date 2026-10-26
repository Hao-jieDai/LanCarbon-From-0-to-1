---
title: Importing and Managing Library Files
short_title: Importing and Managing Library Files
description: Importing and Managing Library Files
authors:
  - name: Haojie Dai
keywords:
  - LanCarbon
label: lc-s6-library
---

# Importing and Managing Library Files

## Imports and Assets

Open **Library**. **Imports** contains PDF and EPUB documents you bring into your collection. **Source materials** shows managed images and attachments used by Notes and Books; their files are stored in **Library/assets**. An imported document can also be referenced in writing without creating another copy in assets.

Importing a document does not insert a link into a Note and does not send its contents to an AI service. These are separate actions.

## Importing documents and creating folders

1. Select **Imports** and the destination folder.
2. Choose **Import PDF / EPUB**, or drop files into the Library area. A batch accepts up to 20 files, each no larger than 100 MB.
3. Check the import report. Use **Locate** if a file already exists.
4. Use **New folder** to organize Imports into topics. Choose a folder in the sidebar to view its contents; use **All files** or search when you do not remember its location.

Select a folder to rename or delete it. **Delete folder** moves its files and subfolders to the parent folder; it does not delete those files. Use file deletion when you intend to remove the documents themselves.

## Duplicate files and naming conflicts

| Situation | What happens |
| --- | --- |
| Same contents, same or different filename | The existing document is reused. Exact file contents, including retained versions, determine a match. |
| Import a.pdf, rename it b.pdf, then import the same a.pdf | The report points to b.pdf; its current name is retained. |
| Same filename, different contents in one folder | The incoming file receives an available numbered name. Existing contents are not overwritten. |
| Same filename in different folders | Both names can be kept in their respective folders. |
| Rename or move would conflict | LanCarbon shows the conflict and an available name; confirm the alternative or cancel. |

Two visually identical PDFs can still have different file contents and be imported separately. Re-importing an older retained version does not replace the current version.

## File management and batch operations

Select a file to see its information and the Notes or Book pages referencing it. Click a reference to return to that page and location. **Rename** changes the name while keeping its extension and links. **Move** places an imported document in another Imports folder. **Folder** opens its location; **Save a copy** exports a separate file.

Choose **Batch select** to display checkboxes. Select individual files or **Select visible**, then choose **Move selected**, **Export selected** or **Delete selected**. **Exit selection** returns to the ordinary list. Changing a folder or filter clears the current selection. Built-in tutorial resources are protected.

Moving preserves references and reading positions. Exporting leaves the originals unchanged and avoids overwriting same-named files at the destination. File deletion is permanent. Check the confirmation for affected Notes and Books, and keep a [backup](../01-getting-started/recovery.md) of material you may need to restore. It removes the managed file and its retained versions and can remove its writing references. Deleting a folder and deleting its files are different actions.

## Document references in Notes and Books

In a Note or Book page, choose **Attach file**. The file chooser starts in Library. Selecting an imported original creates a stable reference to it rather than another copy in assets. Later renaming, moving or updating that document keeps the reference connected to its current contents.

Removing a link from the Markdown text does not delete the original. Removing a linked resource through **Resources** can remove its writing references while retaining the Imports original. Deleting the original through Library removes the original and its linked resources after confirmation.

## External editing and file versions

Use **Open externally** for a PDF or EPUB, or open an ordinary resource such as an image, TXT or Word file with its default application. LanCarbon prepares an editable working copy. Save changes to that opened copy; while LanCarbon is running, the changed contents become a new version. Changes are also checked on the next launch. Unchanged saves do not create versions.

Use **Versions** to inspect revisions and **Save version** to export an earlier copy. Choosing Save As in the external application creates a separate file that needs importing if you want it in Library.

Prefer LanCarbon's controls for managed files. Folder and file moves or renames within Imports are checked when returning to Library and on startup, and are reconciled where the original can be identified. External deletion leaves a missing-file entry so references are not silently erased. Directly overwriting a managed original is not the supported editing route; use **Open externally** for version tracking.

---

# 导入与管理 Library 资料

## Imports 与 Assets

打开 **Library**。**Imports** 保存导入资料库的 PDF 和 EPUB；**Source materials** 显示 Notes 和 Books 使用的受管理图片与附件，其文件保存在 **Library/assets**。已导入的文档也可以用于写作引用，不必再向 assets 复制一份。

导入文档不会自动在 Note 中插入链接，也不会把内容发送给 AI 服务。这些操作彼此独立。

## 导入文档与创建文件夹

1. 选择 **Imports** 和目标文件夹。
2. 点击 **Import PDF / EPUB**，或将文件拖入 Library 区域。每批最多导入 20 个文件，单个文件不超过 100 MB。
3. 查看导入报告。文件已存在时，可以点击 **Locate** 找到它。
4. 使用 **New folder** 按主题建立子文件夹。点击侧栏文件夹查看内容；不确定位置时，使用 **All files** 或搜索。

选择文件夹后可以重命名或删除。**Delete folder** 会把其中的文件和子文件夹移到上一级，不会删除这些文件。需要移除文档本身时，应使用文件删除操作。

## 重复文件与重名规则

| 情形 | 处理方式 |
| --- | --- |
| 内容相同，文件名相同或不同 | 复用已有文档。判断依据是精确的文件内容，也会检查保留的历史版本。 |
| 导入 a.pdf，改名为 b.pdf，再导入相同的 a.pdf | 报告指向 b.pdf，保留现有名称。 |
| 同一文件夹中名称相同、内容不同 | 为新文件生成可用的编号名称，不覆盖已有内容。 |
| 不同文件夹中名称相同 | 可以分别保留各自的名称。 |
| 重命名或移动造成冲突 | 显示冲突与可用名称，由你确认替代名称或取消。 |

两份 PDF 即使看起来相同，实际文件内容也可能不同，因此仍可能分别导入。重新导入已有历史版本不会替换当前版本。

## 文件管理与批量操作

选择文件后，可以查看资料信息以及引用它的 Notes 或 Book 页面。点击引用位置可跳回对应页面。**Rename** 修改名称并保留扩展名与引用；**Move** 将导入文档移到其他 Imports 文件夹；**Folder** 打开所在位置；**Save a copy** 导出独立副本。

点击 **Batch select** 后出现选择框。勾选文件或使用 **Select visible**，然后选择 **Move selected**、**Export selected** 或 **Delete selected**。**Exit selection** 返回普通列表。切换文件夹或筛选条件会清空选择。系统教程资源受保护，不参与批量选择。

移动会保留引用与阅读位置。导出不改变原件，也不会覆盖目标位置的同名文件。文件删除是永久操作。请先查看确认框中受影响的 Notes 和 Books；可能需要恢复的资料应提前[备份](../01-getting-started/recovery.md)。它会移除受管理文件及历史版本，并可清理相应写作引用。删除文件夹与删除文件不是同一操作。

## Notes 和 Books 中的文档引用

在 Note 或 Book 页面点击 **Attach file**，文件选择器默认从 Library 打开。选择已导入原件后，会建立稳定引用，不向 assets 再复制一份。以后重命名、移动或更新文档，引用仍指向其当前内容。

只删除 Markdown 中的链接不会删除原件。通过 **Resources** 移除关联资源时，可以清理写作引用并保留 Imports 原件；通过 Library 删除原件，则会在确认后删除原件及关联资源。

## 外部编辑与文件版本

PDF 和 EPUB 可以使用 **Open externally**；图片、TXT、Word 等普通资源可以用系统默认软件打开。LanCarbon 会准备可编辑的工作副本。请保存到打开的这个副本：软件运行期间，内容变化会登记为新版本；下次启动也会检查变化。内容未变化的保存不会增加版本。

通过 **Versions** 查看历史版本，通过 **Save version** 导出旧副本。在外部软件中使用“另存为”会产生独立文件，需要再次导入才能加入 Library。

管理文件时优先使用 LanCarbon 内的操作。Imports 内通过文件资源管理器完成的改名、移动，会在返回 Library 或启动时检查，并在能够识别原文件时同步。外部删除会保留缺失条目，以免悄悄丢失引用。直接覆盖受管理原件不是推荐的编辑方式，需要版本记录时请使用 **Open externally**。
