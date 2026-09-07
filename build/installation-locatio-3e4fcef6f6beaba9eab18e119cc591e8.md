---
title: Installation Location and Managed Folders
short_title: Installation Location and Managed Folders
description: Choose the LanCarbon root and understand its Application, Data, Config, Cache, Temp, Builds, and Exports folders.
authors:
  - name: Haojie Dai
keywords:
  - LanCarbon
  - installation
  - storage
  - backup
label: lc-s1-storage
---

# Choosing the Installation Location and Understanding LanCarbon Folders

LanCarbon keeps the files it manages under one **LanCarbon root folder**. This makes the application easier to move, back up, inspect, and remove without scattering large caches and Book builds across the system drive.

## The default location

On a Windows computer with a D drive, the installer proposes:

```text
D:\LanCarbon
```

Choose this **LanCarbon root**, not its future `Application` child. The installer creates the child folders and installs the program at `D:\LanCarbon\Application` automatically.

If Windows has no D drive, the installer proposes a LanCarbon folder inside your current Windows user area. The directory page always shows the actual choice before installation.

## Choosing a different drive or parent folder

You may place the root elsewhere, for example:

```text
E:\Writing\Research\LanCarbon
```

For a first installation, two rules apply:

1. The final folder name must be exactly `LanCarbon`.
2. The selected `LanCarbon` folder must be empty.

You may create the empty folder before running the installer or type a new path on the installer directory page. Do not select `Application`, `Data`, or a general folder containing unrelated files.

An existing LanCarbon root containing `Data\notes.json` is recognized for an upgrade or a deliberate migration. The installer keeps the sibling data folders and updates the program inside `Application`.

## Folder map

After installation, the selected root has this structure:

```text
LanCarbon\
├─ Application\
├─ Data\
├─ Config\
├─ Cache\
├─ Temp\
├─ Builds\
└─ Exports\
```

| Folder | Purpose | Backup priority |
|---|---|---|
| `Application` | LanCarbon program files and bundled resources. | Reinstallable; normally omit from a content-only backup. |
| `Data` | Notes, Books, page text, imported images, attachments, and bibliography files. | Essential. This is your primary content. |
| `Config` | Window preferences, the selected Data Location, and remembered Build and Export locations. | Recommended if you want the same setup after restoration. |
| `Cache` | Reusable runtime material, including the bundled Jupyter Book theme cache. | Optional; LanCarbon can recreate it. |
| `Temp` | Temporary Book preparation and GitHub publishing checkouts. | Do not back up. Completed operations remove their temporary working folders. |
| `Builds` | The default parent for local websites produced by Build. | Optional but useful when you want to keep built HTML. Source content remains in Data. |
| `Exports` | The default starting place for independent source copies made with Export. | Back up any export you intentionally keep. Each export still requires an empty destination folder. |

## What uses the C drive

Choosing a D- or E-drive root directs LanCarbon's managed data, configuration, cache, temporary work, builds, and Export starting location to that drive. Windows itself may still use the system drive briefly for installer bookkeeping, shortcuts, registry information, crash handling, or operating-system temporary activity. LanCarbon cannot redirect those Windows services, but it no longer chooses a C-drive application-data folder for its own persistent cache.

Python, Jupyter Book, Git, and GitHub CLI are separate tools. Their installers decide their locations; changing the LanCarbon root does not move them. See **Tools Required from Writing to Publishing** for their installation and verification.

## Backup and migration

The safest complete backup is a copy of the entire LanCarbon root while the application is closed. For a smaller content backup, keep at least `Data`; include `Config` if you also want remembered locations and window preferences.

Before moving the root manually:

1. Close LanCarbon and wait for the window to disappear.
2. Copy the whole `LanCarbon` folder to the new drive.
3. Install LanCarbon into that existing root, or reinstall and select the copied root.
4. Open the application and verify several Notes, the Book table of contents, Resources, and Data Location before deleting the old copy.

Avoid moving individual files while LanCarbon is running. A Book can reference managed resources, and its Build and Publish records are stored with the workspace and configuration.

## Uninstalling

The program is installed in `Application`; your writing is stored beside it in `Data`. Before uninstalling, make a backup of the root. After uninstalling, inspect the root before deleting anything that remains. Retained `Data`, `Builds`, or `Exports` may still contain work you want.

---

# 选择安装位置并了解 LanCarbon 文件夹

LanCarbon 会把由软件管理的文件集中放在一个 **LanCarbon 根目录** 下。这样可以减少系统盘占用，也便于迁移、备份、检查和清理。

