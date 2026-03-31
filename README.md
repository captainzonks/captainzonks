<h2 align="left">Hellooo, I'm a Linux and Rust nerd dabbling in home server development.</h2>

###

## Spoke — Modular Self-Hosted Server Platform

[**Spoke**](https://github.com/captainzonks/spoke) is an open-source hub-and-spoke platform for running a modular home server with Docker Compose. The hub provides core infrastructure (reverse proxy, auth, security engine, database), and modules plug in as independent repos.

<details>
<summary><b>Architecture</b></summary>

```
Hub (core infrastructure)
├── Traefik         — Reverse proxy with automatic TLS
├── Authentik       — SSO and forward auth
├── CrowdSec        — AppSec WAF and IP reputation
├── PostgreSQL      — Shared database
├── Redis           — Cache and session store
├── Sablier         — On-demand container scaling
└── Socket Proxy    — Restricted Docker API access

Modules (plug-and-play service groups)
├── Each module = independent Git repo
├── 3-layer env merge (base → module defaults → site overrides)
├── Automatic Traefik rule deployment
└── Makefile orchestrates everything
```
</details>

### Modules

| Module | Description |
|--------|-------------|
| [spoke-monitoring](https://github.com/captainzonks/spoke-monitoring) | Grafana, Prometheus, Loki, Alloy, Telegraf, Dozzle, NUT |
| [spoke-plex](https://github.com/captainzonks/spoke-plex) | Plex media server with Tautulli monitoring |
| [spoke-immich](https://github.com/captainzonks/spoke-immich) | Self-hosted photo and video management |
| [spoke-music](https://github.com/captainzonks/spoke-music) | Navidrome music streaming, Picard tagging |
| [spoke-books](https://github.com/captainzonks/spoke-books) | Calibre, Audiobookshelf, GraphicAudio scraper |
| [spoke-database](https://github.com/captainzonks/spoke-database) | MinIO, InfluxDB3, CouchDB, Victoria Metrics |
| [spoke-homepage](https://github.com/captainzonks/spoke-homepage) | Homepage dashboard |
| [spoke-torrenting](https://github.com/captainzonks/spoke-torrenting) | VPN-tunneled qBittorrent and Soulseek |
| [spoke-foundryvtt](https://github.com/captainzonks/spoke-foundryvtt) | FoundryVTT virtual tabletop |
| [spoke-protonmail](https://github.com/captainzonks/spoke-protonmail) | Proton Mail Bridge SMTP/IMAP service |
| [spoke-mail-relay](https://github.com/captainzonks/spoke-mail-relay) | HTTP-to-SMTP mail relay for automated notifications |
| [GeneGnome](https://github.com/captainzonks/GeneGnome) | Genetics analysis platform (Rust/Axum API, worker, frontend) |

###

<div align="left">
  <img src="https://skillicons.dev/icons?i=rust" height="30" alt="rust logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/cplusplus/cplusplus-original.svg" height="30" alt="cplusplus logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/python/python-original.svg" height="30" alt="python logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/docker/docker-original.svg" height="30" alt="docker logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/linux/linux-original.svg" height="30" alt="linux logo"  />
</div>

###

[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/E1E21U3S1R)
