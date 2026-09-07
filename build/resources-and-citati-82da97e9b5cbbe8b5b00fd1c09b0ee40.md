---
title: Add Images, Attachments, and Citations
short_title: Resources and Citations
description: Hands-on practice with the resource toolbar and citation workflow.
authors:
  - name: Haojie Dai
keywords:
  - LanCarbon
  - sample Book
  - beginner
  - tutorial
label: lc-s5-resources
---


# Add Images, Attachments, and Citations

Use the sample Book's `Resources and Sources` page for this exercise. The first toolbar row manages files; imported files become managed copies inside LanCarbon.

## Insert an image

1. Choose a small `.png` or `.jpg` that you are allowed to use.
2. Select **Insert image**, choose the file, and confirm that Markdown appears at the cursor.
3. Select **Image settings** while the cursor is in the image syntax.
4. Enter meaningful alternative text such as `A small plant beside a window`.
5. Add a short caption, choose an alignment, and apply.
6. Switch to Preview and confirm the image, caption, and alignment.

You can also drag an image into the editor or paste a screenshot. Test this only with a disposable image so duplicate resources are easy to identify and remove.

The image below demonstrates how a managed screenshot appears in this tutorial:

![LanCarbon workspace used as a managed image example](../assets/2de495e4aed7eca98ea1cfbe93ff676026cc958d049bcddb5065b40f0e00e4d9.png)

## Attach a file

1. Create a small text file named `observation-data.txt` containing one or two sample lines.
2. Select **Attach file** and choose it.
3. Confirm that a download link is inserted.
4. In Preview, select the link and save a copy when prompted.

Do not attach passwords, private data, or large files to a Book that may be published.

## Inspect Resources

Open **Resources** and verify:

- the image is listed as an Image;
- the text file is listed as an Attachment;
- each item shows where it is referenced;
- **Insert** adds another reference at the cursor;
- **Save a copy** creates a user-selected copy without removing the managed resource;
- deleting a Markdown link alone keeps the managed file;
- **Delete** permanently removes the managed copy and its references, so use it only for a disposable test resource.

## Add a citation

Create a plain-text file named `sample-references.bib` with this BibTeX record:

```bibtex
@article{example2026,
  author = {Example Author},
  title = {A Beginner Example for Source Practice},
  journal = {Learning Notes},
  year = {2026}
}
```

Open **Citations**, import the bibliography file, and insert the `example2026` entry using the panel. The inserted source should resemble narrative `@example2026` or parenthetical `[@example2026]` citation syntax. Do not type an unregistered key: Preview and preflight should report it as missing.

Add a bibliography block at the end if the citation panel or current workflow provides it, then verify the citation and bibliography in Preview and again on the built website.

:::{caution}
This record is deliberately fictional and is only a software exercise. Replace it with real bibliographic data before publishing factual work.
:::

## First-row toolbar acceptance

- [ ] Insert image works.
- [ ] Drag or paste image works, if tested.
- [ ] Image settings preserves the image and applies alt text/caption/alignment.
- [ ] Attach file creates a working managed download.
- [ ] Resources search, filtering, references, Insert, and Save a copy work.
- [ ] Citations imports the `.bib` record and inserts a registered key.
- [ ] Preview and Build report no missing managed resources or citation keys.

---



# 添加图片、附件与引用文献

请在样例 Book 的 `Resources and Sources` 页面完成本练习。第一行工具栏负责文件管理；导入后的文件会成为 LanCarbon 内部的受管理副本。

## 插入图片

1. 选择一张你有权使用的小型 `.png` 或 `.jpg` 图片。
2. 点击 **Insert image**，选择文件，确认 Markdown 已插入光标位置。
3. 把光标放在图片语法内，点击 **Image settings**。
4. 填写有意义的替代文字，例如 `A small plant beside a window`。
5. 添加短 caption，选择对齐方式并应用。
6. 切换到 Preview，检查图片、caption 与对齐。

也可以把图片拖入编辑器或粘贴截图。建议只用临时图片测试，这样容易识别并删除重复资源。

下图演示本教程中受管理截图的显示效果：

![作为受管理图片示例的 LanCarbon 工作区](../assets/2de495e4aed7eca98ea1cfbe93ff676026cc958d049bcddb5065b40f0e00e4d9.png)

## 添加附件

1. 创建一个小型文本文件 `observation-data.txt`，写入一两行样例内容。
2. 点击 **Attach file** 并选择它。
3. 确认正文中插入了下载链接。
4. 在 Preview 中点击该链接，并按提示保存副本。

准备公开发布的 Book 不应附带密码、隐私数据或过大的文件。

## 检查 Resources

打开 **Resources** 并确认：

- 图片被列为 Image；
- 文本文件被列为 Attachment；
- 每项资源能显示其引用位置；
- **Insert** 可在光标处再插入一次引用；
- **Save a copy** 可另存用户副本，不会删除受管理资源；
- 只删除正文 Markdown 链接不会删除受管理文件；
- **Delete** 会永久删除受管理副本及其引用，只能用于可丢弃的测试资源。

## 添加引用文献

创建纯文本文件 `sample-references.bib`，内容如下：

```bibtex
@article{example2026,
  author = {Example Author},
  title = {A Beginner Example for Source Practice},
  journal = {Learning Notes},
  year = {2026}
}
```

打开 **Citations**，导入该文献库，并通过面板插入 `example2026`。插入后的源码应类似叙述式 `@example2026` 或括号式 `[@example2026]`。不要手动输入尚未注册的 key，否则 Preview 与 preflight 应提示引用缺失。

如果 Citations 面板或当前流程提供 bibliography block，请在页面结尾添加，然后在 Preview 和 Build 后的网站中再次检查引用及文献表。

:::{caution}
这条文献记录是专门用于软件练习的虚构内容。发布事实性作品前，请替换成真实书目信息。
:::

## 第一行工具栏验收

- [ ] Insert image 正常。
- [ ] 如有测试，拖入或粘贴图片正常。
- [ ] Image settings 保留图片，并正确应用 alt text、caption 与对齐。
- [ ] Attach file 生成可用的受管理下载链接。
- [ ] Resources 的搜索、筛选、引用位置、Insert 与 Save a copy 正常。
- [ ] Citations 能导入 `.bib` 并插入已注册 key。
- [ ] Preview 与 Build 不报告缺失资源或缺失引用 key。
