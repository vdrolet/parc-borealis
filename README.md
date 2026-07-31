# Parc Boréalis - C'est quoi
Parc simulant quelques serveurs vulnérables usuels pour le cours de cyber 3.
On s'en sert pour identifier des vulnérabilités.
> [!CAUTION]
> Ce parc contient des services ayant délibérément des vulnérabilités critiques. Ne surtout pas l'utiliser dans un environnement hors-classe !

# Utilisation
Pré-requis: une machine LINUX avec Docker d'installé.
1. Cloner le repo, ou télécharger les fichiers dans un dossier local.
2. Créer un fichier .env dans le dossier local, pour y mettre ces 2 variables :
```bash
# Fichier .env pour Docker parc Borealis
# Remplace {TON_ID_RÉSEAU_ÉTUDIANT} par le ID donné par le prof, ex. 
# STUDENT_ID=123
STUDENT_ID={TON_ID_RÉSEAU_ÉTUDIANT}
# Le nom de l'interface réseau utilisé pour la route par défaut (dépend de E1000, vmx3, etc.)
# Un "ip a" te donnera le nom de l'interface (ens133, ens192, eth0, etc.)
PARC_IFACE="ens192"
```
3. Puis lancer le parc avec :
```bash
docker compose build
docker compose up -d
```
