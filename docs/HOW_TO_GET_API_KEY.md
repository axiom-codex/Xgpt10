<div align="center">

# 🔑 How to Create API Key on Xgpt10

### ✨ Get your free unified API key in under 1 minute

[![Get Key](https://img.shields.io/badge/🚀_Get_API_Key-xgpt10.cloud.run-00D9FF?style=for-the-badge)](https://xgpt10.cloud.run)

</div>

---

## ⚡ Method 1: Instant Developer Preview (No Sign-In)

```text
1. 🌐 Go to https://xgpt10.cloud.run
2. 👉 Click "Instant Developer Preview (No Sign-In Needed)"
3. ✨ You get temporary access to try the platform
4. 📋 Generate or view a sample API key for testing
```

> 💡 Best for **quick testing**.

---

## 🌟 Method 2: Sign In & Get Permanent API Key (Recommended)

### Step ① — Open the Website
🌐 Visit → **[https://xgpt10.cloud.run](https://xgpt10.cloud.run)**

### Step ② — Sign In
Choose any login method:

| Method | Details |
|:---|:---|
| 🔴 **Google** | 1-Click + Biometric Passkey supported |
| 💻 **GitHub** | Quick developer login |
| 🐦 **Twitter (X)** | Social login |
| 📧 **Email** | Create account or login |

### Step ③ — Open Developer Console
After login you will see the **💻 Developer Console**.

### Step ④ — Generate API Key
- ✨ Click **Generate API Key** / **Create Key**
- 🔑 Your key will look like: `ah_xxxxxxxxxxxxxxxxxxxx`
- 📋 **Copy** and save it securely

> ⚠️ **Never share your API key publicly.**

---

## 🚀 How to Use the API Key

### cURL Example

```bash
curl -N -X POST https://xgpt10.cloud.run/api/v1/chat/completions \
  -H "Authorization: Bearer ah_your_api_key_here" \
  -H "Content-Type: application/json" \
  -d '{
    "provider": "gemini",
    "model": "gemini-3.8-flash",
    "messages": [{"role": "user", "content": "Hello, how are you?"}],
    "stream": true
  }'
```

### Important Headers

| Header | Value |
|:---|:---|
| 🔑 Authorization | `Bearer ah_your_api_key_here` |
| 📦 Content-Type | `application/json` |

---

## 💡 Pro Tips

- 🔒 Keep your API key private
- 🔄 You can regenerate the key anytime from Developer Console
- 📡 Use `stream: true` for real-time responses
- 🔀 Change `provider` and `model` as needed

---

<div align="center">

### 🚀 [Create Your API Key Now →](https://xgpt10.cloud.run)

🌐 [Website](https://xgpt10.cloud.run) • 💻 [GitHub](https://github.com/sumitjilowa34-oss/Xgpt10)

</div>
