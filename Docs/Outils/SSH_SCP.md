# 🔐 SSH & SCP – Guide complet

**SSH (Secure Shell) et SCP (Secure Copy)** sont essentiels pour la connexion et le transfert sécurisé de fichiers sur un réseau. Ce guide couvre installation, utilisation, astuces et bonnes pratiques.

## 1️⃣ SSH – Connexion sécurisée

**💻 Installation**

**Linux / Mac** : préinstallé (ssh)

**Windows** : installer via PuTTY ou OpenSSH

**Vérification** : ssh -V

**🔗 Connexion à un serveur**

ssh utilisateur@adresse_IP

Exemple : ssh loic@192.168.1.10

**🔑 Authentification par clé SSH**

**Générer la clé**: ssh-keygen -t rsa -b 4096 -C "mon_email@example.com"

**Copier la clé sur le serveur** : ssh-copy-id utilisateur@192.168.1.10

Connexion sans mot de passe possible après configuration

**💡 Astuces SSH**

**Vérifier les connexions actives** : who ou w

**Mode verbeux** : ssh -v utilisateur@192.168.1.10

**Transfert via SFTP** : sftp utilisateur@192.168.1.10


## 2️⃣ SCP – Transfert sécurisé de fichiers

**📤 Copier un fichier local vers le serveur**

scp fichier.txt utilisateur@192.168.1.10:/chemin/destination/

**📥 Copier un fichier du serveur vers la machine locale**

scp utilisateur@192.168.1.10:/chemin/fichier.txt /chemin/local/

**📂 Copier un dossier entier**

scp -r dossier utilisateur@192.168.1.10:/chemin/destination/

**💡 Astuces SCP**

**Utiliser un port non standard**: scp -P 2222 fichier.txt utilisateur@IP:/chemin/

**Mode verbeux** : scp -v fichier.txt utilisateur@IP:/chemin/

**Compression** : scp -C fichier.txt utilisateur@IP:/chemin/

## 3️⃣ Sécurité et bonnes pratiques

🔒 Toujours utiliser des **mots de passe forts ou clés SSH**

**❌ Éviter la connexion root directe**

🌐**Restreindre** l’accès par IP si possible

📝 Activer la journalisation pour audit des connexions

✅ Préférer SCP ou SFTP pour les transferts sécurisés

✍️ Ce guide est destiné aux étudiants TSSR pour gérer la connexion sécurisée et le transfert de fichiers dans leurs labs et environnements réseau.
