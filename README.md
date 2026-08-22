<h1 align="center">
  <br>
  Steam Account Manager (SAM)
</h1>

<h4 align="center">Securely manage, switch, and monitor multiple Steam accounts in one place.</h4>

<p align="center">
  <a href="#features">Features</a> •
  <a href="#installation">Installation</a> •
  <a href="#how-it-works">How It Works</a> •
  <a href="#security">Security</a> •
  <a href="#license">License</a>
</p>

---

## Features

- **🚀 One-Click Account Switching:** Switch between multiple Steam accounts instantly without manually typing passwords.
- **🛡️ Secure Local Storage:** Your credentials are encrypted locally using machine-specific hardware keys. No data is ever sent to external servers.
- **📊 Real-Time Account Stats:** Track your Steam Level, VAC/Game Bans, playtime, and currently played games right from the dashboard.
- **📱 SteamGuard Integration:** Built-in TOTP support means you don't need to check your phone every time you switch accounts.
- **📂 Categories & Organization:** Group your accounts (e.g., Mains, Smurfs, Trade Bots) to keep things clean and organized.
- **⚙️ Auto-Updater:** Silent, seamless background updates directly from GitHub Releases. You're always on the newest version.
- **🌑 Modern UI:** Clean, responsive, and dark-mode native interface.

## Installation

1. Go to the [Releases page](https://github.com/czmenz/SAM/releases).
2. Download the latest `SAM.Installer.X.X.X.exe`.
3. Run the installer.
4. Launch the application from your desktop or start menu.

## How It Works

Steam Account Manager interacts with the Steam client locally on your machine. When you add an account, it securely stores the login tokens. When you click to switch accounts, SAM automatically closes Steam, injects the proper login parameters, and cleanly relaunches it directly into the selected account.

### Steam API
To fetch extended details (Steam Level, Avatar, Ban Status, Playtime), you can provide your own **Steam API Key** in the `Settings -> Steam API` tab. Without it, basic switching still works perfectly!

## Security

We take your account security seriously. 
- **No Cloud Syncing:** All data stays on your machine. 
- **Encryption:** Credentials are encrypted using AES-256 before being saved to disk. The decryption key is derived directly from your hardware's unique Machine ID (`machineIdSync`), meaning if someone copies your config file to another PC, they won't be able to decrypt your accounts.

---
*Created by [Czmenz](https://github.com/czmenz)*
