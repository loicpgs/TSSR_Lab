# 🌐 Packet Tracer – Guide d'utilisation

Packet Tracer est un simulateur réseau développé par Cisco, utilisé pour apprendre et tester des configurations réseau sans matériel réel.

---

## 1️⃣ Installation

- Télécharger depuis le site officiel Cisco Networking Academy : [Packet Tracer](https://www.netacad.com/courses/packet-tracer)  
- Disponible pour **Windows**, **Linux** et **Mac**.  
- Vérification de l'installation :
```bash
packettracer --version

2️⃣ Concepts clés

Appareils réseau simulés : Routeurs, Switches, PCs, Serveurs, Access Points.

Câbles :

Droits (straight-through) → PC ↔ Switch

Croisés (crossover) → Switch ↔ Switch ou PC ↔ PC

Modules : Permettent d’ajouter interfaces supplémentaires aux appareils.

Simulation et temps réel :

Mode Réel : fonctionnement comme un vrai réseau

Mode Simulation : analyse des trames, suivi des paquets couche par couche

3️⃣ Utilisation de base

Créer un réseau : glisser-déposer les appareils.

Connecter les appareils avec les câbles appropriés.

Attribuer des IP et configurer les interfaces.

Tester la connectivité :

ping [adresse IP]

Analyser le trafic : cliquer sur un câble → “Simulation” pour suivre les paquets.

4️⃣ Astuces

Utiliser les modèles d’ICMP et ARP pour comprendre le flux de données.

Étiqueter les appareils pour mieux organiser les topologies complexes.

Exporter les topologies et captures en images ou .pkt pour documentation et partage.

✍️ Ce guide est destiné aux étudiants TSSR pour créer, simuler et documenter des réseaux pratiques en labs.