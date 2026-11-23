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

- **[META TV](https://github.com/Katiuxa/Meta-TV-IR)**: Infrared scanner and local Wi-Fi TV control for the **M5Stack Cardputer ADV** (ESP32-S3 / Stamp-S3A, 8 MB Flash, no PSRAM). Current release 1.1.10.
- Infrared: regional brand filtering, Auto-Sweep with freeze-on-reaction, stealth probe (`MUTE` / `VOL+`), full remote, favorites, and continuous ON/OFF brute force.
- Wi-Fi: the password is typed on the device and remembered. The search only listens for TVs that announce themselves. YouTube opens from an 11-character id or from a normal link. Samsung, LG, Sony, Roku, Panasonic, and Philips also take a network remote. Other sets stay on infrared.
- Built with C++ / PlatformIO. M5Burner writes the full flash image. M5Launcher uses the application image.

Project: [Meta-TV-IR](https://github.com/Katiuxa/Meta-TV-IR)

## Automation & APIs

1 GB of RAM leaves no room for local LLMs. Heavy text processing is offloaded to the cloud, while the Pi handles orchestration, systemd, and disk I/O.

[Telegram-Bots-Suite](https://github.com/Katiuxa/Telegram-Bots-Suite) — concurrent Python bots:

- Groq API integration with automatic model fallback when rate limits/quotas are hit.
- Audio/video transcription and document format conversion (Calibre).
- Disposable email service.
- News scraping and extraction: [OnlyNews](https://github.com/Katiuxa/Telegram-Bots-Suite/tree/main/OnlyNews) — Extracts clean article text and media directly from HTML, bypassing paywalls, JavaScript blocks, and reader restrictions.
- [Biblioteca Secreta](https://github.com/Katiuxa/Telegram-Bots-Suite/tree/main/BotBiblioteca): EPUB catalog stored on USB. SQLite search by title or author with direct file delivery via Telegram. The database and books are not hosted on GitHub—source code only.

[Meta-LLM](https://github.com/Katiuxa/Meta-LLM) is a standalone chat interface featuring a Telegram bot and a web panel on port 5000. OpenRouter acts as the API gateway, allowing on-the-fly model switching straight from the menu. Dolphin Venice, Cydonia, Euryale, Hermes, and similar models handle unfiltered chat, creative writing, and roleplay, while Qwen3 Coder and Command R+ remain moderated for coding and long-form text. Image generation routes through Gemini Flash Image, also via OpenRouter. Both the API key and bot token live in the Pi's `.env` file.

## Web & Logic

Classic and historical board games: rule engines, UI, web, and Android.

| Project | Description & Mechanics | Links |
| :--- | :--- | :--- |
| **Ludus Latrunculorum** | Roman strategy board game. Pieces move orthogonally like rooks and capture enemies by custodian pincers, while the *Dux* can only be defeated by surrounding all four orthogonal sides. Includes standard **8×8** and **Britannia 8×12** variants. | [GitHub](https://github.com/Katiuxa/Latrunculi) · [Play](https://latrunculi.vercel.app) |
| **Petteia** | Ancient Greek pincer strategy game (*ΠΕΤΤΕΙΑ*) with orthogonal rook-like movement and custodian captures. Features 5 AI difficulty levels (from *Paidion* to *Palamedes*) plus online multiplayer via room codes. | [GitHub](https://github.com/Katiuxa/Petteia) · [Play](https://petteiagame.vercel.app) |
| **Three-Trick** | Digital adaptation of the mechanical sliding-tile puzzle. Slide, lift, and drop tiles into sequential order from 1 to 9. | [GitHub](https://github.com/Katiuxa/Three-Trick) · [Play](https://tritrick.vercel.app) |
| **8 Damas** | The classic N-Queens logic puzzle—place queens so none share a row, column, or diagonal. Supports free play, pre-set puzzle boards, and 1, 3, or 5-minute time attacks across **8×8** to **11×11** grids. | [GitHub](https://github.com/Katiuxa/Ocho-Damas) · [Play](https://8damas.vercel.app) |
| **Chess Puzzles** | Android puzzle app adapting four chess compositions by Sherzod Khaydarbekov (2025): *Rook Sacrifice*, *The Black Pawn*, *Four Square*, and *Queen Moves*. Standard chess movement on constrained boards with blocked squares. | [GitHub](https://github.com/Katiuxa/Chess-Puzzles) |
| **Klotski** | Traditional *Huarongdao* sliding-block puzzle. Maneuver the surrounding blocks to free the main red piece through the bottom exit gate. | [GitHub](https://github.com/Katiuxa/Klotski) · [Play](https://huarongdaoklotski.vercel.app) |
| **Euler's Knight** | The knight's tour. Move in an L and visit every square on a **5×5**, **6×6**, **7×7**, or **8×8** board exactly once. | [GitHub](https://github.com/Katiuxa/Eulers-Knight) |

## Stack

- Systems & Networking: Linux (Debian), Bash, systemd, SSH, Tailscale, TigerVNC, zRAM.
- Development: Python, C++, JavaScript, HTML/CSS, SQLite, REST APIs.
- Embedded & Hardware: ESP32-S3, M5Stack Cardputer ADV, PlatformIO, infrared protocols, local Wi-Fi (listen-only discovery, YouTube, network remote).
- Media Processing & CLI: FFmpeg, yt-dlp, Calibre (`ebook-convert`).
- Tools: Git/GitHub, Capacitor / Android.
