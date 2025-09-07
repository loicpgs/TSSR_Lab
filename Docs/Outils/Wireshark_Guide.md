# 🕵️ Wireshark – Guide d'utilisation

Wireshark est un outil de capture et d'analyse de paquets réseau très utilisé pour diagnostiquer et comprendre le trafic réseau.

---

## 1️⃣ Installation

- **Windows / Linux / Mac** :  
  Télécharger depuis le site officiel : [Wireshark Download](https://www.wireshark.org/download.html)  
- **Vérification après installation** :  

wireshark --version

## 2️⃣ Concepts clés

**Capture** : Enregistrement du trafic réseau sur une interface donnée.

**Paquet** : Unité de données transmise sur le réseau (Ethernet, IP, TCP, ICMP…).

**Filtrage** : Permet de sélectionner uniquement les paquets qui nous intéressent.

**Exemples :**

ip.addr == 192.168.1.1 – Paquets envoyés ou reçus par l’IP spécifiée

icmp – Tout le trafic ICMP (Ping, Traceroute…)

tcp.port == 80 – Tout le trafic HTTP

## 3️⃣ Utilisation de base 

**Sélectionner** une **interface réseau** pour la capture.

**Démarrer** la capture et **observer les paquets** en temps réel.

**Arrêter** la capture lorsque le test ou la simulation est terminée.

**Analyser les paquets** : détails couche par couche (Ethernet, IP, TCP/UDP…).

## 4️⃣ Astuces

**Couleurs** : Wireshark colorie automatiquement certains types de paquets pour faciliter la lecture.

**Suivi de flux TCP** : clic droit sur un paquet → “Follow TCP Stream” pour voir toute la communication.

**Export / sauvegarde** : fichiers .pcap ou .pcapng pour réutiliser ou partager la capture.

## 5️⃣ Simuler Wireshark avec Packet Tracer

Packet Tracer permet de visualiser les trames comme si Wireshark était utilisé sur un vrai réseau.

**Utile pour des TP ou des labs sans matériel réel.**

**Exporter** les captures simulées sous forme d’images ou de **.pkt**pour documentation.

✍️ Ce guide est destiné aux étudiants TSSR pour comprendre et utiliser Wireshark dans des labs pratiques.


