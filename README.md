# docker seedbox

Installation d'une Seedbox complète sous Debian 10

## Architecture

Filesystem : 
- / --> 50Go
- /home --> le reste 

Installation des conteneurs:
- Suite logicielle de la seedbox: `~/docker/seedbox`
- Traefik: `~/docker/traefik`
- Utilitaire d'administration: `~/docker/admin`
- Dossier des télécharments: `~/docker/downloads/<app>`

## Détail des applications

Système: 
- Traefik : Loadbalancer / Reverse-Proxy : Redirection dynamique des flux internet vers les conteneurs. Supporte le http/https et les couches tcp/udp.
- Prometheus/Grafana : Permet de monitorer l'essentiel de la plateforme. 
- Keycloak : Application de management des identifiants
- ELK : Aggregateur de logs. Permet de centraliser les logs
- Duplicati : Sauvegarde

Seedbox: 
- Radarr
- Sonarr
- Lidarr
- Plex
- pyLoad
- Jackett
- Organizr
- Flood
- rTorrent
- ruTorrent


