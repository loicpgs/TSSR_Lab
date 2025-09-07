# Lab1 – Notes Packet Tracer

Ce document décrit **pas à pas les actions réalisées dans Packet Tracer** pour le Lab1, avec les captures correspondantes.

---

## 1️⃣ Structuration du réseau

- Topologie simple : 2 PC + 1 switch connectés par des câbles droits.
- Chaque PC connecté au switch.

![Step 1](Lab1_Step1.png)

---

## 2️⃣ Attribution des IP

- **PC1** : `192.168.1.10 /24`  
- **PC2** : `192.168.1.11 /24`  

![Step 2](Lab1_Step2.png)  
![Step 3](Lab1_Step3.png)

---

## 3️⃣ Test de connectivité (Ping)

- Ping depuis PC1 vers PC2 et inversement pour vérifier la communication.
- Résultat : **réussi**, réseau fonctionnel.

![Step 4](Lab1_Step4.png)  
![Step 5](Lab1_Step5.png)

---

## 4️⃣ Simulation Wireshark et diagnostic

- Envoi de paquets ICMP entre PC1 et PC2.  
- Vérification du modèle OSI pour ICMP.  
- Vérification du STP sur le switch pour éviter les boucles.

![Step 6](Lab1_Step6.png)  
![Step 7](Lab1_Step7.png)  
![Step 8](Lab1_Step8.png)

---

> Ce document peut être utilisé pour expliquer le déroulement du Lab1, même sans Packet Tracer ouvert.
