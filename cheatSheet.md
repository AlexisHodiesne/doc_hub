# CheatSheet des commandes
## GIT

- ```git config --global user.name "nom"``` : Définir le nom d'utilisateur
- ```git config --global user.email "you@example.com"``` : Définir le mail
- ```git config --global pull.rebase true``` : Activer le rebase automatique au pull
- ```git log --graph``` : Afficher le graphique de l'état des branches
- ```git fetch --all --prune``` : Mettre à jour les branches par rapport au remote
- ```git fetch --prune && git branch -vv | grep ': gone]' | awk '{print $1}' | xargs git branch -d``` : Supprimer les branches locales supprimées de remote
- ```git switch <branche>``` : Changer de branche
- ```git pull``` : Appliquer les mises à jour de la branche remote vers la locale
- ```git reset --hard origin/<branche>``` : Remettre la branche locale au même niveau que la remote
- ```git commit --amend --no-edit``` : Modifier un commit
- ```git commit --amend``` : Ajouter un commit rattaché au précédent
- ```git branch -d <branche>``` : Supprimer une branche locale
- ```git push origin -d <branche>``` : Supprimer une branche remote
- ```git config core.filemode false``` : Ignore chmod changes

## LINUX
### Global
- ```chmod <777>``` : Droits (User - Groupe - Other)
  | **Valeur** | Droits | **Valeur** | Droits      | **Valeur** | Droits       | **Valeur** | Droits       |
  | ---------- | ------ | ---------- | ----------- | ---------- | ------------ | ---------- | ------------ |
  | **0**      | Aucun  | **1**      | Exec        | **2**      | Write        | **3**      | Write + Exec |
  | **4**      | Read   | **5**      | Read + Exec | **6**      | Read + Write | **7**      | Tous         |
- ```man (-k) <sujet>``` : Doc
- ```pwd```	Chemin
- ```sudo <commande>```	commande root
- ```su <user>``` : Se connecter
- ```ls (-l)```	Lister répertoire
- ```touch <nom>```	Créer fichier
- ```mkdir``` : Créer dossier
- ```cat```	Lire fichier
- ```rm (-rf)``` : Supprimer
- ```grep``` : Chercher
- ```alias``` : Créer un alias
- ```cp <fichier> <path/newFichier>``` : Dupliquer
- ```mv <path> <destination_path>``` : Déplacer / renommer
- ```diff <path_1> <path_2>``` : Comparer
- ````ls -l > fichier``` : Rediriger la sortie vers un fichier
- ````ls -l >> fichier``` : Rediriger la sortie vers un fichier après son contenu
- ````ls -l fichierInexistant 2> fichier``` : Rediriger l'erreur vers un fichier

### Spécifique
- ```lsb_release -a``` : Informations sur la distribution linux
- ```update-alternatives --config php``` : Choisir version PHP
- ```composer self-update --<version>``` : Changer version composer

## WSL 

- ```wsl --install -d <DistroName>``` : Installation
- ```wsl -l -o``` : Lister les distribs disponibles
- ```wsl -l -v``` : Vérifier les distribs et leur version installée
- ```wsl --set-version <DistroName> <versionNumber>``` : Changer la version
- ```wsl --set-version <DistroName>``` : Changer la distribution
- ```wsl``` : Demarrage
- ```wsl --shutdown``` : Arrêt
- ```code .``` : Ouvrir VScode

## Docker
- ```docker ps``` : Lister les instances
- ```docker-compose up|down -d (--build)``` : Monter le conteneur
- ```docker start|stop``` : Démarrer / stopper le conteneur
- ```docker exec -it name bash``` : Rentrer dans le conteneur
- ```sudo service docker status``` : Status de docker 
- ```<driver> -u<user> -p<password> <database_name> < chemin_vers_fichier/fichier.sql``` :  Éxecuter un fichier sql sur un BDD donnée

