---
title: Working with AI Chat
---

# Working with AI Chat

Select a configured service and model, then send text. The top heading is the conversation name. Each assistant reply records its configured service and model. Use Copy for Markdown source, Stop generating to save partial output, or Retry reply to replace the last stopped or failed reply without duplicating the question.

In a mixed-model conversation, previous replies from another model are attributed references. User questions and relevant information remain available, while the current model is instructed to answer independently. The model's self-description is not proof of the upstream model identity. Repeating the exact question after a model switch omits earlier answers to that question from other models, while retaining them in the local transcript. For an independent comparison without any prior context, use separate new chats.

Response guidelines in AI Settings apply to future replies from every service. Old replies are retained as written. Chat history is local, and selected conversation text and guidelines go to the selected service. Use Choose sources to ask about Library documents, Notes or Book pages, with saved evidence and source navigation. Without sources, ordinary Chat does not automatically read those files. See [Document Questions](knowledge.md). Delete chat removes the local conversation after confirmation. Writing remains separately stored.

Expand **Evidence** below a document answer to inspect its original passages, locations and retrieval diagnostics. These diagnostics describe retrieval and do not certify every claim.

For account or network errors, check the service's key, balance, permissions and computer network. A rate limit can belong to an upstream shared service pool rather than your account. Cancel an unwanted request with Stop generating or Stop test. Successful connectivity does not guarantee continued provider availability.

Use **Choose sources** directly above the message box to select documents for the current conversation.

Chat replies use Markdown with LaTeX: `$...$` for inline formulae and `$$` on separate lines for displayed formulae. **Copy** preserves this source; paste it into a Note and use **Preview** to render the formulae. Standard LaTeX delimiters are normalized for reading and copying. Plain-text equations in an old reply are not guessed or automatically rewritten; ask for a LaTeX version if needed.

Use **Export PDF** beside the chat title to save the entire conversation. **Include Thinking** is checked by default and exports all saved reasoning, even when collapsed on screen; disable it for answers only. **Include cited evidence excerpts** adds the original passages referenced by each reply. Model names, timestamps, source titles and locations remain included; citation labels belong to their own reply. Wait for generation to finish or stop it first. Export is offline, makes no model request and defaults to the **PDFs** folder. Stopped/error replies retain their partial status; exporting does not delete the chat.

Use **Export to Note** beside the chat title to save the complete conversation as a new editable Note and open its Preview. **Include Thinking** and **Include cited evidence excerpts** work as in PDF export. Each export creates an independent snapshot with the conversation title, questions, answers, model names, timestamps and source locations. Citation links lead to that reply’s source entries inside the Note; identical labels in different replies stay separate. Thinking and original excerpts are preserved as literal text. Wait for generation to finish or stop it first. Export happens locally without a model request. Subsequent chat messages do not automatically change an exported Note.

For academic writing, request APA author-year citations explicitly. Supplied bibliographic information supports the citation text; separate **[S1]** evidence links let you inspect the source. Verify any missing bibliographic details before using a reference in a manuscript.

---

# 使用 AI Chat

选择已配置的服务和模型后发送文字，顶部直接显示会话名称。每条 AI 回复记录当时配置的服务和模型。Copy 复制 Markdown 原文，Stop generating 停止生成并保存已有文字，Retry reply 替换最后一条停止或失败的回复，不重复添加问题。

混合模型会话中，其他模型的旧回答会标注来源，作为参考传递。问题和相关信息保留，当前模型按要求独立分析。模型的自我介绍不能证明上游实际模型身份；切换模型后重复同一问题时，不向新模型发送其他模型对此题的旧答案，旧记录保留在本地；完全独立的比较可在不同新会话中发送同一问题。

AI Settings 的回答规范用于各服务后续回复，旧回复保持原样。会话记录保存在本机，所选会话文字与规范发送到所选服务。通过 Choose sources 可选择 Library 文献、Notes 或 Book 页面进行有引用的资料问答。未选择资料时，普通聊天不会自动读取这些内容。参阅 [资料问答](knowledge.md)。Delete chat 经确认后删除本地会话，写作内容单独保存。

展开资料回答下方的 **Evidence**，查看原文摘录、位置和检索诊断；这些诊断反映检索过程，不是对每个结论的正确性认证。

遇到账户或网络错误时检查平台密钥、余额、权限与电脑网络。限流可能来自上游共享服务池。用 Stop generating 或 Stop test 取消不需要的请求；连接成功并不保证平台持续可用。

点击消息输入框正上方的 **Choose sources**，选择当前聊天使用的资料。

聊天正文使用 Markdown，公式使用 LaTeX：行内公式用 `$...$`，独立公式用单独成行的 `$$`。**Copy** 保留这些源码，粘贴到 Note 后在 **Preview** 中呈现公式。常见 LaTeX 分隔符会统一处理以便阅读与复制；旧回答中的普通文本公式不会被猜测重写，如需转换可明确要求模型提供 LaTeX 版本。

点击聊天标题旁的 **Export PDF** 导出完整会话。默认勾选 **Include Thinking**，即使界面已折叠也会完整导出已保存的推理内容；取消勾选则只导出问答。**Include cited evidence excerpts** 可附加每条回复实际引用的原文摘录。逐条保留模型名称、时间及来源位置，各轮引用编号互不混淆。请先等待生成完成或停止生成；导出在本机完成，不调用模型，默认保存到 **PDFs** 文件夹。停止或失败的回复保留未完成标记，导出不会删除聊天。

点击聊天标题旁的 **Export to Note**，将完整聊天保存为新的可编辑 Note，并直接打开其预览。**Include Thinking** 与 **Include cited evidence excerpts** 的作用与 PDF 导出相同。每次导出创建独立快照，保留会话标题、问题、回答、模型名称、时间与来源位置；引用链接跳到笔记内对应回复的来源说明，不同轮次的相同编号互不混淆。Thinking 和原文摘录按原始文字保留。请先等待生成结束或停止生成；保存全程在本机完成，不调用模型，后续聊天不会自动改动已导出的 Note。

学术写作时可明确要求 APA 作者年份引用；引用文字依据资料中的书目信息，独立的 **[S1]** 证据链接用于核查原文。用于论文前请补齐并核对缺失的书目信息。
