---
title: Rebuilding and Using the Local Website
short_title: Rebuilding and Using the Local Website
description: Bilingual LanCarbon beginner tutorial.
authors:
  - name: Haojie Dai
keywords:
  - LanCarbon
  - Jupyter Book
  - MyST
label: lc-s3-rebuild
---


# Rebuilding and Using the Local Website

![Build window after a successful build](../assets/f2fe167ed5bd34119554be623300d5fcf7380f4706c1481fb1f94e7cfee7ee2c.png)

After the first success, the Build window displays the content status, last successful time, local website address, and saved files location.

- **Build is up to date** means the successful output matches the current Book.
- **Build is out of date** means the Book changed after that success.
- **Open Website** opens the locally served site in your browser.
- **Stop Website** stops the local HTTP server. The saved HTML remains on disk.
- **Open Build Folder** opens the generated files for inspection. Treat them as output; editing them does not update the Book.
- **Change Build Location** selects a different parent directory for future Builds.
- **Close** closes the window.
- **Rebuild Website** generates a fresh website from the current Book.

Normal update cycle:

```text
Edit in LanCarbon → wait for save → Build → Rebuild Website → inspect locally
```

There is no need to Export or clear a folder. If a rebuild fails, expand **Jupyter Book output**, read the first relevant error, fix the named page, and rebuild. A deprecation warning from a dependency can be harmless, but any LanCarbon error or nonzero build result must be resolved before Publish.

The local address works only while LanCarbon's website server is running. Sharing `127.0.0.1` with someone else will not show them your site.

---



# Rebuild 与本地网站操作

![成功构建后的 Build 窗口](../assets/f2fe167ed5bd34119554be623300d5fcf7380f4706c1481fb1f94e7cfee7ee2c.png)

第一次成功后，Build 窗口会显示内容状态、上次成功时间、本地网站地址和保存文件位置。

- **Build is up to date** 表示成功结果与当前 Book 一致。
- **Build is out of date** 表示成功后 Book 又发生了修改。
- **Open Website** 在浏览器中打开本地网站。
- **Stop Website** 停止本地 HTTP 服务；已经保存的 HTML 不会删除。
- **Open Build Folder** 打开生成文件供检查。它们是输出结果，直接修改不会更新 Book。
- **Change Build Location** 为以后的 Build 选择新的上级目录。
- **Close** 关闭窗口。
- **Rebuild Website** 从当前 Book 重新生成网站。

正常更新流程为：

```text
在 LanCarbon 中编辑 → 等待保存 → 打开 Build → Rebuild Website → 本地检查
```

不需要 Export，也不需要手动清空目录。如果 rebuild 失败，展开 **Jupyter Book output**，阅读第一条有实际意义的错误，修复对应页面后再试。依赖库的 deprecation warning 有时不影响结果，但任何 LanCarbon error 或非零构建结果都必须在 Publish 前解决。

本地地址只在 LanCarbon 的网站服务运行时可用。把 `127.0.0.1` 地址发给别人，无法让对方访问你的电脑。
