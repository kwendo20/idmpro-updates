
# IDM Pro — KWENDO Edition

<div align="center">

![Version](https://img.shields.io/badge/version-6.0.0-blue?style=flat-square)
![Python](https://img.shields.io/badge/python-3.8+-blue?style=flat-square&logo=python)
![Platform](https://img.shields.io/badge/platform-Windows%20%7C%20macOS%20%7C%20Linux-lightgrey?style=flat-square)
![License](https://img.shields.io/badge/license-Commercial-orange?style=flat-square)

**A professional desktop download manager built with Python & Tkinter.**  
Multi-segment downloading · Scheduler · yt-dlp support · 5 themes · 6 languages

---

📱 **WhatsApp:** [+254 718 739 981](https://wa.me/254718739981?text=Hi%20KWENDO%2C%20I%20want%20to%20purchase%20IDM%20Pro%20license)  
📧 **Email:** jameskwendo20@gmail.com

</div>

---

## Features

- **Multi-segment downloading** — splits files into up to 64 parallel segments for maximum speed
- **yt-dlp integration** — download videos from YouTube, TikTok, Instagram, and 1000+ sites
- **Download scheduler** — schedule downloads to start at a specific date and time
- **Clipboard watcher** — auto-detects URLs copied to clipboard
- **Queue management** — priority levels (High / Normal / Low), pause, resume, retry
- **Browser extension server** — capture downloads directly from Chrome/Firefox
- **Proxy support** — HTTP, HTTPS, SOCKS proxies with optional authentication
- **Checksum verification** — SHA-256 / MD5 integrity checks after download
- **5 themes** — Dark, Light, Ocean Blue, Forest Green, Sunset Red
- **6 languages** — English, Kiswahili, French, Spanish, Portuguese, Arabic
- **Portable mode** — run from a USB drive, no installation needed
- **Auto-shutdown** — shut down PC automatically after all downloads complete
- **Download history** — searchable log of all completed downloads
- **Settings export/import** — backup and restore your configuration

---

## Screenshots

> _Add your screenshots here_

---

## Requirements

| Requirement | Version |
|---|---|
| Python | 3.8 or higher |
| tkinter | Included with Python |
| yt-dlp _(optional)_ | Latest |
| pyperclip _(optional)_ | Latest |
| pystray + Pillow _(optional)_ | Latest |

---

## Installation

**1. Clone the repository**
```bash
git clone https://github.com/kwendo20/idmpro.git
cd idmpro
```

**2. Install dependencies**
```bash
pip install yt-dlp pyperclip pystray Pillow
```

**3. Run**
```bash
python IDMPro_v6_FINAL.py
```

### Windows — build an executable
```bash
pip install pyinstaller
pyinstaller --onefile --windowed --name "IDMPro" IDMPro_v6_FINAL.py
```

### Portable mode
Place a file named `portable.flag` next to the `.exe` — all data will be stored in the same folder instead of the home directory.

---

## License

IDM Pro uses a **commercial license** with a 7-day / 30-download free trial.

| Plan | Price | Activations |
|---|---|---|
| Trial | Free | 1 device, 30 downloads |
| Pro | Contact KWENDO | Up to 3 devices |

**To purchase a license:**
- WhatsApp: [+254 718 739 981](https://wa.me/254718739981?text=Hi%20KWENDO%2C%20I%20want%20to%20purchase%20IDM%20Pro%20license)
- Email: jameskwendo20@gmail.com

### Activating your license
1. Open IDM Pro → **License & About** → **Activate / Manage License**
2. Enter your license key in the format `KWENDO-XXXX-XXXX-XXXX`
3. Enter your email and click **Activate**

Keys are verified remotely. A valid internet connection is required on first activation.

---

## Update Policy

IDM Pro checks for updates automatically on startup.  
When a new version is available:

- You have a **7-day grace period** to update at your convenience
- The skip button shows a countdown: _"Skip (6d left)"_
- After 7 days the update becomes **mandatory**
- The admin can extend or shorten this window remotely via the Admin Panel

---

## Admin Panel

For developers/resellers. Run on your machine only — **never distribute this file.**

```bash
python python_key_generator.py          # Open full admin panel
python python_key_generator.py generate user@email.com   # Quick key
python python_key_generator.py list     # List all keys
```

### Admin capabilities

| Option | Description |
|---|---|
| Generate key | Create a license key from an email |
| Bulk generate | Generate many keys at once |
| Revoke key (local) | Remove from local database |
| Revoke key (remote) | Push to GitHub — disables all instances within 1 hour |
| Add key (remote) | Push new key to GitHub |
| Sync with GitHub | Merge local + remote keys |
| Update grace period | Extend or reduce how long users can skip updates |
| Set GitHub token | Required for remote operations |

### Setting up remote key management

1. Create a GitHub repo: `yourusername/idmpro-updates`
2. Go to [github.com/settings/tokens](https://github.com/settings/tokens) → generate a token with `repo` scope
3. In the admin panel → **Option 18** → paste your token
4. Use **Option 15** to push your first `valid_keys.json`

---

## File Structure

```
IDMPro_v6_FINAL.py          # Main application
python_key_generator.py     # Admin panel (keep private)
portable.flag               # Place next to .exe for portable mode
```

**Data files created at runtime** (stored in home directory):

```
~/.idmpro_settings_kwendo.json
~/.idmpro_license_kwendo.json
~/.idmpro_queue_kwendo.json
~/.idmpro_history_kwendo.json
~/.idmpro_schedule_kwendo.json
~/.idmpro_valid_keys_kwendo.json
~/.idmpro_kwendo.log
```

---

## Troubleshooting

**Videos not downloading?**
```bash
pip install -U yt-dlp
```

**Clipboard watch not working?**
```bash
pip install pyperclip
# Linux also needs: sudo apt install xclip
```

**System tray not showing?**
```bash
pip install pystray Pillow
```

**License says revoked?**
Contact KWENDO — your key may need to be re-issued.

---

## Developer

Built by **KWENDO** — Kenya 🇰🇪

📱 WhatsApp: [+254 718 739 981](https://wa.me/254718739981)  
📧 Email: jameskwendo20@gmail.com

---

<div align="center">
<sub>© 2025 KWENDO. All rights reserved.</sub>
</div>
