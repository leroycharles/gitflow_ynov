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
