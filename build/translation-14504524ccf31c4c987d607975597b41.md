---
title: Selection Translation
short_title: Selection Translation
keywords:
  - Translation
label: lc-s6-translation
---

# Selection Translation

1. Open **Workshop → Translation Settings**. With **Use an existing AI connection**, select a service and a model already saved in AI Settings. The saved key and model display name are reused; this mode has no model catalogue refresh or editable model fields. To add a dedicated translation service/model, choose **Separate translation connection**, configure SiliconFlow, OpenRouter or Others, then use **Refresh translation models** or enter its exact Model ID and display name. Refresh reads a platform catalogue; account access and pricing still need checking.
2. **Save translation settings**, then **Test translation**. The result beside the buttons shows **Translation test succeeded**, the selected service/model, the fixed English sentence **Climate change affects investment.**, and its Chinese translation. **Stop translation test** cancels a running test. Testing makes a real request even with automatic translation off. The editable **Translation prompt** applies only to translation; model format adaptation is automatic. The default asks for accurate academic Chinese without explanations or emoji. English within this prompt field can also be selected for translation without changing its contents.
3. Translation starts **off** each time LanCarbon opens. Enable the sidebar **Translate** switch or press **Ctrl+Alt+T**. Select an English word, phrase or short passage in Notes/Books **Edit** or **Preview**, Workshop, Library or selectable interface text. After selection settles, the floating panel shows the selected English and Chinese translation. Drag its header to move it; the position is remembered. Close the panel or use the switch/shortcut to disable automatic requests. Passwords, API keys and connection addresses are excluded.
4. Select at most **1,600 characters / 250 words**. Only the selection and translation instructions are sent, without the whole Note, Book or Chat. New selections cancel earlier translation requests. Cancellation cannot undo charges already incurred upstream.
5. Repeated selections with the same saved service/model/prompt reuse local results without another API call. **Saved translations → Clear translation cache** clears only the translation cache, limited to **1,000 results / 5 MB**, stored under **Data/Research/Translation**. Translation and manual tests appear in **Usage → Purpose: Translation**; locally reused results do not add tokens or requests. Configure the translation model's price in **Model prices** when the service does not report costs. Dedicated keys have masked previews and **Remove translation key**; blank key inputs retain the saved key.

6. Translation appears progressively as the service sends text. The waiting timer distinguishes waiting from receiving text. Use **Stop** to cancel or **Retry translation** after a failure; retries are manual. Clicking without selecting another passage does not stop translation. Partial or failed results are not saved in the cache. The service may still take time to send its first text.

7. After **Test translation**, expand **Response time** to compare local request setup, waiting for the first translated text, and total time. This uses the same test request and sends no extra request.

---

# 选词翻译

1. 打开 **Workshop → Translation Settings**。选择 **Use an existing AI connection** 时，仅选择服务与 AI Settings 已保存的模型，密钥和显示名称沿用原配置；该模式不提供目录刷新或模型字段编辑。新增独立的翻译服务／模型时，选择 **Separate translation connection** 配置 SiliconFlow、OpenRouter 或 Others，再 **Refresh translation models** 或手填准确的 Model ID 与显示名称。刷新读取平台目录，可调用权限与价格仍需核对。
2. **Save translation settings → Test translation**。按钮附近的结果明确展示 **Translation test succeeded**、服务／模型、固定原句 **Climate change affects investment.** 与中文译文。**Stop translation test** 取消正在进行的测试；自动翻译关闭时也可手动测试，会产生真实请求。可编辑的 **Translation prompt** 仅用于翻译，所需模型格式自动适配；默认要求准确、专业、只输出简体中文且不用 emoji。提示词输入框中的英文也可选取翻译，原内容不受修改。
3. 每次启动默认**关闭**。点击侧栏 **Translate** 或按 **Ctrl+Alt+T** 开启后，在 Notes／Books 的 **Edit** 或 **Preview**、Workshop、Library 及可选取的界面文字中选择英文单词、词组或短句。选取稳定后浮窗显示原文与中文；拖动标题栏可移动并记住位置。关闭浮窗或使用开关／快捷键停止自动调用。密码、API Key 与接口地址不参与翻译。
4. 单次最多 **1,600 字符／250 词**，仅发送选取内容与翻译要求，不附带整篇 Note、Book 或聊天。新的选取取消旧翻译请求；取消不能撤销上游已经发生的费用。
5. 相同来源、模型、提示词的重复选取复用本地结果，不再次请求 API。**Saved translations → Clear translation cache** 仅清除翻译缓存，位于 **Data/Research/Translation**，上限 **1,000 条／5 MB**。翻译及手动测试在 **Usage → Purpose: Translation** 中统计；本地复用不增加请求与 Token。服务不返回费用时，在 **Model prices** 配置翻译模型价格。独立密钥显示掩码，可用 **Remove translation key** 清除本地保存；输入框留空保留原密钥。


6. 服务返回文字时译文会逐步显示，计时提示区分等待与正在接收。可点击 **Stop** 取消，失败后点击 **Retry translation** 手动重试；不会自动重试。未选取新文字的普通点击不会停止翻译。未完成或失败的结果不写入缓存；服务端首次返回仍可能需要等待。

7. **Test translation** 完成后，展开 **Response time** 可查看本地请求准备、等待首段译文及总耗时。统计来自本次测试，不产生额外请求。
