---
title: Preview, Build, Publish, and Accept the Sample
short_title: Build and Accept the Sample
description: Final workflow and acceptance checklist for the beginner sample Book.
authors:
  - name: Haojie Dai
keywords:
  - LanCarbon
  - sample Book
  - beginner
  - tutorial
label: lc-s5-workflow
---


# Preview, Build, Publish, and Accept the Sample

## Complete the Final Checklist page

Enter this short checklist into the sample Book's `Final Checklist` page:

```markdown
# Final Checklist

- [ ] The table of contents has two Sections and six Child Pages.
- [ ] Every page has a unique Export Path and Label.
- [ ] Book Settings are saved.
- [ ] Preview renders the formatting exercises.
- [ ] Images have alternative text.
- [ ] Attachments and citations have been checked.
- [ ] Build reports zero errors.
- [ ] The local website has correct navigation.
- [ ] The published website has been checked, if publishing was chosen.
```

## Preview the complete Book

Visit all eight pages in order. On each page:

1. wait for **All changes saved**;
2. switch from Edit to **Preview**;
3. read from top to bottom;
4. test internal links and expandable directives;
5. return to Edit and correct any warning or visual problem.

## Optional source copy

Use **Export** only if you want a separate source copy for backup or external editing. Choose an empty destination folder. Build does not read this exported folder; it reads the current Book stored in LanCarbon.

## Build the local website

1. Select **Build**.
2. Confirm Python 3 and Jupyter Book CLI v2 pass their checks.
3. Resolve every preflight error and review warnings.
4. On the first build, select **Choose Location and Build** and choose a stable parent folder.
5. Wait for completion, then select **Open Website**.
6. Visit Home, both Sections, and all Child Pages. Check navigation, formatting, image, attachment, citation, and math.

After editing any page, wait for save and select **Rebuild Website**. The Build panel should change from “Book changed — rebuild required” to “Build is up to date.”

## Optional online publication

Publishing requires Git, GitHub CLI, a signed-in GitHub account, and working access to GitHub. If your network uses a proxy, enable its system proxy or TUN mode before opening Publish.

1. Select **Publish**.
2. Read every environment check; correct any failed item.
3. Create or connect a repository such as `my-first-carbon-book` under **your** account.
4. Initialize GitHub Pages when prompted.
5. After success, select **Open Pages** and inspect the public website.
6. Confirm **Published website** reports the current time and a new commit.

## Final acceptance

| Check | Pass condition |
| :--- | :--- |
| Structure | The sidebar and website show the intended two-level hierarchy. |
| Settings | All Book Settings and Page Properties persist after reopening. |
| Toolbar | Each practiced control produces valid, readable content. |
| Resources | Images, attachments, and registered citations resolve. |
| Preview | No unresolved item remains. |
| Build | Preflight and Jupyter Book finish successfully. |
| Website | Navigation and content work in the local site. |
| Publish, if chosen | Open Pages shows the current built revision. |

:::{important}
The authoritative Book remains inside LanCarbon. The normal update workflow is: edit in LanCarbon → wait for save → Rebuild Website → inspect locally → Update Website. Export is optional.
:::

---



# Preview、Build、Publish 与样例验收

## 完成 Final Checklist 页面

把下面的简短清单写入样例 Book 的 `Final Checklist` 页面：

```markdown
# Final Checklist

- [ ] The table of contents has two Sections and six Child Pages.
- [ ] Every page has a unique Export Path and Label.
- [ ] Book Settings are saved.
- [ ] Preview renders the formatting exercises.
- [ ] Images have alternative text.
- [ ] Attachments and citations have been checked.
- [ ] Build reports zero errors.
- [ ] The local website has correct navigation.
- [ ] The published website has been checked, if publishing was chosen.
```

## Preview 完整 Book

按顺序访问八个页面。每一页都执行：

1. 等待 **All changes saved**；
2. 从 Edit 切换到 **Preview**；
3. 从上到下阅读；
4. 测试内部链接与可展开 directives；
5. 回到 Edit，修正 warning 或视觉问题。

## 可选的源文件副本

只有需要单独备份或外部编辑时才使用 **Export**，并选择空目标文件夹。Build 不读取该导出文件夹，而是读取保存在 LanCarbon 内的当前 Book。

## 构建本地网站

1. 点击 **Build**。
2. 确认 Python 3 与 Jupyter Book CLI v2 检查通过。
3. 解决所有 preflight error，并检查 warning。
4. 第一次 Build 点击 **Choose Location and Build**，选择稳定的父文件夹。
5. 等待完成后点击 **Open Website**。
6. 访问 Home、两个 Section 以及全部 Child Page，检查导航、格式、图片、附件、引用和公式。

修改任意页面后，等待保存，再点击 **Rebuild Website**。Build 面板应从“Book changed — rebuild required”恢复为“Build is up to date”。

## 可选的在线发布

Publish 需要 Git、GitHub CLI、已登录的 GitHub 账号，以及可用的 GitHub 网络连接。如果网络使用代理，打开 Publish 前先启用系统代理或 TUN 模式。

1. 点击 **Publish**。
2. 阅读每一项环境检查，处理所有失败项。
3. 在**自己的**账号下创建或连接名为 `my-first-carbon-book` 的仓库。
4. 按提示初始化 GitHub Pages。
5. 成功后点击 **Open Pages**，检查公开网站。
6. 确认 **Published website** 显示当前时间和新的 commit。

## 最终验收

| 检查项 | 通过标准 |
| :--- | :--- |
| 结构 | 侧边栏和网站显示预期的两级层次。 |
| 设置 | 重新打开后，所有 Book Settings 与 Page Properties 仍保留。 |
| 工具栏 | 每个练习过的控件都生成有效、可读的内容。 |
| 资源 | 图片、附件与已注册引用均能解析。 |
| Preview | 没有 unresolved 项。 |
| Build | Preflight 与 Jupyter Book 都成功完成。 |
| 网站 | 本地网站导航和内容正常。 |
| Publish（如选择） | Open Pages 显示当前构建版本。 |

:::{important}
正式 Book 始终保存在 LanCarbon 内。正常更新流程是：在 LanCarbon 编辑 → 等待保存 → Rebuild Website → 本地检查 → Update Website。Export 是可选步骤。
:::
