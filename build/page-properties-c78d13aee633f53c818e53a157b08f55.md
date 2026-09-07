---
title: Create Pages and Set Page Properties
short_title: Set Page Properties
description: Exact export paths, labels, and metadata for every sample page.
authors:
  - name: Haojie Dai
keywords:
  - LanCarbon
  - sample Book
  - beginner
  - tutorial
label: lc-s5-properties
---

## English

# Create Pages and Set Page Properties

Open each page, select **Page Properties**, and enter the values below. Every page must have a unique **Export Path**. Use forward slashes `/`, lowercase file names, no spaces, and the `.md` extension.

| Page | Export Path — copy exactly | Short title | Label — copy exactly |
| :--- | :--- | :--- | :--- |
| Home | `index.md` | `Home` | `sample-home` |
| Getting Started | `01-getting-started/index.md` | `Getting Started` | `sample-getting-started` |
| Why Carbon Matters | `01-getting-started/why-carbon-matters.md` | `Why Carbon Matters` | `sample-why-carbon` |
| My First Observation | `01-getting-started/first-observation.md` | `First Observation` | `sample-observation` |
| Practice and Resources | `02-practice/index.md` | `Practice` | `sample-practice` |
| Formatting Playground | `02-practice/formatting-playground.md` | `Formatting Playground` | `sample-formatting` |
| Resources and Sources | `02-practice/resources-and-sources.md` | `Resources and Sources` | `sample-resources` |
| Final Checklist | `02-practice/final-checklist.md` | `Final Checklist` | `sample-checklist` |

For every page:

- Keep **Show in table of contents** selected.
- **Description:** write one sentence describing that page. Example: `An introduction to the purpose and structure of this practice Book.`
- **Authors:** optional page-level override. Leave blank to rely on the Book author; enter your name only when the page needs its own credit.
- **Date:** use the date the page was written or substantially revised.
- **Keywords:** use two to four page-specific terms separated as the dialog expects, such as `carbon, beginner, observation`.
- **Label:** must be unique within the Book. Labels support stable cross-references and should not contain spaces.

:::{note}
The Section pages also need Export Paths. Giving each Section an `index.md` inside its own folder keeps the project readable and prevents it from colliding with the Book Home `index.md`.
:::

## Verification

After saving all eight pages:

1. Reopen two or three Page Properties dialogs and confirm the values persisted.
2. Check that no two Export Paths are identical.
3. Check that no two Labels are identical.
4. Confirm all eight pages remain visible in the sidebar.

---

## 中文

# 创建页面并设置 Page Properties

逐页打开内容，点击 **Page Properties**，按下表填写。每页必须有唯一的 **Export Path**。路径统一使用正斜杠 `/`、小写文件名、不含空格，并以 `.md` 结尾。

| 页面 | Export Path（原样填写） | Short title | Label（原样填写） |
| :--- | :--- | :--- | :--- |
| Home | `index.md` | `Home` | `sample-home` |
| Getting Started | `01-getting-started/index.md` | `Getting Started` | `sample-getting-started` |
| Why Carbon Matters | `01-getting-started/why-carbon-matters.md` | `Why Carbon Matters` | `sample-why-carbon` |
| My First Observation | `01-getting-started/first-observation.md` | `First Observation` | `sample-observation` |
| Practice and Resources | `02-practice/index.md` | `Practice` | `sample-practice` |
| Formatting Playground | `02-practice/formatting-playground.md` | `Formatting Playground` | `sample-formatting` |
| Resources and Sources | `02-practice/resources-and-sources.md` | `Resources and Sources` | `sample-resources` |
| Final Checklist | `02-practice/final-checklist.md` | `Final Checklist` | `sample-checklist` |

每个页面还应这样处理：

- 保持勾选 **Show in table of contents**。
- **Description：** 用一句话说明本页内容。例如：`An introduction to the purpose and structure of this practice Book.`
- **Authors：** 可选的页面作者覆盖项。通常留空并使用 Book 作者；只有本页需要单独署名时才填写。
- **Date：** 填写创建或重要修订日期。
- **Keywords：** 填写两到四个本页关键词，例如 `carbon, beginner, observation`。
- **Label：** 在当前 Book 内必须唯一，用于稳定的交叉引用，不要包含空格。

:::{note}
Section 页面同样需要 Export Path。每个 Section 使用自己文件夹内的 `index.md`，既便于阅读，也不会与 Book 首页的 `index.md` 冲突。
:::

## 检查

保存八个页面后：

1. 随机重新打开两三个 Page Properties，确认填写值已经保留。
2. 确认没有两个 Export Path 相同。
3. 确认没有两个 Label 相同。
4. 确认八个页面都仍显示在侧边栏中。
