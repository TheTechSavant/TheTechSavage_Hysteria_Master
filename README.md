# ⚡ TheTechSavage Hysteria 2 Master

![Version](https://img.shields.io/badge/Version-1.0_Premium-cyan?style=for-the-badge) 
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge) 
![Platform](https://img.shields.io/badge/Platform-Ubuntu_20%2B-orange?style=for-the-badge)
![Security](https://img.shields.io/badge/Security-API_Enforced-red?style=for-the-badge)

**The Ultimate Hysteria 2 Standalone Autoscript.** Built for administrators who need a lightweight, dedicated proxy server powered by Hysteria 2's blazing-fast UDP bypassing. Features a dynamic CLI dashboard, Nginx-free native authentication, terminal shortcuts, and automated Telegram cloud backups.

---

## 🚀 Key Features

* 🔐 **Native YAML Authentication:** Strips away clunky external file servers. Authenticate users dynamically using Hysteria 2's internal mechanics for instant creation, modification, and deletion.
* ⚡ **UDP Port Hopping:** Evade ISP throttling and DPI by natively routing traffic across a wide range of UDP ports simultaneously.
* ⏳ **Timed & Trial Accounts:** Generate temporary passes (e.g., 30 minutes) or 24-hour trials that automatically self-destruct from the server when time expires.
* 🧹 **Nightly Sweeper:** A background cronjob that hunts down and deletes expired accounts every night at 1:00 AM to keep your database clean.
* ☁️ **Automated Telegram Backups:** Zip your entire Hysteria 2 architecture, user limits, and configurations, send them to Google Drive, and instantly deliver the download link to your Telegram Bot.
* 📡 **Over-The-Air (OTA) Updates:** Push live script patches to your server directly from the master vault without ever reinstalling the OS.

---

## 📥 Installation

Run this command on a fresh **Ubuntu 20.04 / 22.04 / 24.04 LTS** or **Debian 10 / 11 / 12** VPS.

```bash
apt update && apt install -y wget && wget -q https://raw.githubusercontent.com/TheTechSavant/TheTechSavage_Hysteria_Master/main/install/setup.sh -O setup.sh && chmod +x setup.sh && ./setup.sh
```

### 🛠️ Setup Steps

1.  **Register your IP:**
    * **Free 24h Trial:** Start our [All-in-One Bot](https://t.me/TheTechSavageFile2LinkBot) and use the `/trialip` command to whitelist your VPS instantly.
    * **Full Premium:** Contact [@TheTechSavageSupport](https://t.me/thetechsavagesupport) to purchase a 30-day or Lifetime license.
2.  **Run the Installer:** Paste the installation command above into your terminal.
3.  **Network Configuration:** The script automatically detects your public IPv4 silently. Simply follow the quick prompts to select your custom port (or Port Hopping range), Masquerade URL, and SNI. *Note: If Port 53 is selected, the script will automatically disarm systemd-resolved to prevent port conflicts.*
4.  **Completion:** The server will deploy the UI, configure `iptables` NAT routing, and start the Hysteria 2 engine. 

### 🖥️ Dashboard & Shortcuts

Access the central control panel by typing:
```bash
menu
```

Bypass the menu entirely with native terminal shortcuts:
* `usernew` - Create a new user and generate their URI.
* `renew` - Extend an existing user's expiry.
* `hapus` - Delete an active user.
* `member` - List all registered users and their status.
* `cek` - Monitor live incoming Hysteria 2 connections via `journalctl`.

---

## ⚠️ Credits & Disclaimer

**Core Networking Engine, Dashboard, & Security Architecture:** Developed by [TheTechSavage](https://t.me/thetechsavage)

> *This project is for educational purposes and network management only. The developer is not responsible for misuse.*
