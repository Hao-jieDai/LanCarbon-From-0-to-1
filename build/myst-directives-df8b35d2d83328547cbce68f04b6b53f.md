---
title: MyST Directives and Roles
short_title: MyST Directives and Roles
description: Bilingual LanCarbon beginner tutorial.
authors:
  - name: Haojie Dai
keywords:
  - LanCarbon
  - Jupyter Book
  - MyST
label: lc-s2-myst
---


# MyST Directives and Roles

MyST extends Markdown with scientific and technical publishing features. A **role** is usually inline; a **directive** is a block with a name, optional settings, and content.

## Roles

A role appears inside a sentence and has a compact form. LanCarbon's abbreviation, keyboard, underline, superscript, and subscript tools create supported role syntax. Preview the result immediately after insertion.

## Directives

Open **Directives** and choose a template. Common uses include notes, warnings, figures, and other structured content. A directive uses an opening fence, a name in braces, optional lines beginning with `:`, body content, and a closing fence.

The following is shown as source text for learning:

````markdown
```{note}
This is useful background information.
```

```{warning}
Back up your data before a major change.
```
````

For an imported image, the Image settings panel may create a figure block with options such as width, alignment, alternative text, and caption. Edit the entire figure block together. A caption belongs inside that block; aligning only the caption line can trigger the protected-selection message.

## Good practice

1. Insert a template from the toolbar.
2. Replace every placeholder.
3. Keep the opening and closing fences balanced.
4. Switch to Preview.
5. Run Build before publishing; the official Jupyter Book engine is the final compatibility check.

Use plain Markdown when it is sufficient. Reserve directives for content that needs a semantic container or extra settings.

---



# MyST Directives 与 Roles

MyST 在 Markdown 基础上增加了科学和技术出版功能。**Role** 通常用于一行文字内部；**Directive** 是带名称、可选设置和正文内容的结构化块。

## Roles

Role 出现在句子内部，形式较紧凑。LanCarbon 的缩写、键盘、下划线、上标和下标工具会生成受支持的 role 语法。插入后应立即切换 Preview 检查结果。

## Directives

打开 **Directives** 并选择模板。常见用途包括提示、警告、图片和其他结构化内容。Directive 包含开头围栏、花括号中的名称、以 `:` 开头的可选设置、正文和结尾围栏。

下面以源代码形式展示学习示例：

````markdown
```{note}
This is useful background information.
```

```{warning}
Back up your data before a major change.
```
````

对于已经导入的图片，Image settings 面板可能生成 figure 块，其中包含宽度、对齐、替代文字和 caption 等选项。请把整个 figure 块作为整体修改。Caption 属于该结构的一部分，仅选中 caption 行再点对齐可能触发“受保护选择”提示。

## 推荐做法

1. 从工具栏插入模板。
2. 替换所有占位内容。
3. 确保开头和结尾围栏配对。
4. 切换到 Preview。
5. 发布前运行 Build；官方 Jupyter Book 引擎是最终兼容性检查。

普通 Markdown 能满足需求时优先使用普通语法。只有内容需要语义容器或额外设置时，再使用 Directives。
