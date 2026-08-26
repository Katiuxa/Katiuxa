# Carlos I.R.

Desarrollo de Aplicaciones Web. Soporte IT N1 y administración de sistemas. Zaragoza, España.

Administración de sistemas Linux, diagnóstico y automatización. Busco puesto en Zaragoza como soporte técnico, helpdesk o técnico de sistemas junior: entornos limitados, red y hardware, y scripting.

## Infraestructura y home lab

Servidor doméstico 24/7 donde se administra de verdad, no un laboratorio de capturas.

- Servidor: Raspberry Pi 3 Model B (Debian), 1 GB de RAM.
- Servicios persistentes con systemd (bots y File Browser).
- zRAM para no paginar en la MicroSD y aprovechar la RAM.
- Acceso remoto: SSH, TigerVNC y Tailscale. Almacenamiento en la LAN con File Browser.
- Scripts Bash: healthcheck, umbral de disco (MicroSD y USB) y rotación de logs.

Proyecto: [debian-homelab](https://github.com/Katiuxa/debian-homelab)

## Automatización e APIs

Con 1 GB no hay LLM local. La carga pesada de texto va a la nube; en la Pi queda orquestación, systemd y disco.

[Telegram-Bots-Suite](https://github.com/Katiuxa/Telegram-Bots-Suite) — bots en Python a la vez:

- API Groq con conmutación de modelo cuando se acaba la cuota.
- Transcripción y conversión de formatos (Calibre).
- Correo temporal
- Extracción de noticias.

## Web y lógica

Juegos de mesa clásicos e históricos: reglas, interfaz, web y Android.

| Proyecto | Repositorio | Jugar en el navegador |
|---|---|---|
| Ludus Latrunculorum | [Latrunculi](https://github.com/Katiuxa/Latrunculi) | [demo](https://katiuxa.github.io/Latrunculi/) |
| Petteia | [Petteia](https://github.com/Katiuxa/Petteia) | [demo](https://katiuxa.github.io/Petteia/) |
| Three-Trick | [Three-Trick](https://github.com/Katiuxa/Three-Trick) | [demo](https://katiuxa.github.io/Three-Trick/) |
| 8 Damas | [Ocho-Damas](https://github.com/Katiuxa/Ocho-Damas) | [demo](https://katiuxa.github.io/Ocho-Damas/) |
| Chess Puzzles | [Chess-Puzzles](https://github.com/Katiuxa/Chess-Puzzles) | [demo](https://katiuxa.github.io/Chess-Puzzles/) |
| Klotski | [Klotski](https://github.com/Katiuxa/Klotski) | [demo](https://katiuxa.github.io/Klotski/) |

## Stack

- Sistemas y redes: Linux (Debian), Bash, systemd, SSH, Tailscale, TigerVNC, zRAM.
- Desarrollo (DAW): Python, JavaScript, HTML/CSS, SQLite, APIs REST.
- Procesamiento y CLI: FFmpeg, yt-dlp, Calibre (`ebook-convert`).
- Herramientas: Git/GitHub, Capacitor / Android, Cursor IDE.
