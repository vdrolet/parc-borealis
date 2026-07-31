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
STUDENT_ID={utiliser le ID donné par le prof}
PARC_IFACE="ens192"
```
3. Puis lancer le parc avec :
```bash
docker compose up -d
```
