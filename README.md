# Carlos I.R.

Web & Android Application Development. Tier 1 IT Support & Systems Administration. Zaragoza, Spain.

Linux systems administration, diagnostics, and automation.

## Infrastructure & Home Lab

24/7 home server.

- Server: Raspberry Pi 3 Model B (Debian), 1 GB RAM.
- Persistent services managed via systemd (bots and File Browser).
- zRAM configured to avoid MicroSD swap wear and maximize available RAM.
- Remote access: SSH, TigerVNC, and Tailscale. LAN file storage via File Browser.
- Bash scripts: healthchecks, disk threshold monitoring (MicroSD and USB), and log rotation.

Project: [debian-homelab](https://github.com/Katiuxa/debian-homelab)

## Automation & APIs

1 GB of RAM leaves no room for local LLMs. Heavy text processing is offloaded to the cloud, while the Pi handles orchestration, systemd, and disk I/O.

[Telegram-Bots-Suite](https://github.com/Katiuxa/Telegram-Bots-Suite) — concurrent Python bots:

- Groq API integration with automatic model fallback when rate limits/quotas are hit.
- Audio/video transcription and document format conversion (Calibre).
- Disposable email service.
- News scraping and extraction.
- [Biblioteca Secreta](https://github.com/Katiuxa/Telegram-Bots-Suite/tree/main/BotBiblioteca): EPUB catalog stored on USB. SQLite search by title or author with direct file delivery via Telegram. The database and books are not hosted on GitHub—source code only.

[Meta-LLM](https://github.com/Katiuxa/Meta-LLM) is a standalone chat interface featuring a Telegram bot and a web panel on port 5000. OpenRouter acts as the API gateway, allowing on-the-fly model switching straight from the menu. Dolphin Venice, Cydonia, Euryale, Hermes, and similar models handle unfiltered chat, creative writing, and roleplay, while Qwen3 Coder and Command R+ remain moderated for coding and long-form text. Image generation routes through Gemini Flash Image, also via OpenRouter. Both the API key and bot token live in the Pi's `.env` file.

## Web & Logic

Classic and historical board games: rule engines, UI, web, and Android.

| Project | Repository | Play in browser |
|---|---|---|
| Ludus Latrunculorum | [Latrunculi](https://github.com/Katiuxa/Latrunculi) | [demo](https://latrunculigame.vercel.app) |
| Petteia | [Petteia](https://github.com/Katiuxa/Petteia) | [demo](https://petteiagame.vercel.app) |
| Three-Trick | [Three-Trick](https://github.com/Katiuxa/Three-Trick) | [demo](https://tritrick.vercel.app) |
| 8 Damas | [Ocho-Damas](https://github.com/Katiuxa/Ocho-Damas) | [demo](https://8damas.com) |
| Chess Puzzles | [Chess-Puzzles](https://github.com/Katiuxa/Chess-Puzzles) | [demo](https://puzzleschess.vercel.app) |
| Klotski | [Klotski](https://github.com/Katiuxa/Klotski) | [demo](https://huarongdaoklotski.vercel.app) |

## Stack

- Systems & Networking: Linux (Debian), Bash, systemd, SSH, Tailscale, TigerVNC, zRAM.
- Development: Python, JavaScript, HTML/CSS, SQLite, REST APIs.
- Media Processing & CLI: FFmpeg, yt-dlp, Calibre (`ebook-convert`).
- Tools: Git/GitHub, Capacitor / Android.
