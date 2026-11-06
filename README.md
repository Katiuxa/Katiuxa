# Carlos I.R.

Desarrollo de Aplicaciones Web y Android. Soporte IT N1 y administración de sistemas. Zaragoza, España.

Administración de sistemas Linux, diagnóstico y automatización.

## Infraestructura y home lab

Servidor doméstico 24/7.

- Servidor: Raspberry Pi 3 Model B (Debian), 1 GB de RAM.
- Servicios persistentes con systemd (bots y File Browser).
- zRAM para no paginar en la MicroSD y aprovechar la RAM.
- Acceso remoto: SSH, TigerVNC y Tailscale. Almacenamiento en la LAN con File Browser.
- Scripts Bash: healthcheck, umbral de disco (MicroSD y USB) y rotación de logs.

Proyecto: [debian-homelab](https://github.com/Katiuxa/debian-homelab)

## Automatización y APIs

Con 1 GB no hay LLM local. La carga pesada de texto va a la nube; en la Pi queda orquestación, systemd y disco.

[Telegram-Bots-Suite](https://github.com/Katiuxa/Telegram-Bots-Suite) — bots en Python a la vez:

- API Groq con conmutación de modelo cuando se acaba la cuota.
- Transcripción y conversión de formatos (Calibre).
- Correo temporal.
- Extracción de noticias.
- [Biblioteca Secreta](https://github.com/Katiuxa/Telegram-Bots-Suite/tree/main/BotBiblioteca): catálogo de epubs en el USB. Búsqueda en SQLite por título o autor y envío del fichero por Telegram. La base y los libros no están en GitHub; solo el código.

[Meta-LLM](https://github.com/Katiuxa/Meta-LLM) es el chat aparte. Telegram y un panel en el puerto 5000. OpenRouter hace de pasarela: desde el propio menú cambio de modelo. Dolphin Venice, Cydonia, Euryale, Hermes y compañía van con pocos rechazos (charla, relato, roleplay). Qwen3 Coder y Command R+ se quedan con filtro, para código y textos largos. Las imágenes pasan por Gemini Flash Image, también en OpenRouter. La clave y el token del bot viven en el `.env` de la Pi.

## Web y lógica

Juegos de mesa clásicos e históricos: reglas, interfaz, web y Android.

| Proyecto | Repositorio | Jugar en el navegador |
|---|---|---|
| Ludus Latrunculorum | [Latrunculi](https://github.com/Katiuxa/Latrunculi) | [demo](https://latrunculigame.vercel.app) |
| Petteia | [Petteia](https://github.com/Katiuxa/Petteia) | [demo](https://petteiagame.vercel.app) |
| Three-Trick | [Three-Trick](https://github.com/Katiuxa/Three-Trick) | [demo](https://tritrick.vercel.app) |
| 8 Damas | [Ocho-Damas](https://github.com/Katiuxa/Ocho-Damas) | [demo](https://8damas.com) |
| Chess Puzzles | [Chess-Puzzles](https://github.com/Katiuxa/Chess-Puzzles) | [demo](https://puzzleschess.vercel.app) |
| Klotski | [Klotski](https://github.com/Katiuxa/Klotski) | [demo](https://huarongdaoklotski.vercel.app) |

## Stack

- Sistemas y redes: Linux (Debian), Bash, systemd, SSH, Tailscale, TigerVNC, zRAM.
- Desarrollo (DAW): Python, JavaScript, HTML/CSS, SQLite, APIs REST.
- Procesamiento y CLI: FFmpeg, yt-dlp, Calibre (`ebook-convert`).
- Herramientas: Git/GitHub, Capacitor / Android.
