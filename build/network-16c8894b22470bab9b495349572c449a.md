---
title: Network, Proxy, and TUN Mode
short_title: Network, Proxy, and TUN Mode
description: Bilingual LanCarbon beginner tutorial.
authors:
  - name: Haojie Dai
keywords:
  - LanCarbon
  - Jupyter Book
  - MyST
label: lc-s4-network
---


# Network, Proxy, and TUN Mode

Publish talks to GitHub through several programs: the browser, GitHub CLI, Git, and LanCarbon's GitHub API request. A proxy extension that affects only the browser may let github.com open while Git still fails on port 443.

If your network can reach GitHub directly, no proxy is needed. If GitHub is blocked, unstable, or repeatedly reset:

1. Open your trusted proxy application.
2. Enable **system proxy / global proxy** or **TUN mode**, according to that application's design.
3. Confirm github.com opens in the browser.
4. Return to Publish and select **Refresh Checks**.
5. Confirm both **GitHub API** and **Git HTTPS connection** pass.
6. Publish or update while that network mode remains active.

LanCarbon does not configure or bypass network policy for you. Use only a network method permitted by your organization and location. Turn off the proxy mode afterward if that is your normal practice.

Typical network messages contain `Failed to connect to github.com port 443`, `Connection was reset`, `Recv failure`, `timed out`, `ECONNRESET`, or a failed OAuth access-token request. These messages usually describe connectivity, not damaged Book content.

Do not repeatedly click Publish while a connection is failing. Restore connectivity, select **Refresh Checks**, and retry once. GitHub may also have a service incident; check [GitHub Status](https://www.githubstatus.com/) if your connection otherwise works.

---



# 网络、代理与 TUN 模式

Publish 会通过多个程序连接 GitHub：浏览器、GitHub CLI、Git，以及 LanCarbon 的 GitHub API 请求。只影响浏览器的代理扩展，可能让 github.com 能打开，但 Git 连接 443 端口仍然失败。

如果当前网络可以直接稳定访问 GitHub，就不需要代理。如果 GitHub 无法访问、连接不稳定或反复被重置：

1. 打开你信任的代理软件。
2. 根据该软件的设计，开启 **系统代理/全局代理** 或 **TUN 模式**。
3. 确认浏览器能够打开 github.com。
4. 回到 Publish，点击 **Refresh Checks**。
5. 确认 **GitHub API** 和 **Git HTTPS connection** 都通过。
6. 在该网络模式保持开启时执行 Publish 或 Update。

LanCarbon 不会替你配置代理，也不会绕过网络管理策略。请只使用所在组织和地区允许的网络方式。操作结束后是否关闭代理，可按你的日常习惯处理。

典型网络错误包含 `Failed to connect to github.com port 443`、`Connection was reset`、`Recv failure`、`timed out`、`ECONNRESET`，或 OAuth access-token 请求失败。这些信息通常表示连接问题，不代表 Book 内容损坏。

连接失败时不要连续多次点击 Publish。先恢复网络，点击 **Refresh Checks**，再重试一次。如果本地网络正常，也可以查看 [GitHub Status](https://www.githubstatus.com/)确认 GitHub 是否发生服务故障。
