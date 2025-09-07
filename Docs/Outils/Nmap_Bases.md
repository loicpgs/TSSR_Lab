# 🔍 Nmap – Bases et utilisation

Nmap (Network Mapper) est un outil libre de scan et d’audit réseau, utilisé pour découvrir des hôtes, services et vulnérabilités.

---

## 1️⃣ Installation

- Téléchargement officiel : [https://nmap.org/download.html](https://nmap.org/download.html)  
- Compatible **Windows**, **Linux**, **Mac**  
- Vérification :  


## 2️⃣ Concepts clés

**Hôte** : un périphérique réseau détecté (PC, serveur, switch…)

**Port** : point d’accès réseau sur un hôte

**Service** : application écoutant sur un port (HTTP, SSH…)

**Scan** : méthode pour détecter les hôtes et services actifs

**OS Detection** : identification du système d’exploitation

## 3️⃣ Utilisation de base

**Scanner un réseau** :

nmap 192.168.1.0/24

**Scanner un port précis** :

nmap -p 80 192.168.1.10

**Scan complet avec détection d’OS et services** :

nmap -A 192.168.1.10

**Mode verbeux pour détails** :

nmap -v 192.168.1.0/24

## 4️⃣ Astuces

**Exporter les résultats :**

nmap -oN resultat_scan.txt 192.168.1.0/24

**scanner rapidement** : nmap -F [IP]

Utiliser des scripts Nmap : nmap --script [nom_script] [IP]

✍️ Ce guide est destiné aux étudiants TSSR pour découvrir et comprendre les bases du scanning réseau avec Nmap.
