---
title: AI Connections and Models
---

# AI Connections and Models

1. Open **Workshop → AI Settings** and choose **SiliconFlow**, **OpenRouter** or **Others**. Presets supply their base addresses. Others supports OpenAI-compatible Chat Completions services and additional named configurations.
2. Paste the service's **API Key** and select **Refresh models**, or enter an exact **Model ID** and **Display name**, then **Add model → Save models**. Choose a **Default model**. Use the platform catalogue for current model IDs and account permissions.
3. Saved keys appear as **Configured**, showing their first four and last four characters with the middle hidden. Leave the key input blank to retain it, or enter a replacement and save. **Remove saved key** asks for confirmation and removes only the local key, preserving models and chats. Revoke the key separately at the service when required.
4. Expand **Response guidelines · all chat models** to edit the shared **System prompt**, then select **Save guidelines**. **Restore default guidelines** fills the default; save to apply it. Defaults request professional, accurate, calm, neutral and concise responses, without emoji or decorative language, and distinguish facts from interpretation and uncertainty. These instructions apply to future replies across all services; they do not rewrite history or guarantee identical model quality.
5. **Test model** saves the connection and makes a small request. **Stop test** cancels a running test. Connections follow the computer's network and system proxy; normal service charges apply.
6. In **Chat**, select **service · model** and send text. **Enter** sends; **Shift+Enter** inserts a line break. Use **Stop generating**, **Retry reply** and **Copy**. Markdown, code and mathematics are rendered; provided reasoning is folded separately. The heading shows the actual conversation title.
7. Use **New chat**, **Rename chat** and **Delete chat** to manage local conversations. Switching models retains relevant context, but earlier replies from other models are explicitly attributed reference material. The current model is asked to answer independently, using its configured model ID for identity questions. Similar answers alone do not establish which model was used; check each reply's recorded service/model. When the same question is repeated after switching models, earlier answers from other models to that exact question are omitted from the request and kept locally. Use a separate chat for a comparison without any prior context.

SiliconFlow uses base address `https://api.siliconflow.cn/v1`; OpenRouter uses `https://openrouter.ai/api/v1`. Use **Refresh models** or your platform's catalogue for current IDs. The OpenRouter model `meta-llama/llama-4-maverick` can be added manually when available to your account.

Keys remain encrypted for the current Windows account in **Config/ai-settings.json**; only masked previews reach the interface. Moving to another Windows account may require re-entry. Back up the complete LanCarbon home folder, including Config, Cache and Library, together with any separately selected Data location. Conversations are local in **Data/Research/Chats/chats.json**. Switching to Notes or Books lets generation continue; closing LanCarbon stops it and preserves partial replies. Chat submits your conversation text and response guidelines; Notes, Books and Library files are not automatically attached. PDF reading is available in Library; EPUB reading, retrieval and literature workflows follow separately.

---

# AI 连接与模型

1. 打开 **Workshop → AI Settings**，选择 **SiliconFlow**、**OpenRouter** 或 **Others**。前两项预填 API 地址；Others 支持兼容 OpenAI Chat Completions 的服务，也可添加多个命名配置。
2. 填入服务的 **API Key** 后点击 **Refresh models**，或填写准确的 **Model ID** 与 **Display name**，点击 **Add model → Save models**，并选择 **Default model**。通过平台目录确认当前模型 ID 与账号调用权限。
3. 已保存密钥显示 **Configured**，仅展示前四位和后四位，中间隐藏。密钥输入栏留空保留原密钥，填写新密钥并保存可替换。**Remove saved key** 经确认后仅清除本地保存的密钥，保留模型配置与会话；需要撤销平台上的密钥时另到平台操作。
4. 展开 **Response guidelines · all chat models**，编辑共用的 **System prompt**，点击 **Save guidelines** 保存。**Restore default guidelines** 填入默认内容，保存后生效。默认要求专业准确、冷静中立、简洁高效，不使用 emoji 或装饰性表达，区分事实、解释与不确定性。规范用于各服务后续回复，不改写旧记录，也不保证不同模型质量相同。
5. **Test model** 保存配置并发送小型请求，运行期间可以 **Stop test**。连接跟随电脑网络与系统代理，可能产生平台正常费用。
6. 在 **Chat** 中选择 **服务 · 模型** 并发送文字。**Enter** 发送，**Shift+Enter** 换行。使用 **Stop generating**、**Retry reply** 与 **Copy**；支持 Markdown、代码和公式，提供的推理文字单独折叠。顶部直接显示会话标题。
7. **New chat**、**Rename chat** 和 **Delete chat** 管理本地会话。切换模型保留相关上下文，但其他模型的旧回答会标注来源，作为参考资料传递。当前模型按自己的配置 ID 回答身份问题，并独立分析新问题。回答相似不能单独证明调用了哪个模型，应查看回复记录的服务和模型；切换模型后重复同一问题时，不发送其他模型对此题的旧答案，旧记录仍保留在本地；完全独立的比较可另建会话。

SiliconFlow 地址为 `https://api.siliconflow.cn/v1`，OpenRouter 地址为 `https://openrouter.ai/api/v1`。通过 **Refresh models** 或平台目录获取当前准确 ID；账号可用时可以手动添加 OpenRouter 模型 `meta-llama/llama-4-maverick`。

密钥仍使用当前 Windows 账户加密，保存在 **Config/ai-settings.json**，界面只接收掩码。迁移 Windows 账户后可能需要重填；备份时保留完整 LanCarbon 文件夹（包括 Config、Cache 和 Library），另选的数据目录也需同时备份。会话位于 **Data/Research/Chats/chats.json**；切到 Notes 或 Books 后生成继续，关闭软件会停止生成并保存已有回复。Chat 提交会话文字与回答规范，Notes、Books 和 Library 文件不会自动附加。PDF 可在 Library 内阅读；EPUB 阅读、检索与文献工作流另行提供。

