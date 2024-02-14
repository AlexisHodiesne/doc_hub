# Guide de mise en place du WSL avec Docker

## WSL
Lien vers la documentation officielle : https://learn.microsoft.com/fr-fr/windows/wsl/install

### Installation

_Recommandation : utiliser la version LTS la plus récente_
_Vous retrouverez les commandes basiques dans la cheatSheet.md pour vous aider et pour aller plus loin_

1. Ouvrir une invite de commande (CMD / powershell / ...) en Admin.
2. Installer le wsl : ```wsl --install```  
3. Vérifier la distribution et sa version : ```wsl -l -v```
4. Lancer le wsl : ```wsl```

### Conseils, compléments et bonnes pratiques 

- Il est recommandé d'utiliser l'application "terminal" de Windows. Vous pourrez y démarrer automatiquement une fenêtre de WSL
- Instancier les projets dans ``/home/<utilisateur>``
- Montrer la branche actuelle : ``nano /home/<utilisateur>/.bashrc``  
Coller à la fin : 
```
# Show branch
if [ "$color_prompt" = yes ]; then
        PS1='${debian_chroot:+($debian_chroot)}\[\033[01;32m\]\u@\h\[\033[00m\]:\[\033[01;34m\]\$(`git branch --show-current 2>/dev/null`)\[\033[00m\]\$ '
else
        PS1='${debian_chroot:+($debian_chroot)}\u@\h:\w\$(`git branch --show-current 2>/dev/null`)\$ '
fi

parse_git_branch() {
   git branch 2> /dev/null | sed -e '/^[^*]/d' -e 's/* \(.*\)/ (\1)/'
}
PS1='${debian_chroot:+($debian_chroot)}\[\033[01;32m\]\u@\h\[\033[00m\]:\[\033[01;34m\]\w\[\033[00m\]\[\033[33m\]$(parse_git_branch)\[\033[00m\]\$ '
```

## Docker (To do)
### Installation