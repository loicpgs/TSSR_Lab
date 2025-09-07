# 🪟 Commandes Windows & PowerShell – Bases pour TSSR

Ce document recense les commandes Windows et PowerShell essentielles pour un technicien systèmes et réseaux (TSSR).

---

## 1️⃣ Gestion des fichiers et dossiers

| Commande | Description | Exemple |
|----------|-------------|---------|
| `dir` | Lister les fichiers d’un répertoire | `dir C:\Users` |
| `cd` | Changer de répertoire | `cd C:\Windows\System32` |
| `mkdir` | Créer un dossier | `mkdir C:\Test` |
| `rmdir` | Supprimer un dossier | `rmdir C:\Test` |
| `del` | Supprimer un fichier | `del fichier.txt` |
| `copy` | Copier un fichier | `copy source.txt dest.txt` |
| `move` | Déplacer ou renommer un fichier | `move ancien.txt nouveau.txt` |

---

## 2️⃣ Gestion des utilisateurs et permissions

| Commande | Description | Exemple |
|----------|-------------|---------|
| `whoami` | Afficher l’utilisateur courant | `whoami` |
| `net user` | Lister les utilisateurs | `net user` |
| `net user [nom] [motdepasse] /add` | Créer un utilisateur | `net user test P@ssword1 /add` |
| `net localgroup Administrators [nom] /add` | Ajouter un utilisateur au groupe Admin | `net localgroup Administrators test /add` |
| `icacls` | Gérer permissions fichiers/dossiers | `icacls C:\Test /grant User:F` |

---

## 3️⃣ Gestion des processus et services

| Commande | Description | Exemple |
|----------|-------------|---------|
| `tasklist` | Lister les processus en cours | `tasklist` |
| `taskkill` | Terminer un processus par PID | `taskkill /PID 1234 /F` |
| `Get-Process` | Lister les processus PowerShell | `Get-Process` |
| `Stop-Process` | Arrêter un processus PowerShell | `Stop-Process -Id 1234` |
| `Get-Service` | Lister services Windows | `Get-Service` |
| `Start-Service` | Démarrer un service | `Start-Service -Name Spooler` |
| `Stop-Service` | Arrêter un service | `Stop-Service -Name Spooler` |

---

## 4️⃣ Gestion réseau

| Commande | Description | Exemple |
|----------|-------------|---------|
| `ipconfig` | Afficher les informations IP | `ipconfig /all` |
| `ping` | Tester la connectivité | `ping 8.8.8.8` |
| `tracert` | Suivre le chemin vers une IP | `tracert google.com` |
| `Get-NetIPAddress` | Afficher les IP PowerShell | `Get-NetIPAddress` |
| `Test-Connection` | Ping avancé PowerShell | `Test-Connection google.com -Count 4` |
| `Get-NetAdapter` | Lister les cartes réseau | `Get-NetAdapter` |

---

## 5️⃣ Gestion des disques et fichiers système

| Commande | Description | Exemple |
|----------|-------------|---------|
| `chkdsk` | Vérifier un disque | `chkdsk C:` |
| `diskpart` | Gérer partitions disque | `diskpart` |
| `Get-ChildItem` | Lister fichiers PowerShell | `Get-ChildItem C:\Test` |
| `Copy-Item` | Copier fichier/dossier | `Copy-Item C:\Source\* C:\Dest\` |
| `Move-Item` | Déplacer fichier/dossier | `Move-Item C:\Source\* C:\Dest\` |
| `Remove-Item` | Supprimer fichier/dossier | `Remove-Item C:\Test -Recurse -Force` |

---

## 6️⃣ Astuces PowerShell

- `Ctrl + C` : interrompre la commande  
- `Tab` : autocomplétion des noms de fichiers/dossiers  
- `Get-Help [commande]` : obtenir la documentation d’une commande  
- `Get-Command` : lister toutes les commandes disponibles  
- `history` ou `Get-History` : afficher l’historique des commandes  

---

✍️ *Ce fichier fait partie du repo TSSR_Lab et regroupe les commandes Windows et PowerShell essentielles pour un technicien systèmes et réseaux.*
