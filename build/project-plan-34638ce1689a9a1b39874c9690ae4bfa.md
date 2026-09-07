---
title: Plan the Sample Book
short_title: Plan the Sample Book
description: Create the sample Book and its clear two-section table of contents.
authors:
  - name: Haojie Dai
keywords:
  - LanCarbon
  - sample Book
  - beginner
  - tutorial
label: lc-s5-plan
---

## English

# Plan the Sample Book

## Create the Book

1. Switch the left sidebar to **Jupyter Book**.
2. Select the **+** button beside the Book selector.
3. Enter `My First Carbon Book` as the title and confirm.
4. Select the new Book before adding pages.

LanCarbon creates the Home page automatically. Do not create a second Home page.

## Create the table of contents

Create the following items in this order:

1. Select **+ Section** and name it `Getting Started`.
2. Select that Section, choose **+ Child Page**, and create `Why Carbon Matters`.
3. Keep the same Section selected and create `My First Observation`.
4. Select **+ Section** and name it `Practice and Resources`.
5. Under it, create `Formatting Playground`.
6. Create `Resources and Sources`.
7. Create `Final Checklist`.

Afterward, compare the sidebar with this structure:

```text
My First Carbon Book
├─ Getting Started
│  ├─ Why Carbon Matters
│  └─ My First Observation
└─ Practice and Resources
   ├─ Formatting Playground
   ├─ Resources and Sources
   └─ Final Checklist
```

:::{important}
Select a Section before choosing **+ Child Page**. The selected Section becomes the parent. If a page appears in the wrong place, remove it from this Book and add it again under the intended Section; removing a page from a Book does not delete its underlying Note.
:::

## Why this structure works

The Home page answers “What is this Book?” The first Section contains subject content. The second Section contains practice and supporting material. Two levels are enough for a first project and produce predictable website navigation.

---

## 中文

# 规划样例 Book

## 创建 Book

1. 把左侧栏切换到 **Jupyter Book**。
2. 点击 Book 选择框旁边的 **+**。
3. 标题填写 `My First Carbon Book` 并确认。
4. 添加页面前，确认当前选择的是这本新 Book。

LanCarbon 会自动创建 Home 页面，不要再创建第二个首页。

## 创建目录结构

请按以下顺序创建：

1. 点击 **+ Section**，命名为 `Getting Started`。
2. 选中该 Section，点击 **+ Child Page**，创建 `Why Carbon Matters`。
3. 保持该 Section 被选中，再创建 `My First Observation`。
4. 点击 **+ Section**，命名为 `Practice and Resources`。
5. 在其下创建 `Formatting Playground`。
6. 创建 `Resources and Sources`。
7. 创建 `Final Checklist`。

完成后，将左侧目录与下列结构比较：

```text
My First Carbon Book
├─ Getting Started
│  ├─ Why Carbon Matters
│  └─ My First Observation
└─ Practice and Resources
   ├─ Formatting Playground
   ├─ Resources and Sources
   └─ Final Checklist
```

:::{important}
点击 **+ Child Page** 前先选中目标 Section。当前选中的 Section 就是父级。如果页面位置错误，可以先从 Book 中移除，再添加到正确 Section；从 Book 中移除页面不会删除底层 Note。
:::

## 为什么采用这个结构

Home 页面回答“这本书是什么”；第一个 Section 放主题内容；第二个 Section 放练习与支持材料。两级结构足够新手使用，也能生成清楚、可预测的网站导航。
