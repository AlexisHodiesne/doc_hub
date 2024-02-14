## GIT

Définir le nom d'utilisateur : ```git config --global user.name "nom"```
Définir le mail : ```git config --global user.email "you@example.com"```
Afficher le graphique de l'état des branches : ```git log --graph```
Mettre à jour les branches par rapport au remote : ```git fetch --all --prune```
Changer de branche : ```git switch <branche>```
Appliquer les mises à jour de la branche remote vers la locale : ```git pull```
Remettre la branche locale au même niveau que la remote :```git reset --hard origin/<branche>```
Modifier un commit : ```git commit --amend --no-edit```
Ajouter un commit rattaché au précédent : ```git commit --amend```
Supprimer une branche locale : ```git branch -d <branche>```
Supprimer une branche remote : ```git push origin -d <branche>```
Ignore chmod changes : ```git config core.filemode false```

## LINUX ( TODO )
chmod 777 'fichier'			: Droits 
man (-k) *sujet*			: Doc
pwd							: Chemin
sudo *commande*				: commande root
su *user*					: Se connecter
ls (-l)						: Lister répertoire
touch *nom*					: Créer fichier
mkdir						: Créer dossier
cat							: Lire fichier
rm							: Supprimer
grep						: Chercher 
alias						: Créer des alias 
cp *fichier* *path/nom*		: Copier

update-alternatives --config php  	: Choisir version PHP
composer self-update --1/2 			: Changer version composer

# WSL 

- Installation : ```wsl --install -d <DistroName>```
- Lister les distribs disponibles : ```wsl -l -o```
- Vérifier les distribs et leur version installée : ```wsl -l -v```
- Changer la version : ```wsl --set-version <DistroName> <versionNumber>```
- Changer la distribution : ```wsl --set-version <DistroName>```
- Demarrage : ```wsl```
- Arrêt : ```wsl --shutdown```
- Ouvrir VScode : ```code .```

# Docker
Lister les instances : ```docker ps```										
Monter le conteneur : ```docker-compose up|down -d (--build)```
Démarrer / stopper le conteneur : ```docker start|stop```								
Rentrer dans le conteneur : ```docker exec -it *name* bash```						
Status de docker : ```sudo service docker status```						
Éxecuter un fichier sql sur un BDD donnée : ```<driver> -u<user> -p<password> <database_name> < chemin_vers_fichier/fichier.sql```  

