# 🔒 Sécurité Réseau – Bases

Ce document couvre les concepts fondamentaux pour sécuriser un réseau dans un environnement TSSR.

---

## 🛡️ Principes de sécurité réseau

- **Confidentialité** : protéger les données contre les accès non autorisés  
- **Intégrité** : garantir que les données ne sont pas altérées  
- **Disponibilité** : assurer l’accès aux services et systèmes légitimes  

> Les trois piliers CIAD : **Confidentialité, Intégrité, Accessibilité/Disponibilité**

---

## 🔐 Contrôle d’accès

- **Pare-feu (Firewall)** : filtre le trafic entrant et sortant selon des règles  
- **Listes de contrôle d’accès (ACL)** : règles appliquées sur routeurs ou switches pour limiter l’accès à certaines adresses ou services  
- **Segmentation réseau** : VLANs pour isoler les utilisateurs et services  

---

## 🕵️ Types de menaces

- **Interception** : sniffer le trafic réseau  
- **Altération** : modification des paquets (attaque MITM)  
- **Déni de service (DoS/DDoS)** : saturation des ressources  
- **Intrusion** : accès non autorisé à un système  

---

## 🔧 Outils de base pour TSSR

| Outil | Usage |
|-------|-------|
| Wireshark | Analyse du trafic réseau |
| Nmap | Scan de ports et découverte de réseau |
| iptables / UFW | Configuration de règles firewall Linux |
| tcpdump | Capture et analyse des paquets en ligne de commande |
| Nessus / OpenVAS | Scanner de vulnérabilités |

---

## 🛠️ Bonnes pratiques

1. **Changer les mots de passe par défaut** des équipements réseau  
2. **Activer le chiffrement** (WPA2/WPA3, SSL/TLS)  
3. **Segmenter le réseau** avec VLANs et sous-réseaux  
4. **Mettre à jour régulièrement** firmware et systèmes  
5. **Limiter les services exposés** aux seuls nécessaires  
6. **Surveiller le trafic** pour détecter les anomalies  

---

## 🎯 À retenir

- Sécurité = **prévention + détection**  
- Les VLANs, ACL, pare-feu et monitoring sont les bases pour protéger un réseau  
- Comprendre les menaces et savoir utiliser les outils de sécurité est essentiel pour TSSR  

---

✍️ *Ce fichier fait partie du repo TSSR_Lab pour documenter les bonnes pratiques de sécurité réseau.*
