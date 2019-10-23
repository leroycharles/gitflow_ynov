# Les branches
## Gestion des branches 
Lors de l'initialisation du repo, la branche "master" est automatiquement créer par:
> $ git init

Pour créer une branche on utilise la commande:
> $ git branch branche

Pour afficher toutes les branches on utilise:
> $ git branch

On supprime une branche avec la commande:
> $ git branch -d branche

On force la suppression d'une branche avec la commande:
> $ git branch -D branche

Pour basculer sur une branche on utilise la commande:
> $ git checkout branche

Pour créer une branche et basculer dessus en une seule ligne de commande:
> $ git checkout -b branche

Il est possible de fusionner une branche dans la branche actuelle via la commande:
> $ git merge branche

Il est possible de faire un commit de merge même si les 2 branches ne divergent pas:
> $ git merge branche --no-ff

On peut lister les branches non mergées avec la commande:
> $ git branch --no-merged

## Le remisage
Pour remiser le code qui n'est pas commiter:
> $ git stash

Pour lister les stashs sur la brache courante on utilise la commande:
> $ git stash list

Pour récupérer une stash on utilise la commande:
> $ git stash apply

Pour supprimer une stash on utilise la commande:
> $ git stash drop

