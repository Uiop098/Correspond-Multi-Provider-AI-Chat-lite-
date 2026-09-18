# 🖋️ Correspond — Multi-Provider AI Chat (Lite)

A sleek, privacy-focused, zero-backend, multi-provider AI chat application built with pure vanilla web standards (HTML5, CSS3, JavaScript).

![Web](https://img.shields.io/badge/Platform-Web%20Browser-teal)
![License](https://img.shields.io/badge/License-MIT-blue)
![Dependencies](https://img.shields.io/badge/Dependencies-Zero%20(Pure%20Vanilla)-brightgreen)

---

## ✨ Features

- **🌐 Multi-Provider AI Support:** Connect directly to Groq, Google Gemini, OpenAI, Anthropic, OpenRouter, Mistral, DeepSeek, and local Ollama endpoints.
- **🔒 Privacy-First Architecture:** API keys are stored strictly in JavaScript browser memory during the session—never uploaded, proxied, or saved to external databases.
- **⚡ Lightweight & Fast:** Single-file static web application requiring no Node.js server, Python backend, or build process.
- **🎨 Glassmorphic Interface:** Clean dark-mode editorial aesthetic with Fraunces & Inter typography, animated typing indicators, and message bubble animations.
- **💬 Chat Controls:** Session chat history, Markdown code blocks, auto-scrolling, clear conversation, and keyboard shortcuts (`Enter` to send, `Shift+Enter` for multi-line).

---

## 🚀 Quick Start

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/Uiop098/Correspond-Multi-Provider-AI-Chat-lite-.git
   cd Correspond-Multi-Provider-AI-Chat-lite-
   ```

2. **Open in Browser:**
   Double click `index.html` or serve via any static web server:
   ```bash
   python3 -m http.server 8000
   # or
   npx serve .
   ```

3. **Start Chatting:**
   - Select your preferred AI Provider.
   - Enter your API Key.
   - Choose or enter the model name (e.g., `llama-3.3-70b-versatile`, `gemini-1.5-flash`, `gpt-4o`).
   - Type your prompt and press **Enter**!

---

## 🤖 Supported Providers

| Provider | Supported Models | API Standard |
|---|---|---|
| **Groq** | LLaMA 3.3, LLaMA 3.1, Mixtral, Gemma | OpenAI-compatible |
| **Google Gemini** | Gemini 1.5 Pro, Gemini 1.5 Flash, Gemini 2.0 | Google AI Studio REST |
| **OpenAI** | GPT-4o, GPT-4o-mini, o1, o3-mini | OpenAI REST |
| **Anthropic** | Claude 3.5 Sonnet, Claude 3.5 Haiku | Anthropic Messages API |
| **OpenRouter** | Any OpenRouter routed model | OpenAI-compatible |
| **Ollama** | Local LLaMA, DeepSeek, Qwen | Local REST (localhost:11434) |

---

## 📜 License

MIT License. Designed and maintained by **Uiop098**.
