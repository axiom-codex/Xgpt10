# How to Create API Key on Xgpt10

**Website:** [https://xgpt10.cloud.run](https://xgpt10.cloud.run)

This guide shows you exactly how to generate your unified API key.

---

## Method 1: Instant Developer Preview (No Sign-In)

1. Go to **[https://xgpt10.cloud.run](https://xgpt10.cloud.run)**
2. Click on **"Instant Developer Preview (No Sign-In Needed)"**
3. You will get temporary access to try the platform
4. Generate or view a sample API key for testing

> Best for quick testing.

---

## Method 2: Sign In & Get Permanent API Key (Recommended)

### Step 1: Open the Website
Visit → [https://xgpt10.cloud.run](https://xgpt10.cloud.run)

### Step 2: Sign In
Choose any login method:

- **Sign in with Google** (1-Click + Biometric Passkey supported)
- **GitHub**
- **Twitter (X)**
- **Email** (enter email + password or create account)

### Step 3: Open Developer Console
After login you will see the **Developer Console**.

### Step 4: Generate API Key
- Click on **Generate API Key** / **Create Key**
- Your key will look like: `ah_xxxxxxxxxxxxxxxxxxxx`
- **Copy** and save it securely

> Never share your API key publicly.

---

## How to Use the API Key

### cURL Example

```bash
curl -N -X POST https://api-hub.cloud/api/v1/chat/completions \
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

| Header              | Value                          |
|---------------------|--------------------------------|
| Authorization       | `Bearer ah_your_api_key_here`  |
| Content-Type        | `application/json`             |

---

## Tips

- Keep your API key private
- You can regenerate the key anytime from the Developer Console
- Use `stream: true` for real-time responses
- You can change `provider` and `model` as needed

---

## Need Help?

- Website: [https://xgpt10.cloud.run](https://xgpt10.cloud.run)
- GitHub Repo: [https://github.com/sumitjilowa34-oss/Xgpt10](https://github.com/sumitjilowa34-oss/Xgpt10)
