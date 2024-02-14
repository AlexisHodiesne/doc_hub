# Guide de mise en place du WSL avec Docker

Lien vers la documentation officielle : https://learn.microsoft.com/fr-fr/windows/wsl/install

## WSL

### Installation

Ouvrir un CMD en Admin.
_Recommandation : utiliser la version LTS la plus récente_

- Installation : ```wsl --install``` / ```wsl --install -d <DistroName>```
- Lister les distribs : ```wsl -l -o```
- Lister la version du wsl : ```wsl -l -v```
- Passer en v2 : ```wsl --set-version <DistroName> 2```
- Lancement du wsl : ````wsl```


### Conseils, compléments et bonnes pratiques 

- Utiliser le Terminal windows et configurer une fenêtre Ubuntu 
- Instancier les projets dans ``/home/<utilisateur>``
- Montrer la branche actuelle : ``/home/<utilisateur>`` .bashrc (créer si nécessaire) 
```
if [ "$color_prompt" = yes ]; then
    PS1='${debian_chroot:+($debian_chroot)}\[\033[01;32m\]\u@\h\[\033[00m\]:\[\033[01;34m\]\w\[\033[01;31m\]$(__git_ps1 " (%s)")\[\033[00m\]$ '`
```