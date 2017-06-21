# GIT
GIT est un gestionniaire de fichier, qui permet de sauvegarder des états de fichiers ainsi que de travailler de manière collaborative.


# Quelques infos

- **HEAD**
C'est un nom symbolique qui représente le commit le plus récent dans une branche, généralement là où on a lancé la commande `git checkout unEndroit`.


# Quelques commandes

## Modifier les états

- Faire une sauvegarde (commit)
> `git commit -m "Court desciptif du changement"`

- Créer une branche
> `git branch nouvelleBranche`

- Se positionner quelque part dans l'arboréscence de git, souvent pour aller dans une autre branche
> `git checkout nouvelleBranche`

- Fusionner deux branches entre elles
  1. Se positionner dans la branche qui survivra avec `git checkout`
  2. Puis `git merge brancheSecondaire`

- ou avec `git rebase laBranche`


## Commits relatifs

- Revenir d'un commit en arrière
> `^`

- Revenir de plusieurs commit en arrière
> `~10` pour revenir à *10* commits en arrière.


## Revenir en arrière

- Supprime le dernier commit en supprimant définitivement les commits
> `git reset HEAD^`

- Supprime le dernier commit en ajoutant un commit qui décrit la suppréssion des fichiers (le commit supprimé est toujours disponible)
> `git revert HEAD`

# Autres

git branch nomBranche -f uneReference
 
