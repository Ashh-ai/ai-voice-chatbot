# 🤖 AI Voice Chatbot

A fully featured AI voice chatbot that runs entirely in your browser — no server, no backend, no installation needed. Just open `index.html` and start chatting.

![AI Voice Chatbot](https://img.shields.io/badge/AI-Voice%20Chatbot-7c6aff?style=for-the-badge)
![HTML](https://img.shields.io/badge/HTML-Single%20File-orange?style=for-the-badge)
![No Backend](https://img.shields.io/badge/No%20Backend-Required-green?style=for-the-badge)

---

## ✨ Features

- 🔑 **Multi-provider support** — Anthropic Claude, OpenAI GPT, Google Gemini
- 🎤 **Speech-to-text** — Speak your messages using your microphone
- 🔊 **Text-to-speech** — AI replies are read aloud automatically
- 💬 **Full chat UI** — Message history, timestamps, copy buttons
- ⚙️ **System prompt** — Customize the AI's behavior
- 🌙 **Dark mode** — Sleek dark themed interface
- 📱 **Responsive** — Works on mobile and desktop
- 🔒 **Private** — Your API key stays in your browser only

---

## 🚀 Quick Start

### Option 1 — Open locally
1. Download or clone this repo
2. Open `index.html` in **Chrome** or **Edge**
3. Enter your API key and start chatting

### Option 2 — GitHub Pages (recommended)
1. Fork this repo
2. Go to **Settings → Pages**
3. Set source to `main` branch, `/ (root)`
4. Visit `https://yourusername.github.io/ai-voice-chatbot`

---

## 🔑 API Keys

You need an API key from at least one provider:

| Provider | Get Key | Free Tier |
|----------|---------|-----------|
| **Anthropic** | [console.anthropic.com](https://console.anthropic.com) | $5 free credit |
| **OpenAI** | [platform.openai.com](https://platform.openai.com) | $5 free credit |
| **Google Gemini** | [aistudio.google.com](https://aistudio.google.com) | Free tier available |

> ⚠️ Your API key is **never stored** anywhere — it only lives in your browser session and goes directly to the official API endpoint.

---

## 🎙️ Voice Features

| Feature | How to use |
|---------|-----------|
| **Speak to AI** | Click the 🎤 mic button and talk |
| **AI speaks back** | Toggle "Voice replies" on (enabled by default) |
| **Stop speaking** | Click the mic button again |

> **Best browser for voice:** Chrome or Edge (full Web Speech API support). Firefox has limited support.

---

## 🛠️ Supported Models

### Anthropic
- `claude-sonnet-4-6` *(recommended)*
- `claude-opus-4-6`
- `claude-haiku-4-5`

### OpenAI
- `gpt-4o` *(recommended)*
- `gpt-4o-mini`
- `gpt-4-turbo`

### Google Gemini
- `gemini-2.0-flash` *(recommended)*
- `gemini-1.5-pro`
- `gemini-1.5-flash`

---

## 📁 File Structure

```
ai-voice-chatbot/
├── index.html      ← The entire app (single file)
└── README.md       ← This file
```

Everything is in one HTML file — no dependencies, no npm, no build step.

---

## 🔧 Customization

Open `index.html` in any code editor. The code is organized into clear sections:

```
<!-- SETUP SCREEN -->     → API key entry UI
<!-- CHAT SCREEN -->      → Main chat interface

<style>                   → All CSS / theming (CSS variables at the top)
<script>
  // STATE              → App variables
  // SETUP SCREEN       → Provider switching, connection logic
  // CHAT CONTROLS      → Clear, system prompt, voice toggle
  // SEND MESSAGE       → Message sending flow
  // callAPI()          → API calls for all 3 providers
  // MESSAGE DOM        → Rendering chat bubbles
  // TEXT-TO-SPEECH     → speak() / stopSpeaking()
  // SPEECH-TO-TEXT     → startListening() / stopListening()
```

### Change the theme colors
Edit the CSS variables at the top of `<style>`:
```css
:root {
  --accent: #7c6aff;     /* purple — change to any color */
  --bg: #0d0d0f;         /* background */
  --text: #f0f0f2;       /* main text */
}
```

---

## 🚀 Planned Upgrades

- [ ] Streaming responses (words appear as generated)
- [ ] Persistent chat history (localStorage)
- [ ] Multiple conversation threads
- [ ] Light/dark mode toggle
- [ ] Voice selection dropdown
- [ ] Export chat as text/PDF
- [ ] Image upload (vision models)
- [ ] PWA / installable app

---

## 📄 License

MIT License — free to use, modify, and distribute.

---

## 🙋 Contributing

Pull requests welcome! Open an issue first to discuss major changes.

---

Made with ❤️ — Single HTML file, zero dependencies.
