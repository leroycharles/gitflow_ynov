# Consultation de l’historique et des modifcations
## Utilisation de log
Pour consulter les 2 derniers commits, avec l'affichage sur une ligne:
> $ git log --oneline -2

Pour consulter les commits d’un auteur en particulier :
> $ git log --author "Antoine07"

Pour consulter l’historique à partir du premier jour:
> $ git log --since=1.day

Pour consulter l'historique d'avant une date précise:
> $ git log --before="2019-09-01"

Pour consulter l’historique d’un fichier uniquement :
> $ git log calzone.txt

Pour visualiser les modifications au sein d’un fichier ou de
l’ensemble/d’un ensemble des fichier(s) :
> $ git log -p calzone.txt
> $ git log -p
> $ git log -2 -p