# 🎬 CHEAT CLIP

> **AI-Powered YouTube Viral Hotspot Finder** — Discover the most re-watched moments in any YouTube video and extract viral Shorts, Reels, and TikToks in seconds.

[![React](https://img.shields.io/badge/React-19-blue.svg)](https://react.dev/)
[![FastAPI](https://img.shields.io/badge/FastAPI-0.100+-green.svg)](https://fastapi.tiangolo.com/)
[![Google Gemini](https://img.shields.io/badge/Google_Gemini-Flash_AI-orange.svg)](https://aistudio.google.com/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

---

## ✨ Features

- 📊 **Audience Retention Heatmaps** — Visualizes where viewers rewound and re-watched the most.
- 🧠 **Smart Gemini AI Extraction** — Scans dialogue and heatmap peaks to identify viral hooks, punchlines, and high-energy moments.
- ⏱️ **1-Click Timestamp Export** — Copy raw time ranges (`01:23 - 01:53`), titled notes, or YouTube Chapters.
- 🕒 **Integrated Player** — In-app video playback with auto-looping clips and interactive seeking.
- 🔍 **History & Search** — Search past analyses by title, link, quote, or clip topic with instant local caching.
- 📝 **Flexible Subtitles** — Auto-fetch via Supadata/YouTube with live quota monitoring, or upload manual `.srt`/`.txt` files.
- 🌐 **Bilingual Support** — Seamless toggle between English and Indonesian (Bahasa Indonesia).

---

## 🚀 Quick Start

### Prerequisites
- [Node.js](https://nodejs.org/) (v18+)
- [Python](https://www.python.org/) (v3.10+)
- [Git](https://git-scm.com/)

### 1. Clone & Install
```bash
git clone https://github.com/galihjuansaputra/cheat-clip.git
cd cheat-clip

# Install frontend dependencies
npm install

# Install backend dependencies
python -m pip install -r backend/requirements.txt
```

### 2. Run Locally
```bash
npm run dev
```
Open **[http://localhost:5173](http://localhost:5173)** in your browser. Both frontend (port 5173) and backend (port 8000) will start automatically.

---

## 🔑 Getting an API Key

Cheat Clip requires a Google Gemini API key (free, no credit card required):
1. Visit **[Google AI Studio](https://aistudio.google.com/)** and sign in.
2. Click **"Get API key"** → **"Create API key"**.
3. Paste the key into Cheat Clip (stored securely in your browser's local storage).

> 💡 **Quick Test**: Type `mock` into the API key field to explore the interface with sample data without an API key.

---

## 🎯 How to Use

1. **Paste YouTube URL** — Enter any public YouTube link.
2. **Select Settings** — Choose duration (`15s`, `30s`, `60s`), optional topic prompts, or custom time ranges.
3. **Analyze** — Click **"Analyze Video"** to stream real-time results and heatmap visualization.
4. **Export** — Use **"Copy Timestamps"** to paste straight into your video editor (Premiere, DaVinci, CapCut) or YouTube description.

---

## 📜 Available Commands

| Command | Description |
|---|---|
| `npm run dev` | Runs frontend (Vite) and backend (FastAPI) concurrently |
| `npm run dev-frontend` | Runs only the Vite frontend dev server |
| `npm run dev-backend` | Runs only the FastAPI backend server with auto-reload |
| `npm run build` | Compiles TypeScript and builds production bundle (`dist/`) |
| `npm run lint` | Runs ESLint checks |

---

## 📁 Project Structure

```text
cheat-clip/
├── backend/
│   ├── main.py              # FastAPI server, scraper & Gemini model chain
│   ├── requirements.txt     # Python backend dependencies
│   └── .env.template        # Environment template (rotating Supadata keys & proxy)
├── src/
│   ├── App.tsx              # Main dashboard, clip renderer & player
│   ├── components/          # UI components (HeatmapTimeline, LanguageSwitcher)
│   ├── locales/             # Localization dictionary (en.ts, id.ts)
│   └── index.css            # Dark mode glassmorphic design system
└── package.json             # Scripts & dependencies
```

---

## 📄 License

Distributed under the [MIT License](LICENSE).
