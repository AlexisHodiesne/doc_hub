# CheatSheet des commandes
## GIT

- ```git config --global user.name "nom"``` : Définir le nom d'utilisateur
- ```git config --global user.email "you@example.com"``` : Définir le mail
- ```git log --graph``` : Afficher le graphique de l'état des branches
- ```git fetch --all --prune``` : Mettre à jour les branches par rapport au remote
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
- ``` lsb_release -a``` : Informations sur la distribution linux
- ```chmod <777> <fichier>``` : Droits
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
- ```mv``` : Déplacer

### Spécifique
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

