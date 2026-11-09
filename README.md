# TextLab — Precision Text Utilities

TextLab is a modern, single-page web application focused on text utilities, crafted with a sleek dark slate interface inspired by Linear and Vercel design aesthetics. It contains zero build dependencies and is 100% ready to deploy directly to **GitHub Pages**.

![TextLab Preview](https://img.shields.io/badge/Theme-Linear%2FVercel%20Dark-6366f1?style=for-the-badge)
![Deployment](https://img.shields.io/badge/GitHub%20Pages-Ready-emerald?style=for-the-badge)
![Localization](https://img.shields.io/badge/Languages-Vietnamese%20%7C%20English-blue?style=for-the-badge)

---

## ✨ Features

### 🌐 1. Language Translator (Tab 1)
- **Public API Integration:** Powered by the free MyMemory Translation API.
- **Languages Supported:** Vietnamese (`vi`), English (`en`), Japanese (`ja`), Korean (`ko`), Chinese (`zh-CN`), French (`fr`), German (`de`), Spanish (`es`), Russian (`ru`), plus Auto-Detect.
- **Intelligent Chunking Handler:** Automatically splits long documents into sentence-aware chunks (<420 characters) to avoid the public API query length limits.
- **Interactive Controls:** One-click language swap (⇄) with animation, character counter, live status notifications, and instant copy-to-clipboard.
- **Keyboard Shortcut:** `Ctrl + Enter` (or `Cmd + Enter`) to trigger instant translation.

### 📊 2. Word & Character Counter (Tab 2)
- **Real-time Metrics:** Updates dynamically on keypress or paste.
  - **Total Words:** Accurate Unicode boundary matching supporting accented Vietnamese words.
  - **Total Characters:** Exact character count including spaces and emojis.
  - **Characters without Spaces:** Precise non-whitespace character count.
  - **Estimated Sentences:** Sentence terminator detection (`.`, `!`, `?`, `。`).
  - **Paragraphs Count:** Tracks distinct text blocks.
  - **Reading & Speaking Time Estimates:** Calculated at standard speeds (200 wpm reading, 130 wpm speaking).
- **Quick Transformations:** Convert case (`UPPERCASE`, `lowercase`, `Title Case`, `Sentence case`) and clean redundant whitespace in one click.

### 📡 3. Morse Code Converter (Tab 3)
- **Bi-directional Conversion:**
  - **Text → Morse:** Converts Latin text to International Morse code.
  - **Morse → Text:** Decodes dots (`.` or `•`) and dashes (`-` or `–`, `—`) back to readable text.
- **Vietnamese Accent Normalization:** Automatically converts accented characters (`à, á, ệ, đ...`) to standard unaccented Latin characters before encoding.
- **International Standards:** Letters separated by single spaces, words separated by slashes (` / `).
- **Audio Synthesizer (Web Audio API):** Plays audible Morse code beeps at standard timing with smooth attack/decay envelopes.
- **Live Validation & Reference:** Clear warning alerts for unrecognized symbols, accompanied by a collapsible Morse code cheat sheet table.

---

## 🎨 Design & Theme
- **Theme:** Dark slate background (`#0b0d13`), soft panels (`#161a26`), subtle borders (`#232838`), and glowing indigo/violet accents.
- **Typography:** Inter for clean user interface typography, and JetBrains Mono for Morse and code textareas.
- **Localization:** Instant toggle between **Tiếng Việt (VN)** and **English (EN)** with persistent state stored in `localStorage`.
- **Responsive Layout:** Gracefully breaks down on mobile viewports with flexible grids, touch targets, and adaptive textareas.

## 📄 License
MIT License. Open-source and free to customize.
