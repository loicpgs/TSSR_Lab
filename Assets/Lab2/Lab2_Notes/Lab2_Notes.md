# Lab2 : LAN avec 3 PC et 1 serveur HTTP

Ce laboratoire illustre la configuration d'un réseau local simple avec trois PC et un serveur HTTP dans Cisco Packet Tracer.

---

## 1. Topologie du réseau

![Topologie du réseau](https://github.com/loicpgs/TSSR_Lab/blob/edf4a9c4e142abb7350ef427086067055f42280c/Assets/Lab2/Lab2_Captures/Capture%20d'%C3%A9cran%202025-09-08%20204257.png)

**Description :**
- Trois PC connectés à un switch.
- Un serveur HTTP connecté au même switch.
- Pas de routeur nécessaire pour ce LAN simple.

---

## 2. Plan d'adressage IP

| Appareil   | Adresse IP    | Masque de sous-réseau | Passerelle |
|------------|---------------|-----------------------|------------|
| PC1        | 192.168.1.10  | 255.255.255.0         | 192.168.1.1 |
| PC2        | 192.168.1.11  | 255.255.255.0         | 192.168.1.1 |
| PC3        | 192.168.1.12  | 255.255.255.0         | 192.168.1.1 |
| ServeurHTTP| 192.168.1.13  | 255.255.255.0         | 192.168.1.1 |

---

## 3. Configuration des périphériques

### PC1, PC2 et PC3
- Accéder à l'onglet **Desktop** → **IP Configuration**.
- Saisir l'adresse IP, le masque de sous-réseau et la passerelle.

![Configuration Ips](https://github.com/loicpgs/TSSR_Lab/blob/edf4a9c4e142abb7350ef427086067055f42280c/Assets/Lab2/Lab2_Captures/Capture%20d'%C3%A9cran%202025-09-08%20204433.png)

### Serveur HTTP
- Accéder à l'onglet **Desktop** → **IP Configuration**.
- Saisir l'adresse IP, le masque de sous-réseau et la passerelle.
- Accéder à l'onglet **Services** → **HTTP**.
- Activer le service HTTP.

![Serveur HTTP](https://github.com/loicpgs/TSSR_Lab/blob/edf4a9c4e142abb7350ef427086067055f42280c/Assets/Lab2/Lab2_Captures/Capture%20d'%C3%A9cran%202025-09-08%20204731.png)
---

## 4. Test de connectivité (Ping)

### PC1 → Serveur HTTP

![Ping de PC1 vers le serveur HTTP](https://github.com/loicpgs/TSSR_Lab/blob/edf4a9c4e142abb7350ef427086067055f42280c/Assets/Lab2/Lab2_Captures/Capture%20d'%C3%A9cran%202025-09-08%20204959.png)

**Commande :**

ping 192.168.1.13

## 5. Test HTTP

**Depuis PC1 :** Accéder à l'onglet Desktop → Web Browser.

Saisir l'adresse http://192.168.1.13.

**La page d'accueil du serveur HTTP devrait s'afficher.**

![Test HTTP](https://github.com/loicpgs/TSSR_Lab/blob/edf4a9c4e142abb7350ef427086067055f42280c/Assets/Lab2/Lab2_Captures/Capture%20d'%C3%A9cran%202025-09-08%20205227.png)

## 6. Résumé

Tous **les périphériques** sont sur le **même réseau 192.168.1.0/24.**

Le switch fonctionne en **Layer 2**, aucun routage nécessaire.

Ce laboratoire permet de pratiquer :

**L'adressage IP statique**

**Le test de connectivité avec ping**

**L'accès HTTP au serveur**
