# Xgpt10 — Unified AI Key Platform

**One API Key for All Free & Live AI Models**

Live Website: **[https://xgpt10.cloud.run](https://xgpt10.cloud.run)**

---

## About the Project

**Xgpt10 (API Hub)** is a powerful unified AI platform that lets developers access multiple free and live AI models through a **single API key**.

Instead of managing separate keys for every provider, you get one OpenAI-compatible endpoint that routes your requests to the best free models available.

### Key Highlights

| Feature                  | Details                                      |
|--------------------------|----------------------------------------------|
| **Unified Providers**    | 7+ providers                                 |
| **Live Free Models**     | 20+ models                                   |
| **Gateway Latency**      | < 15ms                                       |
| **Streaming**            | Full SSE (Server-Sent Events) support        |
| **API Compatibility**    | OpenAI-compatible `/v1/chat/completions`     |
| **Auth**                 | Firebase Auth + Google Cloud Infrastructure  |

---

## Documentation

| Document | Description |
|----------|-------------|
| [Features](docs/FEATURES.md) | Complete list of all website features |
| [How to Get API Key](docs/HOW_TO_GET_API_KEY.md) | Step-by-step guide to create your API key |
| [API Usage](docs/API_USAGE.md) | cURL, Python, JavaScript examples |
| [Release Notes](RELEASE_NOTES.md) | v1.0.0 release notes |

---

## Supported Providers & Models

You can query these providers through a single endpoint:

- **Google Gemini** (including Gemini Flash)
- **Groq**
- **OpenRouter**
- **Hugging Face**
- **ChatGPT**
- **Grok** (xAI)
- **Kimi**

More providers and models are being added continuously.

---

## Quick Start — Example API Call

```bash
curl -N -X POST https://api-hub.cloud/api/v1/chat/completions \
  -H "Authorization: Bearer ah_your_api_key_here" \
  -H "Content-Type: application/json" \
  -d '{
    "provider": "gemini",
    "model": "gemini-3.8-flash",
    "messages": [{"role": "user", "content": "Explain quantum computing"}],
    "stream": true
  }'
```

You can also use the same endpoint with Python, JavaScript, or any OpenAI-compatible client library.

Full examples → [API Usage Guide](docs/API_USAGE.md)

---

## How to Create API Key

1. Go to [https://xgpt10.cloud.run](https://xgpt10.cloud.run)
2. Sign in with Google / GitHub / X / Email (or use Instant Preview)
3. Open Developer Console
4. Click **Generate API Key**
5. Copy your key (`ah_...`) and use it in requests

Detailed guide → [How to Get API Key](docs/HOW_TO_GET_API_KEY.md)

---

## Developer Console Features

Visit **[https://xgpt10.cloud.run](https://xgpt10.cloud.run)** to:

- Sign in with **Google** (1-Click + Biometric Passkey support)
- Sign in with **GitHub**
- Sign in with **Twitter (X)**
- Sign in with **Email**
- Get an **Instant Developer Preview** (no sign-in required)
- Generate Instant API Keys
- Stream inference live
- Route requests across multiple providers easily

**Security**: Protected with Firebase Auth and Google Cloud Infrastructure.

---

## Why Xgpt10?

- **Cost-effective** — Access high-quality free tier models without managing multiple accounts
- **Simple integration** — One OpenAI-compatible endpoint
- **Fast** — Gateway latency under 15ms
- **Streaming ready** — Native SSE support for real-time responses
- **Developer friendly** — Instant keys and live console

---

## Links

- **Website**: [https://xgpt10.cloud.run](https://xgpt10.cloud.run)
- **GitHub**: [https://github.com/sumitjilowa34-oss/Xgpt10](https://github.com/sumitjilowa34-oss/Xgpt10)

---

**Made for developers who want free, fast, and simple access to multiple AI models.**
