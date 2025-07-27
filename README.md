# BlerdFlixx Jellyfin Stack (Media2)

This repo tracks my entire media server stack running in LXC container 102 on Proxmox.

## Stack Includes

- Jellyfin (with custom "BlerdFlixx" frontend)
- qBittorrent + Gluetun
- Radarr / Sonarr / SABnzbd
- Docker Compose config
- Configs for persistent volumes

## Structure

- `jellyfin-config/`: All mounted app configs
- `jellyfin-theme/`: Forked frontend for Jellyfin web UI
- `docker-compose.yml`: The full orchestration stack

## Deploy

```bash
cd /srv/jellyfin-server
docker compose up -d
