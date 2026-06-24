# TokensFlow

统一 API 网关，一个接口调用 DeepSeek、Qwen、GLM 等国内主流大模型。

## 特性

- 统一接口：一个 API Key 调用所有模型
- 兼容 OpenAI：可直接替换现有代码
- 按量付费：通过 PayPal 充值，即付即用
- 自动交付：付款后自动生成 API Key

## 快速开始

1. 访问 https://tokensflow.net 完成支付
2. 邮箱收到 API Key
3. 直接调用

```bash
curl https://tokensflow.net/v1/chat/completions \
  -H "Content-Type: application/json" \
  -H "Authorization: Bearer 你的API Key" \
  -d '{
    "model": "deepseek-ai/DeepSeek-V4-Flash",
    "messages": [{"role": "user", "content": "你好"}]
  }'
