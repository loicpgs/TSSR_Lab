# Modèle OSI & TCP/IP

## 1. Modèle OSI (7 couches)
1. Physique ⚡ : câbles, signaux
2. Liaison de données 🔗 : Ethernet, MAC, ARP
3. Réseau 🌍 : IP, routage
4. Transport 📦 : TCP, UDP
5. Session 🗣️ : ouverture de session, dialogues
6. Présentation 🎭 : encodage, chiffrement
7. Application 📱 : HTTP, FTP, DNS

## 2. Suite TCP/IP (4 couches)
1. Accès réseau
2. Internet
3. Transport
4. Application

## 3. Correspondance OSI ↔ TCP/IP
| OSI | TCP/IP | Exemple |
|-----|--------|---------|
| Application, Présentation, Session | Application | HTTP, DNS |
| Transport | Transport | TCP, UDP |
| Réseau | Internet | IP, ICMP |
| Liaison + Physique | Accès réseau | Ethernet, Wi-Fi |

## 4. Points clés pour un TSSR
- OSI est théorique, TCP/IP est utilisé en pratique.
- Savoir **situer un problème réseau** (ex. : si ping ne marche pas → couche 3 Réseau).
- Utiliser Wireshark pour voir à quelle couche un protocole appartient.
