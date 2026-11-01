# ⚡ ZeroTerminal

<p align="center">
  <strong>The Zero-Risk Desktop Toolbox: Ad-Free Media Extractor, Visual Command Safeguard & Private Local AI</strong>
</p>

<p align="center">
  <a href="https://github.com/3pple10/zeroterminal/releases/latest"><img src="https://img.shields.io/github/v/release/3pple10/zeroterminal?color=emerald&label=Release&style=flat-square" alt="Latest Release"></a>
  <a href="https://github.com/3pple10/zeroterminal/releases"><img src="https://img.shields.io/github/downloads/3pple10/zeroterminal/total?color=blue&style=flat-square" alt="Downloads"></a>
  <a href="LICENSE"><img src="https://img.shields.io/badge/License-MIT-purple?style=flat-square" alt="License"></a>
  <img src="https://img.shields.io/badge/Platform-macOS%20%7C%20Windows%20%7C%20Linux-orange?style=flat-square" alt="Platform">
</p>

---

## 📌 Overview

**ZeroTerminal** is an open-source, all-in-one local desktop suite packaged as **Workbench** (`v1.0.0`). It eliminates terminal frustration by giving you visual, fail-safe front-ends for powerful command-line tools without writing commands:

1. **Fetcher:** High-speed 4K video, audio, and subtitle extractor powered by bundled `yt-dlp` and `ffmpeg` (no terminal required).
2. **Safe Shell:** Interactive command simulator with real-time risk radar and live visual file-tree impact blueprints.
3. **Local AI Agent:** 100% offline app generator and code workspace powered by Ollama, LM Studio, or on-device WebGPU models.

---

## 🚀 Quick Download (v1.0.0)

Pre-built binaries include all bundled engines (`yt-dlp`, `ffmpeg`, local runner bridges). Download the package for your operating system:

| Platform | Architecture | Package File | Direct Download |
| :--- | :--- | :--- | :--- |
| **macOS** | Apple Silicon (M1/M2/M3/M4) | `Workbench-macOS-AppleSilicon.zip` | [Download](https://github.com/3pple10/zeroterminal/releases/download/v1.0.0/Workbench-macOS-AppleSilicon.zip) |
| **macOS** | Intel (x86_64) | `Workbench-macOS-Intel.zip` | [Download](https://github.com/3pple10/zeroterminal/releases/download/v1.0.0/Workbench-macOS-Intel.zip) |
| **Windows** | 64-bit | `Workbench-Windows-x64.zip` | [Download](https://github.com/3pple10/zeroterminal/releases/download/v1.0.0/Workbench-Windows-x64.zip) |
| **Linux** | x86_64 | `Workbench-linux-x64.tar.gz` | [Download](https://github.com/3pple10/zeroterminal/releases/download/v1.0.0/Workbench-linux-x64.tar.gz) |

> **Note on App Name:** The desktop binary is distributed under the application name **`Workbench`** (`Workbench.app` / `Workbench.exe`).

---

### 🖥️ First-Time Launch Instructions

Because ZeroTerminal binaries are self-hosted open-source builds without paid corporate code-signing certificates:

* **macOS:** Unzip, drag `Workbench.app` to your Applications folder. On first launch, **right-click `Workbench.app`** and select **Open** (or run `xattr -cr /Applications/Workbench.app` in Terminal).
* **Windows:** Unzip `Workbench-Windows-x64.zip` and run `Workbench.exe`. If Windows SmartScreen appears, click **More info** → **Run anyway**.
* **Linux:** Extract `Workbench-linux-x64.tar.gz` and execute the `Workbench` binary (`chmod +x Workbench && ./Workbench`).

---

## ✨ Features

### 1. 🎬 Fetcher (Media Extractor)
A high-performance GUI wrapper for media downloads that runs completely on your machine.
* **Smart URL Cleaner:** Automatically strips tracking tags, referral parameters, and timestamps. Displays clean URL preview and auto-detects platform badges (YouTube, X/Twitter, Instagram, TikTok, Facebook).
* **Batch Downloader:** Toggle Batch Mode to paste multiple links at once.
* **Format & Quality Control:** Presets from **Best Available**, **4K**, **1080p**, **720p** down to **Audio Only** (`.mp3`, `.flac`, `.mp4`, `.mkv`, `.webm`).
* **Browser Session Support:** Pass cookies from your browser (Chrome, Firefox, Brave, Edge, Safari) to download your private or member-only playlists safely.
* **Live Terminal Output:** Real-time log console, download speed, progress bar, and instant cancel/kill button.

---

### 2. 🛡️ Safe Shell (Visual Terminal Simulator)
Prevent destructive terminal accidents with real-time simulation before commands touch your files.
* **Safeguard Radar:** Real-time confidence scoring:
  * 🟢 **100% Clean:** Safe, non-destructive navigation (`ls`, `cd`, `pwd`).
  * 🟡 **85%–99% Warning:** Syntactically correct but destructive (`rm`, `mv`) — requires a double-confirmation click.
  * 🟠 **70%–84% Caution:** Uncertain or ambiguous file paths.
  * 🔴 **Below 70% Locked:** Critical syntax warning or dangerous typo (`rm file .txt`, `rm -rf /`) — execution button automatically locks out.
* **Live-Impact Blueprint:** Renders an animated SVG schematic of your folder tree character-by-character:
  * `mkdir Photos` spawns a glowing preview folder.
  * `mv doc.txt Desktop/` draws a real vector arrow from the file to the target container.
  * Missing destinations snap the arrow red: *"This path doesn't exist. This will accidentally rename your file instead of moving it."*
* **Trash Recovery:** Destructive file operations automatically use system Trash for safety.

---

### 3. 🤖 Local AI Agent & Offline Studio
Build micro-web apps, games, and tools locally without cloud dependencies.
* **100% Private & Offline:** Zero telemetry or data collection.
* **Flexible Model Backends:**
  * **Local Runner:** Seamless connection to **Ollama** (`localhost:11434`) or **LM Studio** (`localhost:1234`).
  * **On-Device WebGPU:** Run quantized models (like Qwen 2.5 Coder) directly in unified memory.
* **Autonomous Verification Loop:** Plan → Write → Check cycle with automated syntax error correction and built-in offline SQLite/IndexedDB persistence.
* **Jcode Engine:** High-speed native code editing harness support on Apple Silicon.

---

## 🛠️ Running from Source

If you prefer building and running the app directly from source:

### Prerequisites
* Node.js 20+
* Bun / npm / pnpm

```bash
# Clone the repository
git clone https://github.com/3pple10/zeroterminal.git
cd zeroterminal

# Install dependencies
npm install

# Start the web app in development mode
npm run dev

# Launch the desktop Electron app
npm run desktop
