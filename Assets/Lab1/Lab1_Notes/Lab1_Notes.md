# Projet LAN : 2 PC + 1 Switch

Ce petit projet illustre la configuration d’un réseau local simple avec **deux PC et un switch** dans Packet Tracer.

---

## 1. Topologie du réseau

![Topologie du réseau](https://github.com/loicpgs/TSSR_Lab/blob/e68b677863e3fba0e84ffa388de89b0ea5f96741/Assets/Lab1/Lab1_Captures.md/Capture%20d'%C3%A9cran%202025-09-08%20174745.png)

Description :  
- PC1 connecté au switch.  
- PC2 connecté au switch.  
- Pas de routeur dans ce simple LAN.

---

## 2. Configuration IP du PC1

![Configuration IP PC1](https://github.com/loicpgs/TSSR_Lab/blob/e68b677863e3fba0e84ffa388de89b0ea5f96741/Assets/Lab1/Lab1_Captures.md/Capture%20d'%C3%A9cran%202025-09-08%20174757.png)

Paramètres :  
- IP : 192.168.1.10  
- Masque : 255.255.255.0  
- Gateway : 192.168.1.1 (optionnel)

---

## 3. Configuration IP du PC2

![Configuration IP PC2](https://github.com/loicpgs/TSSR_Lab/blob/e68b677863e3fba0e84ffa388de89b0ea5f96741/Assets/Lab1/Lab1_Captures.md/Capture%20d'%C3%A9cran%202025-09-08%20174805.png)

Paramètres :  
- IP : 192.168.1.20  
- Masque : 255.255.255.0  
- Gateway : 192.168.1.1 (optionnel)

---

## 4. Test de connectivité

![Test ping PC1 → PC2](https://github.com/loicpgs/TSSR_Lab/blob/e68b677863e3fba0e84ffa388de89b0ea5f96741/Assets/Lab1/Lab1_Captures.md/Capture%20d'%C3%A9cran%202025-09-08%20174918.png)

- PC1 → PC2 : `ping 192.168.1.20`  
- PC2 → PC1 : `ping 192.168.1.10`  
- Résultat : succès, le LAN fonctionne correctement.

---

## 5. Résumé

- Tous les périphériques sont sur le même **réseau 192.168.1.0/24**.  
- Le switch fonctionne en **Layer 2**, aucun routage nécessaire.  
- Ce lab illustre les **bases de l’adressage IP et du test de connectivité** pour un réseau local simple.
