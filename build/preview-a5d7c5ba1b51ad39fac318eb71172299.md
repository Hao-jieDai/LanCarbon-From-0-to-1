---
title: Previewing and Checking Your Content
short_title: Previewing and Checking Your Content
description: Bilingual LanCarbon beginner tutorial.
authors:
  - name: Haojie Dai
keywords:
  - LanCarbon
  - Jupyter Book
  - MyST
label: lc-s2-preview
---


# Previewing and Checking Your Content

Select **Preview** to render the current page without leaving LanCarbon. Use it frequently, especially after headings, lists, tables, math, directives, image settings, and citations.

Check the following:

1. The heading hierarchy is logical.
2. Lists and tables are not merged into nearby paragraphs.
3. Links open the intended location.
4. Images have the intended width, alignment, alternative text, and caption.
5. Equations and special MyST content render as expected.
6. There are no visible placeholders left from toolbar templates.

Preview is page-focused and optimized for writing. It is not the complete Book website and does not replace Build. Navigation, theme assets, final cross-references, publication paths, and official MyST/Jupyter Book compatibility must be checked in the local built website.

If Preview differs from the built website, treat the successful official Build as the publication reference. First inspect the source around the affected block, then rebuild. Unsupported or unsafe embedded content may remain as source or show a notice instead of running inside the desktop application.

---



# 使用 Preview 检查内容

点击 **Preview** 可以在不离开 LanCarbon 的情况下渲染当前页面。建议经常使用，尤其是在修改标题、列表、表格、数学公式、Directives、图片设置和引用之后。

逐项检查：

1. 标题层级是否合理。
2. 列表和表格是否与相邻段落意外连在一起。
3. 链接是否打开正确位置。
4. 图片宽度、对齐、替代文字和 caption 是否正确。
5. 公式和特殊 MyST 内容是否符合预期。
6. 工具栏模板中是否还残留未替换的占位文字。

Preview 以当前页面和写作效率为重点，它不是完整 Book 网站，也不能取代 Build。网站导航、主题资源、最终交叉引用、发布路径以及 MyST/Jupyter Book 官方兼容性，都需要在本地构建的网站中检查。

如果 Preview 与构建后的网站不同，应把成功通过官方 Build 的结果作为发布依据。先检查受影响结构附近的源文，再重新 Build。软件内不支持或不安全的嵌入内容，可能保持为源文或显示提示，而不会在桌面程序内运行。
