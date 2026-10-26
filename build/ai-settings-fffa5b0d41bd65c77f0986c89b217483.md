---
title: AI Connections and Models
short_title: AI Connections and Models
description: AI Connections and Models
authors:
  - name: Haojie Dai
keywords:
  - LanCarbon
label: lc-s6-ai-settings
---

# AI Connections and Models

## Service accounts and connections

You need an API Key from the service you intend to use. A website's Chat subscription does not necessarily include API access or API credit. Check the service's model catalogue, account access and API billing before choosing a model.

In **Workshop → AI Settings**, choose **SiliconFlow**, **OpenRouter** or **Others**. A connection identifies the service address and key; a model identifies which model to request through that connection. One connection can contain several saved models.

## Connection settings

1. Choose the service. SiliconFlow and OpenRouter supply preset API addresses. **Others** accepts an OpenAI-compatible Chat Completions service and lets you name the configuration and enter its API base address.
2. Copy the API Key from your service's key-management page into **API Key**. Use an API address, not the service's ordinary website address.
3. Select **Save configuration**, or **Refresh models** to save the connection and retrieve the service's model catalogue.

Use the base address and key from the same service region or account. For example, a service's domestic and international sites may have different addresses and separate credit. If the required address differs from a preset, use Others with the address documented by that service.

![AI Settings with an example connection](../assets/d659080065812a642f807c34a48d3fdc9d07708aa1901e52caaaa090a017db0b.png)

Example configuration. Model names and credentials in tutorial screenshots are demonstrations, not working account details.

## Adding and testing models

1. After **Refresh models**, choose a **Model ID** from the list, or enter the exact ID provided by the service.
2. Set a readable **Display name** and click **Add model**.
3. Choose the **Default model**, then click **Save models**.
4. Select **Test model**. A successful response confirms that this connection and model can answer a short request. You can now select it in Chat.

Refresh retrieves a catalogue; it does not add every listed model to your Chat selector or guarantee access to every model. Availability, regional access and pricing depend on the service and account. Display name is your local label; Model ID is the value sent to the service.

Saving settings alone does not generate a Chat answer. Test model makes a real service request and can incur a small fee. If testing fails, check the API address, key, model ID, account credit and network. A busy-service or rate-limit error does not necessarily mean the key is invalid.

## Saved keys and models

After saving, the key input is cleared and **Saved API key** shows only its beginning and end. Leave the input blank to keep the existing key, or enter a replacement. **Remove saved key** removes it from LanCarbon; revoke it on the service's website if you want to disable that key entirely.

Use **Remove** beside a saved model and save the model list to remove it from future selection. Existing chat history remains. Keys are encrypted for the current Windows account; see [backup and recovery](../01-getting-started/recovery.md) before moving to another computer or Windows account.

## Response guidelines

Expand **Response guidelines · all chat models** to edit the shared system prompt. Use it for stable preferences such as professional, concise wording, no decorative emoji and clear mathematical notation. **Save guidelines** applies the text to future replies; it does not rewrite existing messages. **Restore default guidelines** fills the default text; save it to apply.

Translation has its own prompt in Translation Settings. Current full-text document questions use your selected Chat model; you do not need to configure Embedding or Rerank to start. The **Retrieval** area contains advanced tools, including local OCR maintenance, and is separate from the beginner Chat setup.

---

# AI 连接与模型

## 服务账户与连接

首先需要从拟使用的平台获取 API Key。网页聊天订阅不一定包含 API 调用权限或额度，请先确认平台的模型目录、账户权限和 API 计费规则。

打开 **Workshop → AI Settings**，选择 **SiliconFlow**、**OpenRouter** 或 **Others**。“连接”指定服务地址和密钥，“模型”指定通过该连接请求的模型。一个连接可以保存多个模型。

## 连接设置

1. 选择服务。SiliconFlow、OpenRouter 提供预设 API 地址；**Others** 用于兼容 OpenAI Chat Completions 的服务，可填写配置名称和 API 地址。
2. 从平台密钥管理页面复制 API Key，粘贴到 **API Key**。接口地址应使用 API 地址，而不是平台的普通网页地址。
3. 点击 **Save configuration**；也可以点击 **Refresh models**，保存连接并获取平台模型目录。

接口地址与密钥应来自对应的服务区域和账户。例如，同一平台的国内站与国际站可能使用不同地址、独立额度。需要的地址与预设不同时，可在 Others 中按平台说明填写。

![使用示例连接的 AI Settings](../assets/d659080065812a642f807c34a48d3fdc9d07708aa1901e52caaaa090a017db0b.png)

图中是演示配置。教程截图中的模型名称和凭据不能直接作为真实账户配置使用。

## 添加与测试模型

1. **Refresh models** 后，从列表选择 **Model ID**，或手动输入平台提供的准确 ID。
2. 填写便于辨认的 **Display name**，点击 **Add model**。
3. 选择 **Default model**，点击 **Save models**。
4. 点击 **Test model**。成功回复表明该连接和模型能够完成一次短请求，随后可以在 Chat 中选用。

Refresh 获取的是平台目录，并不把其中所有模型加入聊天选项，也不保证账户能使用全部模型。模型可用性、地区权限和价格取决于平台及账户。Display name 是本地显示名称，Model ID 才是发送给服务商的标识。

只保存设置不会生成聊天回答；Test model 会请求真实服务，可能产生少量费用。失败时依次检查接口地址、密钥、模型 ID、账户额度和网络。服务繁忙或限流错误不一定意味着密钥无效。

## 已保存的密钥与模型

保存后输入框会清空，**Saved API key** 只显示密钥开头和结尾。留空可保留已有密钥，输入新值则替换。**Remove saved key** 仅从 LanCarbon 移除密钥；若要彻底停用，还需到平台网站撤销该密钥。

点击模型旁的 **Remove** 并保存模型列表，即可从后续选择中移除它，原有聊天记录仍保留。密钥按当前 Windows 账户加密；迁移电脑或 Windows 账户前，请阅读[备份与恢复](../01-getting-started/recovery.md)。

## 回答规范

展开 **Response guidelines · all chat models**，编辑共用的系统提示词。适合写入长期偏好，例如表达专业简洁、不使用装饰性 emoji、公式使用规范格式。点击 **Save guidelines** 后作用于后续回答，不会改写已有消息。**Restore default guidelines** 会填入默认内容，保存后才应用。

翻译在 Translation Settings 中使用独立提示词。当前全文资料问答使用选定的 Chat 模型，开始使用不需要先配置 Embedding 或 Rerank。**Retrieval** 区域提供高级工具，包括本地 OCR 维护，不属于新手聊天配置的必经步骤。
