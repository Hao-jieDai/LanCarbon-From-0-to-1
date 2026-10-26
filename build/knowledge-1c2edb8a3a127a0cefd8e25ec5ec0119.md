---
title: Questions about Your Knowledge Library
short_title: Questions about Your Knowledge Library
description: Questions about Your Knowledge Library
authors:
  - name: Haojie Dai
keywords:
  - LanCarbon
label: lc-s6-knowledge
---

# Questions about Your Knowledge Library

Use source-based Chat to locate information, explain a passage, compare documents and develop reading notes. It brings together Library documents and your own Notes and Book pages. This is often called retrieval-augmented generation, or RAG; you do not need to manage an index before asking your first question.

Configure a Chat model first. The current full-text question workflow prepares readable source text locally and sends it, your question and relevant conversation context to that model. **Embedding and Rerank are not prerequisites for this workflow.** It does not perform live web searches or automatically obtain new papers.

## Source selection

Open a Chat and select **Choose sources** immediately above the message box.

| Source | How to select it |
| --- | --- |
| **Notes** | Choose individual writing notes. |
| **Books** | Expand a Book into chapters and pages; select a whole Book, a chapter or individual pages. |
| **Library** | Expand folders and subfolders, then select documents or a folder. |

![Selecting sources for a conversation](../assets/2d1d4b5aeacbc660195824c0657ba89614d85b1d2ea59a356ba69d5162df05be.png)

A sample source selection. Expanding a branch and selecting its contents are separate actions.

Use the arrows to expand a branch and the checkboxes to select it. Partial selection is shown on parent branches. Searching keeps matching items visible with their parent locations. **Include linked attachments** also follows supported attachments referenced by the selected writing. **Show built-in content** makes the official tutorial available as a source; it is hidden by default.

The selection belongs to this chat. Whole-Book and folder selections can include later additions; individual page choices keep their selected pages. Use **Clear sources** for ordinary Chat without attached knowledge sources. **Import PDF / EPUB**, or dropping files into Chat, adds or reuses Library documents and selects them for this conversation.

There is no fixed 20-source limit for a chat. The Library's 20-file import batch limit is a different rule. Actual source preparation and sending still have size and model-context limits. If LanCarbon reports that the selection is too large, narrow it to the documents relevant to your question or start a fresh conversation. Selecting the entire library is rarely necessary.

## Questions and follow-up context

After choosing sources, send a concrete question. Preparation happens automatically. PDFs and reflowable EPUBs are parsed, and scanned PDF pages may need [OCR](../06-library/reading.md). Large scans take longer to prepare than text documents.

For two papers on a related subject, a useful conversation might be:

1. “What research question does each paper answer, and what do they measure?”
2. “Why do their estimates differ? Compare their assumptions and study boundaries.”
3. “Explain the equation used in the second paper and define each variable.”
4. “Which findings could support a short comparison paragraph in my literature review?”

You do not need a rigid question format. Use names or titles when a pronoun such as “that paper” would be ambiguous. Keep a follow-up in the same chat when it depends on the preceding exchange. Start a new chat for an unrelated topic or a clean comparison of models.

## Citations and original sources

Source-linked answers include citations and an **Evidence** area. Expand it to inspect passages and use **Open source** or the citation link to return to the relevant document page, EPUB location or writing page. This connects the answer to material you can read yourself.

Check consequential numbers, units, formula variables and the parties being compared against the original. An excerpt citation identifies supporting material; it does not certify every interpretation in the answer. OCR labels identify recognized text that may need closer inspection. If a source is missing or unreadable, repair or replace it before relying on that part of an answer.

Some monetary calculations show an original amount alongside a local conversion or calculation. **Check amounts** can identify calculations that could not be completed. These tools check amount matching and arithmetic; they do not decide whether the chosen scenario or economic entity is the right one.

## Saving reading notes

Use **Export to Note** to save the conversation, optionally including Thinking and cited passages. Edit the result into your own reading note, keep its source references and add it to an appropriate Book. See [Working with AI Chat](chat.md) for export options.

## Data sent and request costs

Source preparation and OCR run locally, but answering sends selected readable material to your chosen AI service. Full-text questions can use substantially more input tokens than ordinary Chat, and follow-ups can send source material again. Choose a focused scope and inspect [Usage](usage.md) when learning how much your reading sessions cost.

