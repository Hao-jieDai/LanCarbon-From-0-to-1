---
title: Complete the Formatting Playground
short_title: Formatting Playground
description: A toolbar-driven exercise covering rich Markdown and MyST formatting.
authors:
  - name: Haojie Dai
keywords:
  - LanCarbon
  - sample Book
  - beginner
  - tutorial
label: lc-s5-formatting
---


# Complete the Formatting Playground

Open the sample Book's `Formatting Playground` page. Perform the exercises in **Edit**, then inspect them in **Preview**. Use the toolbar button named in bold whenever one is available.

## Editing and headings

1. Type `Formatting Playground` and apply **Heading 1**.
2. Create smaller headings with **Heading 2** and **Heading 3**.
3. Type a sentence, change it, choose **Undo**, then **Redo**.

## Inline text tools

Create this line by selecting one phrase at a time:

Normal text, **bold**, *italic*, {underline}`underlined`, {delete}`deleted`, CO{sub}`2`, m{sup}`2`, {abbr}`IPCC (Intergovernmental Panel on Climate Change)`, and {kbd}`Ctrl+F`.

Then insert inline code: `carbon_total = 42`.

## Alignment

Write three short standalone paragraphs and apply **Align left**, **Align center**, and **Align right**. Check the generated syntax in Edit and the visual positions in Preview. Alignment is best used sparingly for captions or short display text.

## Lists and quotation

Use **Lists** to create:

- Atmosphere
  - Measurement
  - Interpretation
- Land
- Ocean

Then create an ordered list:

1. Observe.
2. Record.
3. Review.

Select one sentence and apply **Quote**:

> A useful note states what was observed and how it was measured.

Use **Separator** to insert the line below.

---

## Link and code

Use **Link** to create [LanCarbon project practice](https://github.com/). On the desktop Preview, external navigation may be blocked intentionally; verify the destination after the Book is built.

Use **Code** to create a fenced Python block:

```python
emissions = 100
removals = 40
net_change = emissions - removals
print(net_change)
```

## Table

Use **Table** to create three columns and three data rows. Set the last column to right alignment.

| Store | Example | Value |
| :--- | :--- | ---: |
| Atmosphere | Sample A | 100 |
| Land | Sample B | 40 |
| Ocean | Sample C | 60 |

Reopen the table tool from inside the table, change one value, apply it, then use Undo and Redo.

## Mathematics

Use **Math** once in inline mode and once in display mode:

Inline: $E-R=60$.

$$
\Delta C = E - R = 100 - 40 = 60
$$

Try a fraction template and replace its placeholders before applying.

## Directives

Use **Directives** to insert at least a Note, Tip, Warning, and Dropdown:

:::{note}
This is a neutral explanation.
:::

:::{tip}
Preview after each unfamiliar format.
:::

:::{warning} Check the unit
A number without a unit may be misleading.
:::

:::{dropdown} Show the answer
The net change in this example is **60**.
:::

If you want an extra test, insert a nested block or an initially open dropdown. Keep the content short so it is easy to inspect.

## Acceptance

- [ ] Every toolbar action changed the source at the cursor or selection.
- [ ] Undo and Redo restored the expected content.
- [ ] Edit contains readable Markdown/MyST rather than corrupted text.
- [ ] Preview renders every element without an unresolved warning.
- [ ] The built website later shows the same meaning and hierarchy.

---



# 完成 Formatting Playground

打开样例 Book 的 `Formatting Playground` 页面。在 **Edit** 中逐项练习，再到 **Preview** 检查。存在对应按钮时，请使用文中加粗的工具栏按钮。

## 编辑与标题

1. 输入 `Formatting Playground` 并应用 **Heading 1**。
2. 使用 **Heading 2** 和 **Heading 3** 创建较低级标题。
3. 输入一句话并修改，然后点击 **Undo**，再点击 **Redo**。

## 行内文字工具

每次选择一个短语，完成下列一行：

Normal text, **bold**, *italic*, {underline}`underlined`, {delete}`deleted`, CO{sub}`2`, m{sup}`2`, {abbr}`IPCC (Intergovernmental Panel on Climate Change)`, and {kbd}`Ctrl+F`.

再插入行内代码：`carbon_total = 42`。

## 对齐

写三个独立短段落，分别应用 **Align left**、**Align center** 和 **Align right**。在 Edit 中观察生成语法，在 Preview 中检查位置。对齐适合少量用于标题说明或短展示文字。

## 列表与引用

使用 **Lists** 创建：

- Atmosphere
  - Measurement
  - Interpretation
- Land
- Ocean

再创建编号列表：

1. Observe.
2. Record.
3. Review.

选择一句话并应用 **Quote**：

> A useful note states what was observed and how it was measured.

使用 **Separator** 插入下面的分隔线。

---

## 链接与代码

使用 **Link** 创建 [LanCarbon project practice](https://github.com/)。桌面 Preview 可能有意阻止外部跳转，请在 Build 后的网站中验证目标地址。

使用 **Code** 创建 Python 围栏代码块：

```python
emissions = 100
removals = 40
net_change = emissions - removals
print(net_change)
```

## 表格

使用 **Table** 创建三列、三行数据，并将最后一列设为右对齐。

| Store | Example | Value |
| :--- | :--- | ---: |
| Atmosphere | Sample A | 100 |
| Land | Sample B | 40 |
| Ocean | Sample C | 60 |

把光标放回表格内重新打开表格工具，修改一个数值并应用，然后使用 Undo 和 Redo。

## 数学公式

使用 **Math** 分别插入一次行内公式和展示公式：

行内：$E-R=60$。

$$
\Delta C = E - R = 100 - 40 = 60
$$

再尝试 Fraction 模板，在应用前替换占位符。

## Directives

使用 **Directives** 至少插入 Note、Tip、Warning 和 Dropdown：

:::{note}
This is a neutral explanation.
:::

:::{tip}
Preview after each unfamiliar format.
:::

:::{warning} Check the unit
A number without a unit may be misleading.
:::

:::{dropdown} Show the answer
The net change in this example is **60**.
:::

如果希望增加练习，还可以插入 Nested blocks 或 Initially open。内容保持简短，便于检查。

## 验收

- [ ] 每次工具栏操作都在光标或选区位置正确修改源码。
- [ ] Undo 和 Redo 能恢复预期内容。
- [ ] Edit 中是可读的 Markdown/MyST，没有损坏文字。
- [ ] Preview 正常渲染所有元素，没有 unresolved 警告。
- [ ] 后续 Build 的网站保持相同含义和层级。
