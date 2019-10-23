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

## Les tags
Pour créer un tag léger on utilise la commande:
> $ git tag v1

Pour créer un tag annoté on utilise la commande:
> $ git tag -a v1.0 -m "message"

On peut lister les tags via la commande:
> $ git tag

On peut voir un tag annoté via la commande:
> $ git show v1.0

On peut cherhcer un tag via la commande:
> $ git tag -l "v1.0"

## Introduciton aux branches distantes
On peut créer un serveur git à partir des commandes suivantes:
> $ mkdir repo.git
> $ cd repo.git
> $ git --bare init

On peut associer un repo local à un repo serveur via la commande:
> $ git remote add origin path_to_server
> $ git push origin master

On peut lister les repo distant via la commande:
> $ git remote

On peut récupérer les éléments d'un repo distant via la commande:
> $ git fetch origin
> $ git merge origin/master

Ce qui est l'aquivalent de la commande:
> $ git pull nom_distant branche

