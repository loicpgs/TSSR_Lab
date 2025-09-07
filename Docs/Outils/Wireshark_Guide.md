# 🕵️ Wireshark – Guide d'utilisation

Wireshark est un outil de capture et d'analyse de paquets réseau très utilisé pour diagnostiquer et comprendre le trafic réseau.

---

## 1️⃣ Installation

- **Windows / Linux / Mac** :  
  Télécharger depuis le site officiel : [Wireshark Download](https://www.wireshark.org/download.html)  
- **Vérification après installation** :  
```bash
wireshark --version

2️⃣ Concepts clés

Capture : Enregistrement du trafic réseau sur une interface donnée.

Paquet : Unité de données transmise sur le réseau (Ethernet, IP, TCP, ICMP…).

Filtrage : Permet de sélectionner uniquement les paquets qui nous intéressent.

Exemples :

ip.addr == 192.168.1.1 – Paquets envoyés ou reçus par l’IP spécifiée

icmp – Tout le trafic ICMP (Ping, Traceroute…)

tcp.port == 80 – Tout le trafic HTTP

3️⃣ Utilisation de base

Sélectionner une interface réseau pour la capture.

Démarrer la capture et observer les paquets en temps réel.

Arrêter la capture lorsque le test ou la simulation est terminée.

Analyser les paquets : détails couche par couche (Ethernet, IP, TCP/UDP…).

4️⃣ Astuces

Couleurs : Wireshark colorie automatiquement certains types de paquets pour faciliter la lecture.

Suivi de flux TCP : clic droit sur un paquet → “Follow TCP Stream” pour voir toute la communication.

Export / sauvegarde : fichiers .pcap ou .pcapng pour réutiliser ou partager la capture.

5️⃣ Simuler Wireshark avec Packet Tracer

Packet Tracer permet de visualiser les trames comme si Wireshark était utilisé sur un vrai réseau.

Utile pour des TP ou des labs sans matériel réel.

Exporter les captures simulées sous forme d’images ou de .pkt pour documentation.

✍️ Ce guide est destiné aux étudiants TSSR pour comprendre et utiliser Wireshark dans des labs pratiques.

2️⃣ Concepts clés

Appareils réseau simulés : Routeurs, Switches, PCs, Serveurs, Access Points

Câbles :

Droits (straight-through) → PC ↔ Switch

Croisés (crossover) → Switch ↔ Switch ou PC ↔ PC

Modules : Ajouter des interfaces ou fonctionnalités aux appareils

Modes :

Réalité (Real-Time) : fonctionnement comme un vrai réseau

Simulation : analyse des paquets, couche par couche

3️⃣ Utilisation de base

Créer un réseau : glisser-déposer les appareils sur le plan de travail

Connecter les appareils avec le câble approprié

Attribuer des adresses IP et configurer les interfaces

Tester la connectivité :

ping [adresse IP]


Analyser le trafic : cliquer sur un câble → “Simulation” → suivre les paquets

4️⃣ Astuces

Visualiser ICMP et ARP pour comprendre le flux de données

Nommer et organiser les appareils dans des topologies complexes

Exporter : fichiers .pkt ou images pour documentation ou partage

✍️ Ce guide est destiné aux étudiants TSSR pour créer, simuler et documenter des réseaux pratiques en labs.