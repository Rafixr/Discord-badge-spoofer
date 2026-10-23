# ✦ Discord Badge Spoofer ✦

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python 3.10+">
  <img src="https://img.shields.io/badge/Console-HexLogger-8A5CF6?style=for-the-badge" alt="HexLogger">
  <img src="https://img.shields.io/badge/Platform-Windows-0078D6?style=for-the-badge&logo=windows&logoColor=white" alt="Windows">
  <img src="https://img.shields.io/badge/Author-Nur%20Mohammad%20Rafi-10B981?style=for-the-badge" alt="Author">
</p>

A high-performance Discord game activity & badge spoofer designed for Windows. Built with the **HexLogger** console library featuring live gradient animations, real-time progress bars, session analytics, and native Windows PE32+ hardware-bound executable fingerprinting.

---

## ⚡ Features

- **HexLogger Console Suite**: Premium colored console interface with gradient banners, rounded stats panels, animated spinners, and live progress bars.
- **Dynamic Theme Engine**: Switch between built-in visual themes (`premium`, `neon`, `sunset`, `ocean`, `hacker`, `minimal`) on the fly.
- **Hardware-Bound PE32+ Fingerprinting**: Generates legitimate Windows Authenticode and `MachineGuid` fingerprints required for game badge verification.
- **Automated Game Discovery**: Loads thousands of verified games directly from Discord's CDN with local cache fallback.
- **Smart Rotation**: Intelligently tracks and rotates through games to maximize badge credit without repetition.
- **Session Super Properties**: Spoofs Discord Desktop Client telemetry headers and handshake events.

---

## 📋 Prerequisites

- **Operating System**: Windows 10 / 11 (64-bit recommended for PowerShell fingerprinting)
- **Python**: Version 3.10 or higher
- **Discord Account**: User token and `cf_clearance` cookie

---

## 🚀 Installation & Setup

### 1. Clone or Download the Repository

```bash
git clone https://github.com/your-username/discord-badge-spoofer.git
cd discord-badge-spoofer
```

### 2. Install Required Dependencies

Install dependencies using `requirements.txt`:

```bash
pip install -r requirements.txt
```

*(If missing, `hexlogger` will also automatically install on the first run of `spoofer.py`)*

---

## 🎮 How to Use

### 1. Launch the Application

Run the spoofer script from your terminal:

```bash
python spoofer.py
```

### 2. First-Time Setup & Authentication

Upon initial launch, the spoofer will guide you through setup:

1. **Gate Verification**: Follow the prompt to subscribe to the YouTube channel and join the Discord community.
2. **Discord Account Token**: Paste your account authorization token when prompted (saved locally in `data.json`).
3. **Cloudflare Cookie (`cf_clearance`)**: Paste your cookie header to pass Cloudflare verification on Discord's `/science` telemetry endpoint.

> [!TIP]
> **How to get your Discord Token**:
> - Open Discord in your browser or desktop app (`Ctrl + Shift + I` for DevTools).
> - Go to the **Network** tab, trigger any request (e.g. click a channel), and copy the `Authorization` header value.

> [!TIP]
> **How to get your Cookie (`cf_clearance`)**:
> - In browser DevTools under **Application** > **Cookies** > `https://discord.com`, copy the `cf_clearance` cookie or raw request `Cookie` header.

### 3. Generate Hardware Fingerprint (Recommended)

From the main menu, select **Option 3**:
- Point it to a verified game executable (e.g. `C:\Games\Game.exe`) or the process ID (`PID`) of any running 64-bit game.
- The script executes PowerShell to generate an authenticode-hashed PE32+ fingerprint tied to your machine and user ID.

### 4. Claim Games & Badges

From the main menu, select **Option 1**:
1. Enter the number of games to spoof (or press Enter for all available).
2. Enter the duration in hours per game (e.g., `1` or `2.5`).
3. Sit back and watch the live progress bar stream telemetry events!

---

## 🎨 Themes

Change the console theme at any time via **Option 4** in the menu:
- `Premium` *(Default - Cyber Violet & Emerald)*
- `Neon` *(Cyan & Electric Pink)*
- `Sunset` *(Warm Amber & Crimson)*
- `Ocean` *(Deep Blue & Aqua)*
- `Hacker` *(Terminal Green & Matrix)*
- `Minimal` *(Clean & Subtle)*

---

## 🔗 Official Links & Community

- **YouTube Channel**: [Subscribe to NoMercy Development](https://www.youtube.com/@NoMercyDevelopment?sub_confirmation=1)
- **Discord Community**: [Join NoMercy Discord Server](https://discord.gg/d7AyVrEF68)

---

## 👤 Author

- **Nur Mohammad Rafi** (NoMercy Team)

---

## ⚠️ Disclaimer

> [!WARNING]
> This software is provided for educational and security research purposes only. Automating interactions with Discord's private APIs or spoofing telemetry events may violate Discord's [Terms of Service](https://discord.com/terms) and [Community Guidelines](https://discord.com/guidelines). Use this utility entirely at your own discretion and risk. The author and contributors assume no liability for account restrictions, suspensions, or any other consequences resulting from the use of this tool.
