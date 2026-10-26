---
title: Preparing GitHub and Signing In
short_title: Preparing GitHub and Signing In
description: Bilingual LanCarbon beginner tutorial.
authors:
  - name: Haojie Dai
keywords:
  - LanCarbon
  - Jupyter Book
  - MyST
label: lc-s4-prepare
---


# Preparing GitHub and Signing In

## One-time preparation

1. Create and verify a personal account at [GitHub](https://github.com/).
2. Install [Git for Windows](https://git-scm.com/install/windows).
3. Install [GitHub CLI](https://cli.github.com/).
4. Restart LanCarbon so it can detect newly installed commands.
5. Build the Book successfully.

Open **Publish**. Git and GitHub CLI should show check marks and versions. If the account card says you are signed out, select **Sign in with GitHub CLI**. LanCarbon opens a visible terminal.

The device sign-in flow normally asks whether Git should use your GitHub credentials, displays a one-time code, and opens `https://github.com/login/device`. Copy the code, sign in in the browser, approve the GitHub CLI request, return to the terminal, and wait for success. Then return to LanCarbon and select **Refresh Checks**.

LanCarbon uses the account already authenticated by GitHub CLI. It does not ask you to put a GitHub password or token in the Book.

## After restart

Authentication is normally stored securely by GitHub CLI and survives a computer or LanCarbon restart. You only need to sign in again if the credential is revoked, expires, is removed, you sign out, or you change accounts.

## If the button seems inactive

Look for a terminal window behind LanCarbon or in the taskbar. If GitHub CLI was installed while LanCarbon was open, close and restart LanCarbon. If no terminal appears after that, open a normal terminal and run `gh auth login`, complete the flow, then use **Refresh Checks**.

---



# 准备 GitHub 并登录账号

## 一次性准备

1. 在 [GitHub](https://github.com/)创建并验证个人账号。
2. 安装 [Git for Windows](https://git-scm.com/install/windows)。
3. 安装 [GitHub CLI](https://cli.github.com/)。
4. 重启 LanCarbon，使软件能够检测到新安装的命令。
5. 先成功 Build 当前 Book。

打开 **Publish**。Git 与 GitHub CLI 应显示通过标记和版本。如果账号卡片提示未登录，点击 **Sign in with GitHub CLI**。LanCarbon 会打开一个可见终端。

设备登录流程通常会先询问是否让 Git 使用 GitHub 凭据，然后显示一次性代码并打开 `https://github.com/login/device`。复制代码，在浏览器登录并批准 GitHub CLI 请求，回到终端等待成功。最后回到 LanCarbon，点击 **Refresh Checks**。

LanCarbon 使用 GitHub CLI 已经认证的账号，不会要求你把 GitHub 密码或 token 写进 Book。

## 重启以后

GitHub CLI 的认证通常会安全保存，重启电脑或 LanCarbon 后依然有效。只有凭据被撤销、过期、删除、主动退出或切换账号时，才需要重新登录。

## 按钮看起来没有反应时

检查终端窗口是否被 LanCarbon 挡住，或是否出现在任务栏。如果安装 GitHub CLI 时 LanCarbon 仍在运行，请关闭并重启 LanCarbon。仍无终端时，可以在普通终端运行 `gh auth login`，完成后回到软件点击 **Refresh Checks**。
