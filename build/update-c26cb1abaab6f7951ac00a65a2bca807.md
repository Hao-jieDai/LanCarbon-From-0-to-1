---
title: Updating an Existing Published Book
short_title: Updating an Existing Published Book
description: Bilingual LanCarbon beginner tutorial.
authors:
  - name: Haojie Dai
keywords:
  - LanCarbon
  - Jupyter Book
  - MyST
label: lc-s4-update
---

## English

# Updating an Existing Published Book

Once a Book is connected, do not create another repository for each revision. Use the saved binding.

```text
Edit in LanCarbon
→ wait for All changes saved
→ Build / Rebuild Website
→ inspect Open Website
→ Publish
→ Update Website
→ wait for deployment
→ Open Pages and verify
```

Export is not part of this routine unless you want a separate source backup. The Build location and repository binding are remembered per Book.

The Publish window compares the current Book with the latest successful Build. If the build is outdated, rebuild it. If a Git network check fails, the update button may be unavailable until connectivity is restored and checks are refreshed. A failed update does not erase the already published website; it remains on its previous successful commit.

After success, compare the Published website commit/time with what you just sent. GitHub Pages can cache or deploy asynchronously, so wait briefly and perform a full browser refresh if old text remains. Open Repository can confirm the newest commit reached `gh-pages`.

Make a meaningful publication only when the public result is ready. Small local edits can accumulate before the next Build and Update.

---

## 中文

# 更新已经发布的 Book

Book 建立连接后，不需要每次修改都创建新仓库，应继续使用已保存的绑定。

```text
在 LanCarbon 中编辑
→ 等待 All changes saved
→ Build / Rebuild Website
→ 用 Open Website 本地检查
→ 打开 Publish
→ Update Website
→ 等待部署
→ Open Pages 并验证
```

除非需要额外保存源文件备份，否则日常更新不包含 Export。每本 Book 的 Build 位置和仓库绑定都会被记住。

Publish 窗口会比较当前 Book 与最新成功 Build。如果 build outdated，就先重新构建。如果 Git 网络检查失败，更新按钮可能暂时不可用，直到恢复连接并刷新检查。更新失败不会删除已发布网站；线上仍保留上一次成功 commit。

成功后，对照 Published website 显示的 commit/时间与本次操作。GitHub Pages 部署和缓存可能存在延迟；仍显示旧文字时，稍等后进行浏览器完整刷新。Open Repository 可以确认最新 commit 是否已经到达 `gh-pages`。

只有公开结果准备好时才需要发布。多次很小的本地修改可以积累到一起，再执行一次 Build 和 Update。
