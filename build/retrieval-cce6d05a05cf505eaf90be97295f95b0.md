---
title: Retrieval Models / 检索模型
short_title: Retrieval Models
description: Embedding, reranking, service configuration and local vector preparation.
authors:
  - name: Haojie Dai
keywords:
  - LanCarbon
  - Retrieval
  - Embedding
label: lc-s6-retrieval
---

# Retrieval Models

Open **Workshop → AI Settings → Retrieval**. Embedding and optional Rerank have separate service/model choices. **Use an existing connection** reuses a saved Chat or translation key without changing its Chat model list. **Separate retrieval connection** stores an independent encrypted key; choose SiliconFlow, OpenRouter or Others. Others accepts an HTTPS API base address and exact model ID. Embedding requires a compatible **/embeddings** endpoint with float vectors; Rerank requires **/rerank** with indexed relevance scores. A service may offer only one of these endpoints. Model IDs and account permissions must match the service.

1. Select an Embedding service and model, enable **Enable semantic retrieval**, and save. SiliconFlow model examples are **BAAI/bge-m3** and **Pro/BAAI/bge-m3**. Consult your service's current catalogue for availability and prices. The suggestions are not an account-access check.
2. Optionally enable **Use reranking**, select its connection and model, and save. SiliconFlow examples are **BAAI/bge-reranker-v2-m3** and **Pro/BAAI/bge-reranker-v2-m3**. Embedding and Rerank may use the same connection or different services/keys. Removing an independent key affects the retrieval roles sharing that connection and preserves Chat settings.
3. **Test Embedding** sends a built-in English sentence and checks vector dimensions. **Test Rerank** sends a built-in question and two short examples. Both use normal service billing and are recorded under their corresponding Usage purposes. **Stop** cancels a test or active retrieval task. Saving alone makes no model request.
4. In **Workshop → Usage → Model prices**, configure each retrieval model's input price per million tokens and set output to zero. For a model currently offered free, set both to zero. Provider-reported token counts and charges are used when available; missing usage remains unknown. Failed attempts and retries remain recorded. Reusing a connection automatically uses its existing billing account; independent retrieval connections can be grouped with Chat/translation in **Connections sharing this balance**. Keep a paid account tracked when only some of its models are free.

**Index tools** is an optional advanced panel. It prepares vectors only for current cached source text. Unchanged passage text is reused; changed/deleted or deselected sources are excluded from retrieval. A changed Embedding service/model has a separate vector space and needs preparation again. Local keyword ranking and semantic ranking are combined; optional Rerank orders the candidate passages. Retrieval check displays source passages and positions without generating a Chat answer. If semantic retrieval or reranking fails, the panel explicitly identifies the fallback and any incomplete preparation.

Preparing sources sends their extracted text to the selected Embedding service. A search sends the question to Embedding and selected candidate passages to Rerank when enabled. Ordinary writing and local keyword search with semantic retrieval off make no retrieval requests. Retrieval follows the computer's network and system proxy. Query instructions are normally blank; Qwen3 Embedding receives its standard retrieval query instruction automatically, and document text is not prefixed.

Vectors use a bounded **128 MB** local cache in **Data/Research/Retrieval**, with up to 40,000 passages and 8,192 dimensions. No local model files are downloaded. **Clear vector index** removes vectors while keeping original files and extracted text; preparing again may incur service charges. Clearing the text index also clears its vector cache. Completed batches survive stop/restart; an interrupted task is resumed explicitly with Prepare. Data Location carries the derived cache. Chat automatically prepares its selected sources when you send a question. Refresh Embedding models and Refresh Rerank models fetch role-specific catalogues without changing Chat models; save and test your selected IDs. See [Document Questions](knowledge.md).

---

# 检索模型

打开 **Workshop → AI Settings → Retrieval**。Embedding 和可选的 Rerank 分别选择服务与模型。**Use an existing connection** 复用已保存的 Chat 或翻译密钥，不修改 Chat 模型列表；**Separate retrieval connection** 保存独立的加密密钥，可选 SiliconFlow、OpenRouter 或 Others。Others 填入 HTTPS API 基础地址及准确模型 ID。Embedding 需要兼容 **/embeddings** 的浮点向量接口；Rerank 需要兼容 **/rerank**、返回输入序号及相关分数的接口。同一服务可能只支持其中一种接口，模型 ID 和账号权限须以平台为准。

1. 选择 Embedding 服务和模型，勾选 **Enable semantic retrieval** 并保存。SiliconFlow 模型示例为 **BAAI/bge-m3**、**Pro/BAAI/bge-m3**；可用性和价格请查平台当前目录，软件建议列表不代表账号一定有调用权限。
2. 按需勾选 **Use reranking**，选择其连接和模型并保存。SiliconFlow 示例为 **BAAI/bge-reranker-v2-m3**、**Pro/BAAI/bge-reranker-v2-m3**。两类模型可共用连接，也可使用不同服务或密钥。删除独立密钥只影响共用该连接的检索角色，保留 Chat 配置。
3. **Test Embedding** 发送一条内置英文句子并检查向量维度；**Test Rerank** 发送内置问题和两条短例文。测试按平台规则计费，分别记入对应的 Usage 用途；**Stop** 可取消测试或正在执行的检索任务。仅保存设置不会请求模型。
4. 在 **Workshop → Usage → Model prices** 设置每个检索模型每百万输入 tokens 的价格，输出价格设为零。平台当前免费的模型将输入和输出均设为零。优先使用平台返回的 tokens 和费用，缺失用量保留为未知；失败尝试和重试照实记录。复用连接自动沿用原余额账户；独立检索连接可在 **Connections sharing this balance** 与 Chat／翻译归入同一计费账户。仅部分模型免费时，保留付费账户的余额跟踪。

**Index tools** 是可选的高级工具，为已缓存且成功提取的文本准备向量。未变化片段直接复用；修改、删除或取消选取的资料退出检索。更换 Embedding 服务或模型后使用独立向量空间，需要重新准备。系统结合本地关键词排名和语义排名，并可用 Rerank 重排候选片段。Retrieval check 展示资料片段及位置，不生成 Chat 回答；语义检索、重排失败或资料尚未准备完整时会明确提示降级情况。

准备资料会将提取的正文发送给所选 Embedding 服务；检索将问题发送给 Embedding，启用 Rerank 时再发送候选片段。普通写作及关闭语义检索后的本地关键词搜索不调用检索 API；网络沿用电脑的网络与系统代理。Query instructions 通常留空，Qwen3 Embedding 自动使用标准检索问题指令，不给资料正文添加指令前缀。

向量缓存保存在 **Data/Research/Retrieval**，上限 **128 MB**，最多 40,000 个片段及 8,192 维，不下载本地模型。**Clear vector index** 仅删除向量，保留原文件及提取文本；重新准备可能再次计费。清除文本索引也会清除对应向量缓存。暂停和重启保留已完成批次，中断任务用 Prepare 明确继续；Data Location 会携带缓存。Chat 在发送资料问题后自动准备所选来源。Refresh Embedding models 与 Refresh Rerank models 分别获取对应目录，不改变聊天模型列表；选择后请保存并测试。参阅 [资料问答](knowledge.md)。
