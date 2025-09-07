# 🌐 Adressage IP & VLANs

Ce document présente les notions d’**adressage IP** et de **VLANs** essentielles pour tout technicien systèmes et réseaux (TSSR).

---

## 🖧 1. Adressage IP

### IPv4
- Format : **32 bits** = 4 octets (ex: `192.168.1.10`)
- Écrit en **décimal pointé**
- Divisé en **réseau** et **hôte**

### Classes d’adresses
- Classe A : `0.0.0.0 – 127.255.255.255` (ex: 10.0.0.0/8)  
- Classe B : `128.0.0.0 – 191.255.255.255` (ex: 172.16.0.0/16)  
- Classe C : `192.0.0.0 – 223.255.255.255` (ex: 192.168.0.0/24)  

👉 Aujourd’hui on préfère utiliser les **CIDR** (notation `/24`, `/16` etc.)

### IPv6
- Format : **128 bits** (ex: `2001:db8::1`)  
- Beaucoup plus d’adresses possibles  
- Syntaxe en hexadécimal, séparée par `:`  

---

## 📏 2. Masque de sous-réseau

Le **masque** définit la partie "réseau" et la partie "hôte".

- Exemple :  
  - Adresse IP : `192.168.1.10`  
  - Masque : `255.255.255.0` ou `/24`  
  - Réseau : `192.168.1.0`  
  - Broadcast : `192.168.1.255`  
  - Plage d’hôtes : `192.168.1.1 – 192.168.1.254`

---

## 🌍 3. VLANs (Virtual LAN)

### Définition
Un **VLAN** = un réseau local virtuel, séparé logiquement sur un même switch.  
Chaque VLAN est **isolé** des autres → sécurité et organisation.

### Avantages
- Isolation des flux (ex: Production / Admin / Invités)  
- Réduction du broadcast  
- Sécurité accrue  
- Gestion flexible du réseau  

### Fonctionnement
- Chaque port du switch est affecté à un VLAN (ex: VLAN 10, VLAN 20)  
- Communication entre VLANs = via un **routeur** ou un **switch de niveau 3**  
- Les trames VLAN portent un **tag 802.1Q**

---

## 🛠️ 4. Exemple pratique

### Plan d’adressage
| VLAN | Usage       | Réseau          | Passerelle    |
|------|-------------|-----------------|---------------|
| 10   | Admin       | 192.168.10.0/24 | 192.168.10.1 |
| 20   | Utilisateurs| 192.168.20.0/24 | 192.168.20.1 |
| 30   | Invités     | 192.168.30.0/24 | 192.168.30.1 |

### Sur un switch
- Port 1–5 → VLAN 10 (Admin)  
- Port 6–15 → VLAN 20 (Utilisateurs)  
- Port 16–20 → VLAN 30 (Invités)  

### Communication
- PC Admin (192.168.10.5) → PC Utilisateur (192.168.20.8)  
  👉 Besoin d’un **routeur ou L3 switch** pour inter-VLAN routing.  

---

## 🔍 5. Liens avec le modèle OSI

- VLANs = **Couche 2 (Liaison de données)** (séparation logique des trames Ethernet)  
- Adressage IP = **Couche 3 (Réseau)** (identification et routage des paquets)  

---

## 🎯 À retenir pour TSSR
- **IP = identité logique** d’un hôte  
- **VLAN = séparation logique** des réseaux sur un switch  
- Communication entre VLANs = nécessite un **équipement de routage**  
- Toujours bien documenter son **plan d’adressage**  

---

✍️ *Document préparé pour le repo TSSR_Lab (formation TSSR / AdminSys).*  
