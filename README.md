# Docker Compose Stack

This repository contains a collection of **Docker Compose configurations** used for self-hosting media services and supporting infrastructure.  
The setup is modular, practical, and intended for both **learning purposes** and **personal use**.

## Contents

### Media Server
- **Jellyfin**  
  Self-hosted media server for movies, series, and music.

### *arr Stack (Media Automation)
- **Prowlarr** – Indexer manager
- **Radarr** – Movie management
- **Sonarr** – TV series management
- **Bazarr** – Subtitle management
- **qBittorrent** – Torrent client
- **Gluetun** – VPN container for secure traffic routing
- **FlareSolverr** – Cloudflare challenge solver for indexers

All *arr services are designed to work together as a single automated pipeline.

### Maintenance
- **Watchtower**  
  Automatically updates running containers when new images are available.

## Structure

Each service or stack is defined using its own `docker-compose.yml`, allowing:
- Independent deployment
- Easy modification
- Clear separation of concerns

Environment variables and volume mappings are expected to be customized per system.

## Requirements
- Docker
- Docker Compose (v2)
- Basic understanding of container networking and volumes

## Usage

Clone the repository:
```bash
git clone https://github.com/yourusername/your-repo-name.git
cd your-repo-name
