# ⚡ ZeroTerminal

<p align="center">
  <strong>The Zero-Risk Desktop Toolbox for CLI Tools, 4K Media Extraction & Offline Local AI.</strong>
</p>

<p align="center">
  <a href="https://github.com/3pple10/zeroterminal/releases/latest">
    <img src="https://img.shields.io/github/v/release/3pple10/zeroterminal?color=blue&style=flat-square" alt="Latest Release" />
  </a>
  <a href="https://github.com/3pple10/zeroterminal/stargazers">
    <img src="https://img.shields.io/github/stars/3pple10/zeroterminal?style=flat-square" alt="Stars" />
  </a>
  <a href="https://github.com/3pple10/zeroterminal/blob/main/LICENSE">
    <img src="https://img.shields.io/badge/license-MIT-green?style=flat-square" alt="License: MIT" />
  </a>
  <img src="https://img.shields.io/badge/platform-macOS%20%7C%20Windows%20%7C%20Linux-lightgrey?style=flat-square" alt="Platforms" />
</p>

---

## 💡 What is ZeroTerminal?

Most powerful developer tools live exclusively in the terminal (`yt-dlp`, `ffmpeg`, local LLM runtimes, bash scripts). For everyday users, terminal syntax is intimidating, and one accidental typo like `rm file .txt` can destroy hours of work.

**ZeroTerminal** bridges this gap. It wraps the internet's most capable command-line engines into an intuitive, beautiful desktop application with real-time visual safety guards—giving you full CLI power with **zero setup** and **zero terminal risk**.

---

## ✨ Core Features

### 1. 🎬 High-Speed Media Fetcher (yt-dlp & FFmpeg GUI)
* **Zero Command Line Needed:** Paste any video or audio link, select your desired resolution (4K, 1440p, 1080p, 720p, or Audio MP3/FLAC), and click Download.
* **Auto-Cleaning Engine:** Automatically strips tracking tags, timestamps, and referral clutter from pasted links.
* **Batch Mode:** Queue dozens of URLs at once with multi-line inputs.
* **Browser Cookie Pass-Through:** Seamlessly bypass platform login walls (YouTube, X, Instagram) by using your active browser session (Chrome, Firefox, Brave, Edge, Safari).
* **Live Streaming Console:** Watch real-time download speeds, ETA, and native execution logs in a sleek terminal feed.

### 2. 🛡️ Safe Shell (Visual Terminal Simulator & Command Guardian)
* **Safeguard Radar:** Real-time confidence score analyzing commands character-by-character before you execute them:
  * 🟢 **100% Score:** Completely safe, non-destructive read operations (`ls`, `pwd`, `cd`).
  * 🟡 **85% – 99%:** High confidence but mathematically flagged as destructive (`rm`, `mv`). Requires explicit confirmation.
  * 🟠 **70% – 84%:** Unverified target paths.
  * 🔴 **< 70%:** Syntax critical lockout. Catches fatal beginner typos (e.g., accidental space before an extension: `rm file .txt` or destructive roots like `rm -rf /`).
* **Live-Impact Blueprint:** An animated visual schematic of your filesystem that updates in real time:
  * Typing `mkdir Photos` spawns a ghosted folder showing exactly where it will be built.
  * Typing `mv doc.txt Desktop/` draws a path vector connecting the source to the destination.
  * If the destination is missing, the vector turns bright red and alerts you: *"This path doesn't exist. This command will accidentally rename your file."*

### 3. 🤖 Offline AI & Local Web App Builder
* **Private & Local:** Connect to on-device models via Ollama, LM Studio, or in-browser WebGPU engines (Qwen 2.5 series).
* **Autonomous Micro-App Agent:** Describe a local tool (e.g., task scheduler, budget tracker, mini game), and the agent plans, writes, and tests the code with zero cloud dependency.
* **Embedded Local Database:** Created apps save their state inside their own folder without external servers.

---

## 🚀 Quick Download & Install

Download the latest pre-packaged standalone bundle directly from the **[Releases Page](https://github.com/3pple10/zeroterminal/releases/latest)**:

| Platform | Architecture | Package |
| :--- | :--- | :--- |
| **macOS** | Apple Silicon (M1 / M2 / M3 / M4) | `ZeroTerminal-mac-arm64.zip` |
| **macOS** | Intel (x86_64) | `ZeroTerminal-mac-x64.zip` |
| **Windows** | 64-bit (Windows 10/11) | `ZeroTerminal-win-x64.zip` |
| **Linux** | 64-bit (Ubuntu / Debian / Fedora) | `ZeroTerminal-linux-x64.zip` |

> **macOS First Launch Note:**  
> Because ZeroTerminal is not signed with an expensive Apple Developer certificate, right-click `ZeroTerminal.app` and select **Open**, or run:
> ```bash
> xattr -cr /Applications/ZeroTerminal.app
> ```

> **Windows First Launch Note:**  
> If Windows Defender SmartScreen appears, click **"More info"** → **"Run anyway"**.

---

## ⚡ Terminal Quick-Run (macOS & Linux)

Prefer to test or unpack right from your terminal? Run:

```bash
# Clone the repository
git clone https://github.com/3pple10/zeroterminal.git
cd zeroterminal

# Run the app locally
bun install
bun run desktop
