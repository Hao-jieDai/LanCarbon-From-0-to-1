---
title: Markdown Essentials and the Formatting Toolbar
short_title: Markdown Essentials and the Formatting Toolbar
description: Bilingual LanCarbon beginner tutorial.
authors:
  - name: Haojie Dai
keywords:
  - LanCarbon
  - Jupyter Book
  - MyST
label: lc-s2-markdown
---

## English

# Markdown Essentials and the Formatting Toolbar

Markdown is plain text with small marks that describe structure. The toolbar writes these marks for you, but recognizing them makes editing easier.

## Structure and history

- **Undo / Redo** reverses or reapplies recent editor changes.
- The **Paragraph** menu inserts headings. Use one `#` heading for the page title, `##` for major parts, and `###` for subsections. Do not choose heading levels only for visual size.

```markdown
# Page title
## Major part
### Smaller part
```

## Inline emphasis

| Tool | Source example | Result or meaning |
|---|---|---|
| Bold | `**important**` | strong emphasis |
| Italic | `*term*` | emphasis or a term |
| Underline | MyST role inserted by LanCarbon | underlined presentation |
| Strikethrough | `~~removed~~` | deleted or obsolete text |
| Superscript | MyST role | raised text such as an ordinal |
| Subscript | MyST role | lowered text such as a chemical index |
| Abbr | abbreviation role | an abbreviation with an explanation |
| Keyboard | keyboard role | a key such as Ctrl |

Select the intended words before clicking an inline tool. If nothing is selected, LanCarbon inserts an editable sample or marker.

## Paragraph-level tools

- **Align** changes paragraph alignment. Do not select text inside a special MyST block, code block, table, or math block; use that feature's own settings instead.
- **Lists** creates unordered, ordered, or task lists. Keep a blank line before and after a list.
- **Quote** starts a block quote with `>`.
- **Link** inserts `[visible text](https://example.com)`.
- **Code** inserts inline code or a fenced code block. Choose the language after the opening fence when syntax highlighting matters.
- **Table** inserts a Markdown table; keep one header row and a separator row.
- **Math** inserts inline or display mathematics.
- The horizontal-line tool inserts `---` as a thematic break.

```markdown
- First item
- Second item

> A short quotation.

[LanCarbon project](https://github.com/)

| Item | Status |
|---|---|
| Draft | In progress |
```

## Selection safety

If LanCarbon says the selection contains code, math, a table, or special syntax, it is protecting a structured block from being partially wrapped. Select plain text only, use the relevant panel, or edit the Markdown source directly.

---

## 中文

# Markdown 基础与格式工具栏

Markdown 是一种通过少量标记表达结构的纯文本格式。工具栏可以替你写入这些标记，但认识它们会让修改更轻松。

## 结构与操作历史

- **Undo / Redo** 撤销或恢复最近的编辑操作。
- **Paragraph** 菜单插入标题。每页用一个 `#` 作为页面标题，`##` 表示主要部分，`###` 表示更小的分节。不要只因为字号大小而随意选择标题级别。

```markdown
# 页面标题
## 主要部分
### 更小的部分
```

## 行内格式

| 工具 | 源文示例 | 结果或含义 |
|---|---|---|
| Bold | `**important**` | 强调重要内容 |
| Italic | `*term*` | 一般强调或术语 |
| Underline | LanCarbon 插入的 MyST role | 下划线显示 |
| Strikethrough | `~~removed~~` | 删除或废弃内容 |
| Superscript | MyST role | 上标文字 |
| Subscript | MyST role | 下标文字，例如化学式序号 |
| Abbr | 缩写 role | 带解释的缩写 |
| Keyboard | 键盘 role | 表示 Ctrl 等按键 |

点击行内格式工具前，先选中需要处理的文字。如果没有选中内容，LanCarbon 会插入可继续修改的示例或标记。

## 段落级工具

- **Align** 修改段落对齐。不要只选中特殊 MyST 块、代码块、表格或数学块中的一部分再应用；应使用对应功能的设置，或直接编辑源文。
- **Lists** 创建无序、有序或任务列表。列表前后保留空行。
- **Quote** 用 `>` 创建块引用。
- **Link** 插入 `[显示文字](https://example.com)`。
- **Code** 插入行内代码或围栏代码块。需要语法高亮时，在开头围栏后写语言名称。
- **Table** 插入 Markdown 表格；应保留表头行和分隔行。
- **Math** 插入行内或独立数学公式。
- 横线工具插入 `---` 作为主题分隔线。

```markdown
- 第一项
- 第二项

> 一段简短引用。

[LanCarbon project](https://github.com/)

| 项目 | 状态 |
|---|---|
| 初稿 | 进行中 |
```

## 选择内容时的保护

如果 LanCarbon 提示所选内容包含代码、数学、表格或特殊语法，说明软件正在避免把结构化块的一部分错误包裹。请只选择普通文本、使用该功能自己的面板，或直接修改 Markdown 源文。
