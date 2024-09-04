# Holodeck project
## Description du sujet
### Contraintes matérielles
Commençons par les contraintes matérielles au niveau des
machines virtuelles

| VM / Caractéristiques | Serveur | Client |
| :-------------------- | :-----: | :----: |
| OS | Debian 12.7 | Debian 12.7 |
| vCPU | 2 | 2 |
| RAM | 2048 Mo | 2048 Mo |
| Disk | 32 Go | 16 Go |
| ethernet link 1 | (ens33) 00:0c:29:95:2b:e5 | (ens37) 00:0c:29:b9:a9:7c |
| ethernet link 2 | (ens33) 00:0c:29:95:2b:ef | (ens37) 00:0c:29:b9:a9:86 |

### Réseaux

| Machine | Interface | Type | IP | Réseau | Passerelle |
| :-------------------- | :----: | :----: | :----: | :----: | :----: |
| Serveur | ens33 | NAT | dynamic | 192.168.246.0/24 | 192.168.246.2 |
| Serveur | ens37 | Host-only | 192.168.10.10 | 192.268.10.0 / 24 | X |
| Client | ens33 | NAT | dynamic | 192.168.246.0/24 | 192.168.246.2 |
| Client | ens37 | Host-only | dynamic | 192.268.10.0 / 24 | X |
 