## 默认位置

Windows 电脑存在 D 盘时，安装器默认建议：

```text
D:\LanCarbon
```

安装时请选择这个 **LanCarbon 根目录**，不要选择未来的 `Application` 子文件夹。安装器会自动创建全部子目录，并把程序安装到 `D:\LanCarbon\Application`。

如果电脑没有 D 盘，安装器会在当前 Windows 用户目录中建议一个名为 LanCarbon 的文件夹。正式安装前，目录页面会显示实际选择的位置。

## 自定义其他位置

可以选择其他磁盘或更深的父目录，例如：

```text
E:\Writing\Research\LanCarbon
```

首次安装需要同时满足两项规则：

1. 最后一级文件夹必须准确命名为 `LanCarbon`。
2. 所选的 `LanCarbon` 文件夹必须为空。

可以提前创建这个空文件夹，也可以直接在安装器的目录页面输入新路径。不要选择 `Application`、`Data`，也不要选择存有其他无关文件的通用文件夹。

如果根目录中已经存在 `Data\notes.json`，安装器会把它识别为升级或主动迁移的 LanCarbon 数据。此时同级数据目录会保留，程序只在 `Application` 中安装或更新。

## 目录结构

安装完成后，所选根目录的结构如下：

```text
LanCarbon\
├─ Application\
├─ Data\
├─ Config\
├─ Cache\
├─ Temp\
├─ Builds\
└─ Exports\
```

| 文件夹 | 用途 | 备份建议 |
|---|---|---|
| `Application` | LanCarbon 程序文件和随软件提供的资源。 | 可以重新安装；只备份内容时通常不需要。 |
| `Data` | Notes、Books、页面正文、导入的图片、附件和参考文献文件。 | 必须备份，这是最主要的内容。 |
| `Config` | 窗口偏好、Data Location，以及每本 Book 记住的 Build 和 Export 位置。 | 希望恢复原有使用状态时建议备份。 |
| `Cache` | 可重复生成的运行缓存，包括随安装包提供的 Jupyter Book 主题缓存。 | 可选，LanCarbon 可以重新生成。 |
| `Temp` | Build 准备过程和 GitHub Publish 的临时工作目录。 | 不需要备份；正常完成或失败后会清理对应临时目录。 |
| `Builds` | Build 生成本地网站时的默认父目录。 | 可选；需要保留已构建 HTML 时可以备份，源内容仍在 Data 中。 |
| `Exports` | Export 独立源文件副本时的默认起始位置。 | 有意保留的导出副本可以备份；每次 Export 仍需要选择空目标文件夹。 |

## C 盘还会发生什么

选择 D 盘或 E 盘根目录后，LanCarbon 自己管理的数据、配置、缓存、临时发布文件、Build 结果和 Export 起始位置都会优先位于所选磁盘。Windows 仍可能为了安装记录、快捷方式、注册信息、崩溃处理或系统临时操作而短暂使用系统盘，这些属于操作系统行为，LanCarbon 无法全部重定向。不过，LanCarbon 不再主动把自己的长期缓存放到 C 盘的应用数据目录中。

Python、Jupyter Book、Git 和 GitHub CLI 是独立工具，它们由各自的安装器决定位置。更改 LanCarbon 根目录不会移动这些工具。安装与检查方法请阅读 **Tools Required from Writing to Publishing**。

## 备份与迁移

最稳妥的完整备份方式是在关闭软件后复制整个 LanCarbon 根目录。如果只备份写作内容，至少保留 `Data`；希望同时恢复记住的路径和窗口偏好时，再保留 `Config`。

手动迁移前建议按以下顺序操作：

1. 关闭 LanCarbon，确认窗口已经完全消失。
2. 把整个 `LanCarbon` 文件夹复制到新磁盘。
3. 把软件安装到这个已有根目录，或重新安装并选择复制后的根目录。
4. 打开软件，检查几篇 Notes、Book 目录、Resources 和 Data Location；确认无误后再处理旧副本。

不要在 LanCarbon 运行时移动其中的单个文件。Book 可能引用受管理资源，Build 和 Publish 记录也会与工作区及配置共同保存。

## 卸载

程序位于 `Application`，写作数据位于同级的 `Data`。卸载前请先备份根目录。卸载完成后，在删除残留目录前先检查其中内容；保留下来的 `Data`、`Builds` 或 `Exports` 仍可能包含需要的作品。
