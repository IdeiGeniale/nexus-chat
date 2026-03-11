# ✦ NexusChat

A sleek, ChatGPT-like AI chat interface powered by GPT-4 Turbo via RapidAPI. Built as a single self-contained HTML file — no frameworks, no build tools, no dependencies.

---

## Features

- **GPT-4 Turbo** responses via the `chatgpt-42` RapidAPI endpoint
- **Conversation history** — full message context is sent with every request for coherent multi-turn chats
- **Sidebar** with saved chat history (persisted via localStorage) and a New Conversation button
- **Copy button** — inline "Copy" button next to any code the AI outputs
- **Typing indicator** — animated dots while waiting for a response
- **Auto-resizing input** — textarea grows as you type; Shift+Enter for newlines
- **Welcome screen** with quick-start suggestion prompts
- **Mobile support** — collapsible sidebar with overlay, fully touch-friendly layout
- **Dark theme** — deep-space aesthetic with purple accents

---

## Getting Started

No installation required. Just open the URL in any modern browser.

```
open chat.html
```

That's it.

---

## Configuration

The API key and endpoint are set at the top of the `<script>` block inside `chat.html`:

```js
const API_URL = 'https://chatgpt-42.p.rapidapi.com/conversationgpt4-2';
const API_KEY = 'YOUR_RAPIDAPI_KEY_HERE';
```

Replace `YOUR_RAPIDAPI_KEY_HERE` with your own key from [RapidAPI](https://rapidapi.com/).

---

## Usage

1. Type a message in the input box and press **Enter** (or tap the send button)
2. NexusChat sends your full conversation history to GPT-4 Turbo and streams back a response
3. If the AI responds with code, a **Copy** button appears inline — click it to copy the code to your clipboard
4. Previous conversations are saved in the sidebar and can be resumed at any time
5. Click **New Conversation** to start fresh

---

## Tech Stack

| Layer | Technology |
|---|---|
| UI | HTML, CSS, JavaScript (vanilla) |
| AI Model | GPT-4 Turbo |
| API | [chatgpt-42 on RapidAPI](https://rapidapi.com/haimomo24/api/chatgpt-42) |
| Fonts | [Sora](https://fonts.google.com/specimen/Sora) + [JetBrains Mono](https://fonts.google.com/specimen/JetBrains+Mono) via Google Fonts |
| Storage | localStorage (chat history) |

---

## File Structure

```
nexuschat/
└── chat.html      # The entire app — HTML, CSS, and JS in one file
└── README.md      # This file
```

---

## License

GPL 3.0 — do whatever you want with it.
