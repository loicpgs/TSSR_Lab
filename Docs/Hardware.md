# 📄 Composants essentiels d’un PC – Vue TSSR

## 1. Carte Mère (Motherboard)
- **Rôle** : Support physique qui relie tous les composants (CPU, RAM, cartes d’extension, périphériques).
- **Importance TSSR** : 
  - Comprendre les emplacements (slots) pour diagnostics matériels.
  - Identifier les connecteurs (SATA, M.2, PCIe).
  - Vérifier compatibilités (RAM/CPU/Chipset).

---

## 2. Chipset
- **Rôle** : Contrôleur intégré à la carte mère qui gère la communication entre CPU, RAM, GPU, stockage et périphériques.
- **Northbridge** (anciennement) : RAM + PCIe + GPU.
- **Southbridge** (anciennement) : USB, SATA, réseau, audio.
- **Importance TSSR** :
  - Influence la compatibilité (type de RAM, nombre de ports, support virtualisation).
  - Impact sur performances et gestion d’énergie.

---

## 3. Processeur (CPU)
- **Rôle** : Cerveau de la machine, exécute les instructions.
- **Caractéristiques clés** :
  - Nombre de cœurs et threads (impact multitâche).
  - Fréquence (GHz).
  - Cache (L1, L2, L3).
  - Support des instructions (64 bits, virtualisation Intel VT-x / AMD-V).
- **Importance TSSR** :
  - Performance pour VM, serveurs, calculs réseaux.
  - Choix selon usage (bureautique, serveur, cloud).

---

## 4. Mémoire Vive (RAM)
- **Rôle** : Stockage temporaire et rapide des données utilisées par le CPU.
- **Caractéristiques** :
  - Capacité (Go).
  - Fréquence (MHz).
  - Latence (CL).
  - Type (DDR3, DDR4, DDR5).
- **Importance TSSR** :
  - Critique pour serveurs et VM.
  - Diagnostiquer pannes (test memtest).
  - Optimiser allocations (virtualisation, conteneurs).

---

## 5. Bus et Lignes de Communication
- **Front Side Bus (FSB)** : Ancien lien CPU ↔ chipset.
- **PCIe** : Connecte GPU, SSD NVMe, cartes réseaux.
- **SATA/NVMe** : Interfaces de stockage.
- **USB** : Périphériques externes.
- **Importance TSSR** :
  - Comprendre limites de débit (Gb/s).
  - Dépanner lenteurs liées aux bus saturés.

---

## 6. Stockage
- **Types** :
  - HDD : grande capacité, lent.
  - SSD SATA : rapide, fiable.
  - NVMe : très rapide, connecté en PCIe.
- **Importance TSSR** :
  - Impact sur performances systèmes/VM.
  - Sauvegardes et migrations.
  - RAID (sécurité et tolérance aux pannes).

---

## 7. Carte Graphique (GPU)
- **Rôle** : Calcul et affichage graphique.
- **Importance TSSR** :
  - Peu critique en serveur, sauf pour calculs (GPU computing, IA).
  - Pertinent en VDI (infrastructures bureaux virtuels).

---

## 8. Carte Réseau (NIC)
- **Rôle** : Connexion au réseau (Ethernet, Wi-Fi).
- **Caractéristiques** :
  - Débit (1 Gbps, 10 Gbps…).
  - Support VLAN, PXE boot.
- **Importance TSSR** :
  - Cruciale pour accès distant, déploiement, monitoring.
  - Redondance avec plusieurs interfaces.

---

## 9. Alimentation (PSU)
- **Rôle** : Fournit l’énergie électrique aux composants.
- **Importance TSSR** :
  - Pannes fréquentes → diagnostics.
  - Notion de puissance (Watt).
  - Efficacité (80 PLUS).

---

## 10. Système de Refroidissement
- **Types** :
  - Ventirads, watercooling, refroidissement passif.
- **Importance TSSR** :
  - Impact sur fiabilité et durée de vie.
  - Monitoring température (surchauffe serveur = panne).

---

## 11. BIOS / UEFI
- **Rôle** : Logiciel bas niveau qui initialise le matériel.
- **Fonctions utiles TSSR** :
  - Boot order.
  - Activation virtualisation.
  - Sécurisation (Secure Boot, mot de passe BIOS).
  - Mise à jour firmware.

---

# ✅ Synthèse pour un TSSR
Un technicien doit savoir :
- Identifier les composants et leurs rôles.
- Diagnostiquer pannes matérielles (RAM, PSU, disque).
- Vérifier compatibilités (chipset/CPU/RAM).
- Optimiser la configuration pour les usages (serveur, virtualisation, réseau).
- Gérer le BIOS/UEFI et options de virtualisation/sécurité.