---

# 基于个人知识库提问

资料问答用于定位信息、解释段落、比较文档与整理阅读笔记。来源既可以是 Library 文献，也可以是自己的 Notes 和 Book 页面。这类能力通常称为检索增强生成，即 RAG；开始提问前不需要先手动管理索引。

首先配置一个 Chat 模型。当前全文问答流程在本地准备可读的来源文字，再将文字、问题和相关对话上下文发送给该模型。**Embedding 和 Rerank 不是此流程的使用前提**。它不会执行实时联网搜索，也不会自动获取新文献。

## 资料来源与选择范围

打开 Chat，点击消息输入框正上方的 **Choose sources**。

| 来源 | 选择方式 |
| --- | --- |
| **Notes** | 选择独立笔记。 |
| **Books** | 逐层展开 Book、章节和页面，可以选择整本书、章节或单页。 |
| **Library** | 展开文件夹与子文件夹，选择文档或整个文件夹。 |

![为聊天选择资料来源](../assets/2d1d4b5aeacbc660195824c0657ba89614d85b1d2ea59a356ba69d5162df05be.png)

示例来源选择界面。展开目录与勾选其中内容是不同操作。

点击箭头展开目录，使用选择框勾选；只选中部分内容时，上级目录显示部分选中状态。搜索会保留匹配内容及其上级位置。**Include linked attachments** 同时纳入选定写作内容所引用的受支持附件。内置教程默认不参与选择，开启 **Show built-in content** 后才会显示。

来源范围属于当前聊天。整本 Book 或整个文件夹的选择可以纳入后来新增内容；单独勾选页面时保留选定页面。**Clear sources** 清除来源，恢复不附加知识资料的普通聊天。**Import PDF / EPUB** 或向 Chat 拖入文件，会导入或复用 Library 文档，并把它们加入当前聊天来源。

聊天没有固定的 20 项来源限制；Library 每批导入 20 个文件是另一条规则。但资料准备、发送体积和模型上下文仍有容量限制。软件提示范围过大时，请缩小到与问题相关的资料，或另开聊天。通常无需把整个资料库全部选上。

## 提问与追问

选择来源后发送具体问题，软件会自动准备资料。PDF 与可重排 EPUB 会提取文字，扫描 PDF 可能需要 [OCR](../06-library/reading.md)。大型扫描件的准备时间通常长于文字文档。

比较两篇相关论文时，可以这样进行多轮对话：

1. “两篇文章分别回答什么研究问题，衡量的对象是什么？”
2. “为什么估计结果不同？比较它们的假设和研究边界。”
3. “解释第二篇文章使用的公式，并说明各变量含义。”
4. “哪些结果适合放进文献综述中的一段比较？”

不需要严格的提问模板。“那篇文章”等指代不清时，使用作者或标题。依赖前文的追问留在同一聊天；无关主题或需要独立比较模型时，新建聊天更清楚。

## 引用与原文定位

资料回答提供来源引用和 **Evidence** 区域。展开后查看原文片段，通过 **Open source** 或引用链接返回对应 PDF 页、EPUB 位置或写作页面，使回答与可直接阅读的材料相连。

对结论影响较大的数字、单位、公式变量和比较主体，应回到原文检查。引用标识提供支持材料，不代表回答中的所有解释都经过认证。OCR 标识说明片段来自文字识别，需要时更仔细核对；来源缺失或无法读取时，先修复或替换该来源。

部分金额计算会同时显示原始金额和本地换算或计算结果。**Check amounts** 可以指出未能完成的计算。这些工具检查金额匹配与算术，不负责判断所选情景或经济主体是否正确。

## 保存阅读笔记

使用 **Export to Note** 保存对话，可按需包含 Thinking 和引用片段。将结果编辑为自己的阅读笔记，保留来源，再加入合适的 Book。导出选项见[使用 AI Chat](chat.md)。

## 发送内容与请求费用

资料准备和 OCR 在本地运行，但生成回答时会将选定的可读材料发送给你配置的 AI 服务。全文问答的输入 Token 可能明显多于普通聊天，追问也可能再次发送资料。初次使用时，选择聚焦的来源范围，并结合 [Usage](usage.md)了解阅读对话的实际用量。
