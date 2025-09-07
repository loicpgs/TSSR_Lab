# 💾 Sauvegardes – Bases pour TSSR

Ce document présente les concepts, méthodes et bonnes pratiques pour la sauvegarde des données dans un environnement IT.

---

## 1️⃣ Concepts clés

- **Backup** : copie de sécurité des données pour prévenir leur perte.  
- **Restore** : restauration des données à partir d’une sauvegarde.  
- **Full backup** : copie complète de toutes les données.  
- **Incremental backup** : copie uniquement des données modifiées depuis la dernière sauvegarde.  
- **Differential backup** : copie des données modifiées depuis la dernière sauvegarde complète.  
- **RPO (Recovery Point Objective)** : tolérance de perte de données (temps depuis le dernier backup).  
- **RTO (Recovery Time Objective)** : temps maximal pour restaurer les données après incident.  

---

## 2️⃣ Types de sauvegardes

| Type | Avantages | Inconvénients |
|------|-----------|---------------|
| Complète (Full) | Restauration rapide et complète | Temps et espace importants |
| Incrémentale | Sauvegarde rapide, moins d’espace | Restauration plus lente |
| Différentielle | Bon compromis | Nécessite la dernière full |

---

## 3️⃣ Méthodes et outils

- **Sauvegarde locale** : disque dur externe, NAS, serveur interne.  
- **Sauvegarde réseau** : serveur de fichiers centralisé, NAS.  
- **Sauvegarde cloud** : OneDrive, Google Drive, Azure Backup, AWS S3.  
- **Outils classiques** :
  - Windows : `Robocopy`, `wbadmin`  
  - Linux : `rsync`, `tar`, `cron` pour planification  
  - Solutions professionnelles : Veeam, Acronis, Bacula, Duplicati  

---

## 4️⃣ Bonnes pratiques

- Planifier des sauvegardes régulières (quotidiennes, hebdomadaires).  
- Tester régulièrement les restaurations pour s’assurer de la fiabilité.  
- Stocker les sauvegardes sur plusieurs sites si possible (local + cloud).  
- Chiffrer les sauvegardes pour sécurité et conformité.  
- Documenter les procédures et versions de sauvegarde.  

---

## 5️⃣ Liens utiles

- [Veeam Backup Docs](https://www.veeam.com/documentation-guides-datasheets.html)  
- [Microsoft Backup and Restore](https://learn.microsoft.com/en-us/windows-server/administration/windows-commands/wbadmin)  
- [rsync Linux Guide](https://linux.die.net/man/1/rsync)  

---

✍️ *Ce fichier fait partie du repo TSSR_Lab et fournit une référence pratique pour la sauvegarde et restauration des données.*
