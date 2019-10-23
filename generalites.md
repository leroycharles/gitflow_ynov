# Généralités
## Configuration
Enregistrer vos informations "user" dans le .gitconfig:
> $ git config --global user.name Tony  
> $ git config --global user.email tony@tony.fr

Définir un éditeur pour écrire le texte du commit
> $ git config --system core.editor vim

Vous pouvez effectuez les même action sur un dépôt spécifique en vous plaçant dans se dépôt et en changeant "global" par "local".

## Zone de travail
Pour initialiser un dépôt on utilise la commande:
> $ git init

Pour obtenir le status d'un dépôt on utilise la commande:
> $ git status

Pour ajout un fichier à un dépôt on utilise la commande:
> $ git add fichier

Pour ajouter tous les fichiers à un dépôt on utilise la commande:
> $ git add .

Pour désindexer un fichier d'un dépôt on utilise la commande:
> $ git rm --cached fichier

Pour créer un commit avec un message dans un dépôt on utilise la commande:
> $ git commit -m "message"

Pour obtenir l'historique des commits d'un dépôt on utilise la commande:
> $ git log

## Configuration du .gitignore

Pour obtenir la liste des fichiers suivis dans un dépôt on utilise la commande:
> $ git ls-files

Remarques sur les patterns à utiliser pour exclure des fichiers :

	- doc/foo/ --> matchera avec doc/foo mais pas a/doc/foo
	- foo/ --> matchera avec a/foo et foo
	- foo/* --> matchera avec n'importe quel fichier autre qu'un "/"
	- *.txt --> ignore tous les fichiers qui ont cette extension dans le dépôt : racine, dossi
	- foo/*.txt --> ignore tous les fichiers de ce type dans les dossiers foo de l'application.
	- /*.txt --> ignore juste au niveau racine du dépôt.
	- **/foo --> ignore foo/a, bar/foo/a mais n'ignore pas foo/a/b
	- foo[0-9] --> ignore foo0, foo1, ... foo9
	- foo --> ignore a/foo, foo/a/b, a/b/foo, ...
	- foo/**/bar --> ignore foo/a/b/c/bar, foo/bar, ...

