---
title: Understanding Page Properties
short_title: Understanding Page Properties
description: Bilingual LanCarbon beginner tutorial.
authors:
  - name: Haojie Dai
keywords:
  - LanCarbon
  - Jupyter Book
  - MyST
label: lc-s2-properties
---


# Understanding Page Properties

![Page Properties window](../assets/4ae88bd1f7ad63f1b331b9800cb081de2926dbbe799019ebf411cc87edb28eaa.png)

Each page has properties independent of the Book settings.

| Field | Required? | Meaning |
|---|---:|---|
| Export Path | Yes | Relative filename used in the generated project, such as `lessons/first-step.md`. Use forward slashes, no drive letter, and a `.md` ending for Markdown pages. The home page remains `index.md`. |
| Show in table of contents | No | When checked, the page appears in website navigation. Hidden pages may still be linked directly. |
| Short title | No | A compact navigation title when the full title is long. |
| Description | No | Page-specific summary. |
| Authors | No | Overrides or supplements authorship at page level. |
| Date | No | Publication or revision date for this page. |
| Keywords | No | Topics specific to this page. |
| Label | No | Stable MyST target used for cross-references. Use a unique, simple value such as `first-build`. |

Good export paths are lowercase, readable, and stable. Changing a path after publication can change the page URL and break old links. Organize related pages in the same folder, for example `build/first-build.md` and `build/rebuild.md`.

Select **Save Properties** after changes. Duplicate paths, invalid paths, missing Notes, and duplicate labels are detected by the preflight check before Build.

---



# 理解 Page Properties

![Page Properties 窗口](../assets/4ae88bd1f7ad63f1b331b9800cb081de2926dbbe799019ebf411cc87edb28eaa.png)

每个页面都有一组独立于 Book Settings 的属性。

| 字段 | 是否必填 | 含义 |
|---|---:|---|
| Export Path | 是 | 生成项目时使用的相对文件名，例如 `lessons/first-step.md`。使用正斜杠，不写盘符，Markdown 页面以 `.md` 结尾。首页固定为 `index.md`。 |
| Show in table of contents | 否 | 勾选后页面出现在网站导航中。隐藏页面仍可以通过直接链接访问。 |
| Short title | 否 | 完整标题较长时，用于导航栏的短标题。 |
| Description | 否 | 当前页面的摘要。 |
| Authors | 否 | 页面级作者信息。 |
| Date | 否 | 当前页面的发布日期或修订日期。 |
| Keywords | 否 | 当前页面特有的主题关键词。 |
| Label | 否 | 用于交叉引用的稳定 MyST 目标。请使用唯一且简单的值，例如 `first-build`。 |

好的 Export Path 应使用小写、容易识别并尽量保持稳定。在线发布后再改路径，可能会改变页面网址并使旧链接失效。相关页面可以放在同一目录，例如 `build/first-build.md` 与 `build/rebuild.md`。

修改后点击 **Save Properties**。重复路径、非法路径、缺失 Note 和重复 Label 会在 Build 前的 preflight 检查中被发现。
