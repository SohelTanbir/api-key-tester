# API Key Tester

**Live:** [https://api-key-tester-seven.vercel.app](https://api-key-tester-seven.vercel.app)

A simple, single-file web app to validate AI platform API keys instantly. No build step, no dependencies, no backend — just open `index.html` in your browser.

## Supported Providers

| Provider | Test Method |
|---|---|
| OpenAI / ChatGPT | GET `/v1/models` |
| Google Gemini | GET `/v1beta/models` |
| Groq | GET `/openai/v1/models` |
| Anthropic (Claude) | POST `/v1/messages` (1 token) |
| Mistral AI | GET `/v1/models` |
| Cohere | GET `/v2/models` |
| Together AI | GET `/v1/models` |
| DeepSeek | GET `/v1/models` |
| OpenRouter | GET `/api/v1/auth/key` |
| Custom Provider | User-defined endpoint |

## Features

- Paste your key, pick a provider, click **Test Key**
- Shows clear valid / invalid / rate-limited / quota-exhausted states
- Eye icon to show/hide the key inside the input
- Custom provider support — set your own endpoint, auth header, method, and body
- Reset button to clear the form instantly
- Your key is sent **only to the provider** — never stored or logged

## Usage

**Option 1 — Live site (no install):**
Visit [https://api-key-tester-seven.vercel.app](https://api-key-tester-seven.vercel.app), select your provider, paste the API key, click **Test Key**.

**Option 2 — Local:**
1. Download or clone this repo
2. Open `index.html` in any browser
3. Select your provider, paste the API key, click **Test Key**

No server required. Works from `file://` directly.

## Privacy

This tool runs entirely in your browser. The API key is transmitted directly to the chosen provider's API endpoint and nowhere else. No analytics, no logging, no third-party requests except the provider you select and Google Fonts / Font Awesome CDN for styling.

## License

MIT
