# 🖥️ Virtualisation – Bases pour TSSR

Ce document présente les concepts, outils et bonnes pratiques liés à la virtualisation pour un technicien systèmes et réseaux (TSSR).

---

## 1️⃣ Concepts clés

- **Hyperviseur** : logiciel permettant de créer et gérer des machines virtuelles (VM).  
  - **Type 1 (Bare-metal)** : installé directement sur le matériel (ex : VMware ESXi, Hyper-V).  
  - **Type 2 (Hosted)** : installé sur un OS hôte (ex : VirtualBox, VMware Workstation).  
- **Machine virtuelle (VM)** : environnement simulant un ordinateur complet, isolé et indépendant.  
- **Snapshot** : capture de l’état d’une VM à un instant précis, utile pour restaurer.  
- **Template** : VM préconfigurée servant de modèle pour déploiement rapide.  

---

## 2️⃣ Avantages de la virtualisation

- Optimisation de l’utilisation des ressources matérielles (CPU, RAM, stockage).  
- Isolation des environnements pour tests et production.  
- Sauvegarde et restauration simplifiées grâce aux snapshots.  
- Déploiement rapide de nouvelles machines via templates.  

---

## 3️⃣ Outils courants

| Outil | Type | Utilisation principale |
|-------|------|----------------------|
| VirtualBox | Type 2 | VM sur poste de travail |
| VMware Workstation | Type 2 | VM sur poste de travail |
| VMware ESXi | Type 1 | Hyperviseur serveur |
| Hyper-V | Type 1 | Hyperviseur Windows Server |
| Proxmox VE | Type 1 | Virtualisation serveur, containers LXC |
| Docker | Conteneurs | Virtualisation légère pour applications |
| Vagrant | Automation | Provisionnement VM via scripts |

---

## 4️⃣ Gestion et bonnes pratiques

- Allouer suffisamment de ressources (CPU/RAM/disque) à chaque VM.  
- Utiliser des snapshots avant toute modification critique.  
- Documenter la configuration réseau et IP des VM.  
- Séparer les environnements de test et production.  
- Sauvegarder régulièrement les fichiers de VM (VMDK, VDI, VHD).  

---

## 5️⃣ Réseau dans la virtualisation

- **NAT** : VM partage l’IP de l’hôte pour accéder à internet.  
- **Bridged** : VM sur le même réseau que l’hôte, visible par les autres machines.  
- **Host-only** : VM isolée du réseau externe, communique uniquement avec l’hôte.  
- **Internal** : VM communique uniquement avec d’autres VM sur le même hyperviseur.  

---

## 6️⃣ Liens utiles

- [VirtualBox Documentation](https://www.virtualbox.org/manual/UserManual.html)  
- [VMware Docs](https://www.vmware.com/support/pubs/)  
- [Hyper-V Microsoft Docs](https://learn.microsoft.com/en-us/virtualization/hyper-v-on-windows/)  

---

✍️ *Ce fichier fait partie du repo TSSR_Lab et fournit un aperçu pratique de la virtualisation pour un technicien systèmes et réseaux.*
