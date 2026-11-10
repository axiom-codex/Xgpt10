<div align="center">

# 💻 Xgpt10 API Usage Guide

### ⚡ OpenAI-Compatible • Streaming Ready • Multi-Provider

[![API](https://img.shields.io/badge/🚀_API-Live-00C853?style=for-the-badge)](https://xgpt10.cloud.run)

</div>

---

## 🔗 Base Endpoint

```text
https://xgpt10.cloud.run/api/v1/chat/completions
```

> 🌐 Website: [https://xgpt10.cloud.run](https://xgpt10.cloud.run)

---

## 🔑 Authentication

All requests require your API key:

```text
Authorization: Bearer ah_your_api_key_here
```

---

## 📦 Request Format

```json
{
  "provider": "gemini",
  "model": "gemini-3.8-flash",
  "messages": [
    {"role": "user", "content": "Explain quantum computing"}
  ],
  "stream": true
}
```

### Main Parameters

| Parameter | Type | Description |
|:---|:---|:---|
| 🌐 `provider` | string | Which provider to use (gemini, groq, etc.) |
| 🤖 `model` | string | Specific model name |
| 💬 `messages` | array | Chat messages (OpenAI format) |
| 📡 `stream` | boolean | `true` = SSE streaming, `false` = full reply |

---

## ⚡ cURL Example (Streaming)

```bash
curl -N -X POST https://xgpt10.cloud.run/api/v1/chat/completions \
  -H "Authorization: Bearer ah_your_api_key_here" \
  -H "Content-Type: application/json" \
  -d '{
    "provider": "gemini",
    "model": "gemini-3.8-flash",
    "messages": [{"role": "user", "content": "Explain quantum computing"}],
    "stream": true
  }'
```

---

## 🐍 Python Example

```python
import requests

url = "https://xgpt10.cloud.run/api/v1/chat/completions"
headers = {
    "Authorization": "Bearer ah_your_api_key_here",
    "Content-Type": "application/json"
}
data = {
    "provider": "gemini",
    "model": "gemini-3.8-flash",
    "messages": [
        {"role": "user", "content": "Explain quantum computing"}
    ],
    "stream": True
}

response = requests.post(url, headers=headers, json=data, stream=True)

for line in response.iter_lines():
    if line:
        print(line.decode("utf-8"))
```

---

## 💻 JavaScript / Node.js Example

```javascript
const response = await fetch("https://xgpt10.cloud.run/api/v1/chat/completions", {
  method: "POST",
  headers: {
    "Authorization": "Bearer ah_your_api_key_here",
    "Content-Type": "application/json"
  },
  body: JSON.stringify({
    provider: "gemini",
    model: "gemini-3.8-flash",
    messages: [{ role: "user", content: "Explain quantum computing" }],
    stream: true
  })
});

const reader = response.body.getReader();
// Handle streaming chunks...
```

---

## 🌐 Supported Providers (Examples)

| Provider Code | Name |
|:---|:---|
| `gemini` | 🧠 Google Gemini |
| `groq` | ⚡ Groq |
| `openrouter` | 🔗 OpenRouter |
| `huggingface` | 🤖 Hugging Face |
| `chatgpt` | 💬 ChatGPT |
| `grok` | 🤖 Grok (xAI) |
| `kimi` | 🌟 Kimi |

> Model names depend on the provider (example: `gemini-3.8-flash`).

---

## 💡 Notes

- 🔒 Always use `https`
- 🔑 Keep your API key secret
- 📡 Streaming (`stream: true`) is recommended for better UX
- 🔗 The API is designed to be **OpenAI-compatible** for easy integration

---

<div align="center">

### 🚀 [Get Your Free API Key →](https://xgpt10.cloud.run)

✨ **One Key. All Models. Unlimited Possibilities.** ✨

</div>
