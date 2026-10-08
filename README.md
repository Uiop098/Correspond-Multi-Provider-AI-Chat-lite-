# 🖋️ Correspond — Multi-Provider AI Chat & Arena (Lite)

A sleek, privacy-focused, zero-backend, multi-provider AI chat and comparison arena application built with pure vanilla web standards (HTML5, CSS3, JavaScript).

![Web](https://img.shields.io/badge/Platform-Web%20Browser-teal)
![License](https://img.shields.io/badge/License-MIT-blue)
![Dependencies](https://img.shields.io/badge/Dependencies-Zero%20(Pure%20Vanilla)-brightgreen)
![Free AI](https://img.shields.io/badge/Free%20Direct%20AI-Zero%20API%20Key-emerald)

---

## ✨ Features

- **⚡ Instant Free Chat (Zero API Keys Needed):** Chat immediately with free public models including **Pollinations Reasoning Fast OSS**, **GPT-OSS 20B**, and client-side models like **Gemini 2.0 Flash (Free)**, **DeepSeek R1 (Free)**, and **GPT-4o Mini (Free)** without entering any credit card or API key.
- **🔀 Multi-Model Checkbox Arena (Parallel Comparison):** Select multiple AI models simultaneously using interactive checkboxes. Send a single prompt and watch the models respond side-by-side in real time with response latency badges (`✓ 1.2s`) and independent copy buttons.
- **✨ Latest Google Gemini Integration:** Full, updated support for Google's newest models including:
  - `gemini-2.5-pro` (Newest reasoning & complex coding flagship)
  - `gemini-2.5-flash` (Newest ultra-fast multimodal frontier model)
  - `gemini-2.0-flash` & `gemini-2.0-flash-lite`
  - `gemini-1.5-pro` & `gemini-1.5-flash`
- **🌐 Comprehensive Provider Support (BYOK):** Connect directly to official providers:
  - **Google Gemini** (Gemini 2.5 Pro, 2.5 Flash, 2.0 Flash)
  - **DeepSeek** (DeepSeek R1, DeepSeek V3)
  - **OpenAI** (GPT-4o, GPT-4o Mini, o3-mini, o1)
  - **Anthropic** (Claude 3.7 Sonnet, Claude 3.5 Sonnet)
  - **Groq** (LLaMA 3.3 70B @ 300+ t/s, DeepSeek R1 Distill)
  - **OpenRouter** (Free and routed models)
- **🔒 Privacy-First Architecture:** Pure client-side static web app. No intermediate servers or logging. Optional browser storage keeps keys strictly on your device.
- **🎨 Glassmorphic Modern UI:** Dark-mode aesthetic with Fraunces & Inter typography, responsive multi-column comparison grid, smooth typing indicators, stop generation controls, and full Markdown code blocks with syntax styling and one-click copy.
- **⚙️ Power Tools:** Custom system instructions / persona presets, chat export to Markdown (`.md`), quick prompt chips, and instant conversation reset.

---

## 🚀 Quick Start

### 1. Run Directly in Browser
Double-click `index.html` or open it with any static web server:

```bash
# Using Python
python3 -m http.server 8000

# Or using Node.js
npx serve .
```

Visit `http://localhost:8000` in your browser.

### 2. Free Instant Mode
No setup required! Open the app, type your message, and hit **Enter** to chat with free public reasoning models right away.

### 3. Checkbox Multi-Model Arena
1. Click **"🔀 Compare Arena"** in the top navigation bar.
2. Click **"☑ Select Models"** to open the checkbox drawer.
3. Check 2, 3, or more models (or use the **"⚡ Compare Top 3"** preset).
4. Send your prompt to view side-by-side responses and compare speeds and answers in real time!

### 4. Custom API Keys (BYOK)
Click **"🔑 Use API Keys"** in the header to enter your API keys for Google Gemini, Groq, OpenAI, DeepSeek, Anthropic, or OpenRouter.

---

## 🤖 Supported Models & Providers

| Provider / Engine | Access Mode | Featured Models |
|---|---|---|
| **Free Public Engine** | ⚡ **No API Key** | `Reasoning Fast OSS`, `GPT-OSS 20B`, `Gemini 2.0 Flash (Free)`, `DeepSeek R1 (Free)`, `GPT-4o Mini (Free)` |
| **Google Gemini** | Official API | `gemini-2.5-pro`, `gemini-2.5-flash`, `gemini-2.0-flash`, `gemini-1.5-pro` |
| **DeepSeek** | Official API | `deepseek-reasoner` (R1), `deepseek-chat` (V3) |
| **OpenAI** | Official API | `gpt-4o`, `gpt-4o-mini`, `o3-mini`, `o1` |
| **Anthropic** | Official API | `claude-3-7-sonnet-20250219`, `claude-3-5-sonnet-20241022` |
| **Groq Cloud** | High-Speed LPU | `llama-3.3-70b-versatile`, `deepseek-r1-distill-llama-70b` |
| **OpenRouter** | Multi-Route / Free | `google/gemini-2.0-flash-exp:free`, `deepseek/deepseek-r1:free` |

---

## 📜 License

MIT License. Designed and maintained by **Uiop098**.
