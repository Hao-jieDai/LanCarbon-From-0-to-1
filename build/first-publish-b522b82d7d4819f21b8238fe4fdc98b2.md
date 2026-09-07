---
title: Publishing Your First Website
short_title: Publishing Your First Website
description: Bilingual LanCarbon beginner tutorial.
authors:
  - name: Haojie Dai
keywords:
  - LanCarbon
  - Jupyter Book
  - MyST
label: lc-s4-first
---


# Publishing Your First Website

## Final local check

1. Wait for the latest edit to save.
2. Build or Rebuild the website.
3. Open the local website and inspect it.
4. Remove private or unfinished material.

## Connect the repository

Open Publish and make every required environment/account/network check pass. For a new user, the simplest route is often **New repository**: confirm your account as owner, enter a unique repository name, keep `gh-pages`, choose visibility, and select **Connect and Initialize Pages**. If you created an empty repository yourself on GitHub, choose **Existing repository** and enter its exact owner and name.

Repository and folder are different concepts. Seeing a repository on github.com does not mean LanCarbon is connected; the binding card must show that exact `owner/name` as reachable.

## Publish

After the binding is ready, select the main publish/update action. LanCarbon downloads the publication branch, replaces the managed website files, creates a Git commit, pushes it, requests a Pages deployment, and verifies the published revision.

Wait for the success state. Deployment may remain pending briefly after the push. Select **Open Pages** only after the Pages URL is reported. The first visit may take several minutes. Refresh the browser after waiting rather than starting another publish immediately.

## Acceptance check

The first publication is complete when:

- Repository binding passes.
- Git HTTPS connection passes.
- GitHub Pages shows the expected URL.
- Published website shows a time and commit.
- Open Pages displays the full Book theme and current content.
- Navigation, images, attachments, and internal links work from the public URL.

---



# 第一次发布网站

## 最终本地检查

1. 等待最新编辑保存。
2. Build 或 Rebuild 网站。
3. 打开本地网站并检查。
4. 删除隐私内容和未完成内容。

## 连接仓库

打开 Publish，让所有必要的环境、账号和网络检查通过。新手最简单的方式通常是选择 **New repository**：确认 owner 为自己的账号，输入唯一仓库名，保留 `gh-pages`，选择可见性，再点击 **Connect and Initialize Pages**。如果你已经在 GitHub 手工创建了空仓库，则选择 **Existing repository**，准确填写 owner 与仓库名。

Repository 与本地文件夹是不同概念。在 github.com 能看到仓库，不代表 LanCarbon 已经连接；Repository binding 卡片必须显示完全相同的 `owner/name` 且可访问。

## 发布

绑定完成后，点击主要发布/更新按钮。LanCarbon 会下载发布分支、替换受管理网站文件、创建 Git commit、推送到 GitHub、请求 Pages 部署，并检查在线版本。

等待成功状态。推送结束后，部署可能短暂显示 pending。看到 Pages URL 后再点击 **Open Pages**。第一次访问可能需要等待几分钟；先等待并刷新浏览器，不要立刻重复发布。

## 验收检查

满足以下条件，第一次发布才算完成：

- Repository binding 通过。
- Git HTTPS connection 通过。
- GitHub Pages 显示预期网址。
- Published website 显示时间和 commit。
- Open Pages 展示完整 Book 主题和当前内容。
- 从公开网址访问时，导航、图片、附件和内部链接均正常。
