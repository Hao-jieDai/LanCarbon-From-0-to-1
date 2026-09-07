---
title: Understanding Book Settings
short_title: Understanding Book Settings
description: Bilingual LanCarbon beginner tutorial.
authors:
  - name: Haojie Dai
keywords:
  - LanCarbon
  - Jupyter Book
  - MyST
label: lc-s2-settings
---

## English

# Understanding Book Settings

![Book Settings window](../assets/2ed04c61ae2d3f2479c2090e9d729a4b64608925a5b0612b2284f7533e6f08d7.png)

Open **Settings** while the intended Book is selected.

| Field | Required? | What to enter |
|---|---:|---|
| Book title | Yes | The complete human-readable title. |
| Subtitle | No | A short second line that explains scope. |
| Description | No | One or two sentences for metadata and discovery. |
| Authors | No | Author names. Separate multiple names as the interface instructs. |
| GitHub repository URL | No at first | The public repository address once known. Publishing can establish the binding separately. |
| License | No, recommended for sharing | A license identifier such as `CC-BY-4.0`, only if it matches your intended terms. |
| Keywords | No | A small set of discoverable topics. |
| Site title | No | Short browser/site branding; Book title is a sensible default. |
| Logo Path | No | A managed image reference used as the site logo. Use Resources rather than typing an arbitrary local file path. |
| Favicon Path | No | A managed icon reference for the browser tab. |

Only **Book title** is marked with `(*)` and must be present. Optional does not mean unimportant: author, description, license, and keywords make a public Book easier to understand and reuse.

Select **Save Settings** after editing. Wait for the save confirmation before Building. If a logo or favicon is missing during Build, reopen Resources and reinsert or reselect the managed file.

---

## 中文

# 理解 Book Settings

![Book Settings 窗口](../assets/2ed04c61ae2d3f2479c2090e9d729a4b64608925a5b0612b2284f7533e6f08d7.png)

先选中目标 Book，再打开 **Settings**。

| 字段 | 是否必填 | 应填写的内容 |
|---|---:|---|
| Book title | 是 | 完整、便于阅读的书名。 |
| Subtitle | 否 | 用一行短句说明范围。 |
| Description | 否 | 用一两句话概括内容，便于元数据展示和检索。 |
| Authors | 否 | 作者姓名；多人时按照界面提示分隔。 |
| GitHub repository URL | 初期不必填 | 已经确定后可填写公开仓库地址；Publish 也会单独建立绑定。 |
| License | 否，但公开分享时建议填写 | 例如 `CC-BY-4.0`，应与你希望采用的授权条件一致。 |
| Keywords | 否 | 少量能够代表内容的关键词。 |
| Site title | 否 | 网站或浏览器中的较短名称；通常可以沿用 Book title。 |
| Logo Path | 否 | 网站 Logo 的受管理图片引用。应通过 Resources 管理，不要手工填写任意本地文件路径。 |
| Favicon Path | 否 | 浏览器标签页图标的受管理引用。 |

只有带 `(*)` 的 **Book title** 必须填写。可选不等于没有价值：作者、描述、许可证和关键词能让公开 Book 更容易被理解和复用。

修改后点击 **Save Settings**，等待保存完成再 Build。如果 Build 提示 Logo 或 favicon 缺失，请重新打开 Resources，重新导入或选择受管理文件。
