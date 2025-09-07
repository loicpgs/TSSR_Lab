# 🔀 Routage & Switching

Ce document explique les bases du **switching** et du **routing**, deux fonctions clés pour construire et gérer un réseau.

---

## 🖧 Switching (Commutation)

- **Couche OSI : 2 (Liaison de données)**  
- Fonction : transmettre les trames entre les machines du même réseau local.  
- Utilise les **adresses MAC** et maintient une **table CAM** pour savoir où envoyer chaque trame.  
- **VLANs** : permettent de segmenter le réseau et isoler le trafic.  

**Types de switching :**
- **Store-and-Forward** : attend la trame complète avant d’envoyer  
- **Cut-Through** : transmet dès qu’il lit l’adresse MAC de destination  

---

## 🌍 Routing (Routage)

- **Couche OSI : 3 (Réseau)**  
- Fonction : transmettre les paquets entre réseaux différents.  
- Utilise les **adresses IP** et consulte la **table de routage** pour savoir où envoyer chaque paquet.  

**Types de routage :**
- **Statique** : routes configurées manuellement  
- **Dynamique** : protocole de routage (RIP, OSPF, BGP, EIGRP) met à jour automatiquement les routes  

---

## 🔑 Comparaison Switching vs Routing

| Fonction | Switching | Routing |
|----------|-----------|---------|
| Couche OSI | 2 | 3 |
| Adresse utilisée | MAC | IP |
| Domaine impacté | Collisions / VLAN | Réseaux différents |
| Matériel | Switch | Routeur / Switch L3 |
| Exemple | PC à PC dans le même LAN | PC vers Internet ou VLAN différent |

---

## 🛠️ Cas pratique : Inter-VLAN Routing

### 1️⃣ Router on a Stick
- Un routeur gère plusieurs VLAN via **sous-interfaces**  
- Permet la communication entre VLANs sur un lien trunk  

```bash
interface g0/0.10
  encapsulation dot1Q 10
  ip address 192.168.10.1 255.255.255.0

2️⃣ Switch L3

Le switch peut router directement entre VLANs

Activer ip routing et créer les interfaces VLAN

interface vlan 10
  ip address 192.168.10.1 255.255.255.0
ip routing

🎯 Points clés à retenir

Switch : couche 2, VLAN, MAC, LAN local

Routeur : couche 3, IP, inter-réseaux

Switch L3 : combine les deux fonctions

Comprendre tables MAC et tables de routage est fondamental pour TSSR

✍️ Ce fichier fait partie du repo TSSR_Lab pour apprendre et documenter les fondamentaux réseau.