# 🐧 Commandes Linux – Bases pour TSSR

Ce document recense les commandes Linux essentielles pour un technicien systèmes et réseaux (TSSR).

---

## 1️⃣ Gestion des fichiers et dossiers

| Commande | Description | Exemple |
|----------|-------------|---------|
| `ls` | Lister les fichiers d’un répertoire | `ls -l` |
| `cd` | Changer de répertoire | `cd /home/user` |
| `pwd` | Afficher le chemin du répertoire courant | `pwd` |
| `mkdir` | Créer un répertoire | `mkdir Projet` |
| `rm` | Supprimer un fichier ou dossier | `rm fichier.txt` / `rm -r dossier` |
| `cp` | Copier fichier ou dossier | `cp source.txt dest.txt` |
| `mv` | Déplacer ou renommer | `mv ancien.txt nouveau.txt` |
| `cat` | Afficher le contenu d’un fichier | `cat fichier.txt` |
| `less` | Lire un fichier page par page | `less fichier.txt` |
| `touch` | Créer un fichier vide | `touch fichier.txt` |

---

## 2️⃣ Gestion des utilisateurs et permissions

| Commande | Description | Exemple |
|----------|-------------|---------|
| `whoami` | Afficher l’utilisateur courant | `whoami` |
| `id` | Afficher UID/GID et groupes | `id` |
| `chmod` | Modifier permissions fichier/dossier | `chmod 644 fichier.txt` |
| `chown` | Changer propriétaire | `chown user:group fichier.txt` |
| `passwd` | Modifier mot de passe | `passwd user` |
| `groups` | Afficher les groupes de l’utilisateur | `groups` |

---

## 3️⃣ Gestion des processus et services

| Commande | Description | Exemple |
|----------|-------------|---------|
| `ps` | Lister les processus en cours | `ps aux` |
| `top` | Moniteur des processus et ressources | `top` |
| `kill` | Terminer un processus par PID | `kill 1234` |
| `systemctl` | Gérer les services | `systemctl status ssh` |
| `service` | Démarrer/stopper un service (anc.) | `service ssh start` |

---

## 4️⃣ Gestion des fichiers journaux et logs

| Commande | Description | Exemple |
|----------|-------------|---------|
| `dmesg` | Afficher messages du kernel | `dmesg | less` |
| `tail` | Lire fin d’un fichier | `tail -f /var/log/syslog` |
| `journalctl` | Logs systèmes (systemd) | `journalctl -u ssh` |

---

## 5️⃣ Gestion réseau

| Commande | Description | Exemple |
|----------|-------------|---------|
| `ifconfig` / `ip addr` | Afficher les interfaces réseau | `ip addr` |
| `ping` | Tester la connectivité | `ping 8.8.8.8` |
| `netstat` / `ss` | Voir connexions et ports | `ss -tuln` |
| `traceroute` | Suivre le chemin vers une IP | `traceroute google.com` |
| `nslookup` / `dig` | Résolution DNS | `dig example.com` |

---

## 6️⃣ Gestion des packages

| Commande | Description | Exemple |
|----------|-------------|---------|
| `apt-get update` | Mettre à jour la liste des packages (Debian/Ubuntu) | `sudo apt-get update` |
| `apt-get upgrade` | Mettre à jour les packages installés | `sudo apt-get upgrade` |
| `yum update` | Mise à jour (RedHat/CentOS) | `sudo yum update` |
| `dpkg -i` | Installer un package .deb | `sudo dpkg -i package.deb` |

---

## 7️⃣ Raccourcis utiles

- `Ctrl + C` : interrompre une commande  
- `Ctrl + Z` : suspendre une commande  
- `Ctrl + R` : recherche dans l’historique des commandes  
- `!!` : répéter la dernière commande  
- `history` : afficher l’historique  

---

✍️ *Ce fichier fait partie du repo TSSR_Lab et regroupe les commandes Linux essentielles pour un technicien systèmes et réseaux.*
