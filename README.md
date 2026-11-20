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

## Embedded & Hardware

Custom firmware development for microcontrollers.

- **META TV IR**: Interactive infrared TV scanner and universal remote firmware for the **M5Stack Cardputer ADV** (ESP32-S3 / Stamp-S3A, 8 MB Flash, no PSRAM).
- Features regional codebase filtering (EU, US, Asia, All), interactive Auto-Sweep with instant freeze-on-reaction, stealth probing (`MUTE` / `VOL+`), full remote layout, favorites, and continuous ON/OFF brute-force mode.
- Built with C++ / PlatformIO and distributed via M5Burner and M5Launcher.

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

Classic and historical board games. Rule engines, interface, web, and Android.

**[Ludus Latrunculorum](https://github.com/Katiuxa/Latrunculi).** Roman soldiers on an incised board. Every piece moves like a rook. An enemy falls by custody, caught between two of yours. The Dux does not fall that way: you win by closing its four sides. Normal is 8×8. Britannia is 8×12. [Play](https://latrunculi.vercel.app)

**[Petteia](https://github.com/Katiuxa/Petteia).** The Greek pincer game, under the name ΠΕΤΤΕΙΑ. Pieces move like a rook and capture by closing a pincer. Five strengths, from Paidion to Palamedes, or an online game with a room code. [Play](https://petteiagame.vercel.app)

**[Three-Trick](https://github.com/Katiuxa/Three-Trick).** The physical tile puzzle, on screen. Slide, lift, and drop until the tiles sit in order from 1 to 9. [Play](https://tritrick.vercel.app)

**[8 Damas](https://github.com/Katiuxa/Ocho-Damas).** The eight queens puzzle. Place the queens so that none share a row, a column, or a diagonal. Normal play, problem boards with queens already fixed, and a time attack of 1, 3, or 5 minutes. Boards run from 8×8 to 11×11. [Play](https://8damas.vercel.app)

**[Chess Puzzles](https://github.com/Katiuxa/Chess-Puzzles).** Android app. Four chess studies by Sherzod Khaydarbekov (2025): Rook Sacrifice, The Black Pawn, Four Square, and Queen Moves. Orthodox moves, blocked squares, one objective on each board.

**[Klotski](https://github.com/Katiuxa/Klotski).** Huarongdao. Slide the blocks and bring the single red piece out through the bottom gate. [Play](https://huarongdaoklotski.vercel.app)

## Stack

- Systems & Networking: Linux (Debian), Bash, systemd, SSH, Tailscale, TigerVNC, zRAM.
- Development: Python, C++, JavaScript, HTML/CSS, SQLite, REST APIs.
- Embedded & Hardware: ESP32-S3, M5Stack Cardputer ADV, PlatformIO, Infrared (IR) protocols.
- Media Processing & CLI: FFmpeg, yt-dlp, Calibre (`ebook-convert`).
- Tools: Git/GitHub, Capacitor / Android.
