---
title: Creating Your First Book
short_title: Creating Your First Book
description: Bilingual LanCarbon beginner tutorial.
authors:
  - name: Haojie Dai
keywords:
  - LanCarbon
  - Jupyter Book
  - MyST
label: lc-s2-create
---

## English

# Creating Your First Book

## Create the Book

1. Select **Jupyter Book** in the sidebar.
2. Select the plus button beside the Book selector.
3. Enter a clear title and confirm. LanCarbon creates the Book and its home page.
4. Open **Settings** and complete the key metadata described on the next page.

## Understand the hierarchy

- **Book home page** is the opening page and always exports as `index.md`.
- **Section** is a top-level page that groups related content. It can contain introductory text and Child Pages.
- **Child Page** is a normal content page nested under a Section or another page.
- **Table of contents** is the ordered tree in the sidebar and becomes the website navigation.

A simple first Book might be:

```text
My First Book
├─ Getting Started
│  ├─ Welcome
│  └─ What You Need
├─ Main Topic
│  ├─ First Lesson
│  └─ Second Lesson
└─ Further Reading
```

## Add and arrange pages

Select the home page, then choose **+ Section**. Give the Section a meaningful title. Select that Section and choose **+ Child Page**. Repeat for other pages. Use the Book tree's supported drag-and-drop behavior to reorder pages or move them between Sections.

Use one subject per page. Short pages are easier to navigate, review, and update. Give every page a unique export path and a visible first-level heading that matches its purpose.

## Removing versus deleting

**Remove from Book** disconnects the page from this Book and leaves it as an ordinary Note. The trash control deletes the Note itself. **Delete** in the Book controls deletes the entire Book and all pages after confirmation, so back up important work first.

---

## 中文

# 从零创建第一本 Book

## 创建 Book

1. 在侧边栏选择 **Jupyter Book**。
2. 点击 Book 下拉框旁边的加号。
3. 输入清晰的书名并确认。LanCarbon 会创建 Book 及其首页。
4. 打开 **Settings**，填写下一页说明的关键元数据。

## 理解层级结构

- **Book 首页** 是全书的起始页，并固定导出为 `index.md`。
- **Section** 是组织相关内容的顶层页面。它既可以包含导语，也可以包含多个 Child Page。
- **Child Page** 是位于 Section 或其他页面下面的普通内容页。
- **Table of contents** 就是侧边栏中的有序树形目录，它会成为网站导航。

一本简单的新手 Book 可以采用以下结构：

```text
My First Book
├─ Getting Started
│  ├─ Welcome
│  └─ What You Need
├─ Main Topic
│  ├─ First Lesson
│  └─ Second Lesson
└─ Further Reading
```

## 添加和整理页面

先选中首页，再点击 **+ Section**，给 Section 一个明确标题。随后选中该 Section，点击 **+ Child Page**。其他页面依此添加。使用 Book 目录支持的拖放操作调整顺序，或把页面移动到其他 Section。

建议每个页面只讲一个主题。较短的页面更容易导航、检查和更新。每页都应有唯一的 Export Path，并在正文开头写一个符合页面用途的一级标题。

## 移出与删除的区别

**Remove from Book** 只会把页面从当前 Book 中移出，对应内容仍作为普通 Note 保留。垃圾桶会删除 Note 本身。Book 操作区中的 **Delete** 会在确认后删除整本 Book 及其全部页面，重要内容请先备份。
