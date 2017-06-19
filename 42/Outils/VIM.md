# VIM
VIM est un éditeur de texte en ligne de commande.

## JE SUIS PERDU !!!
* Pour **sortir de VIM** sans sauvegarder :

    `ÉCHAP` (retourne dans le mode commande) puis tapez `:q!`

* Pour **sortir et sauvegarder** le document :

    `ÉCHAP` puis tapez `:wq!`

* Pour **insérer du texte** :
    
    rentrer dans le mode insertion avec la touche `i` puis écrire. Pour sortir du mode insertion appuyez sur `ÉCHAP`

## Installation

* Sur Ubuntu & Debian

    `$ apt install vim`

## Utilisation
Attention, il existe une différence entre les les lettres majuscules et minuscules !

### Les modes
Il existe différents modes dans VIM :

* **mode normale**

C'est le mode par défaut lors du démarrage du logiciel. 

> Pour retourner sur ce mode : appuyez sur `ÉCHAP`

* **mode commande**

il permet de réaliser les commandes VIM, comme par exemple enregistrer le document ou quitter le logiciel.

> En `mode normale` appuyez sur la touche `:` et ensuite tapez votre commande.

* **mode insertion**

C'est le mode pour insérer du texte dans votre document.

> En `mode commande` appuyez sur la touche `i`.

Il existe un mode remplacement (remplace les caractères existants par les nouveaux) avec `R`.

* **mode visuel**

Permet de sélectionner du texte. Les commandes exécutaient agissent sur l'ensemble du texte sélectionné.

> En `mode commande` appuyez sur  `v`

Il existe d'autres modes similaires : le mode visuel par ligne avec `V` & le mode visuel par bloc `Ctrl` + `V`.

### Quelques raccourcies
Les parenthèses indique le mode à utiliser pour exécuter le raccourcie

* Supprimer le caractère à droite
> `x`

* Supprimer (et copier) une ligne entière
> `dd`

* Coller
> `p`

#### Rechercher
* Rechercher
> `/` puis ce que vous rechercher, *ex: `/recherche`*

* Ensuite, afficher les résultats suivants
> `n`

* Et afficher les résultats précédents
> `N`

#### Copier/collé
* Copier et supprimer une ligne entière
> `dd`

* Copier (en mode visuel)
> `y`

* Copier ligne entière
> `yy`

* Coller après le curseur
> `p`

* Coller avant le curseur
> `P`

#### Annuler/refaire
* Annuler
> `u`

* Refaire
> `CTRL` + `r`

#### Quelques triks

- Variante d'insertion de texte :
  - insertion basique
  > `i`
  - insertion à la ligne suivante
  > `o` *(lettre o minuscule)*
  - insertion à la ligne précédente
  > `O` *(lettre o majuscule)*
  - supprimer le mot pour ensuite écrire
  > `cw`

- Déplacement avancé
  - aller à la première colonne
  > `0` *(zéro)*
  - aller au premier caractère de la ligne
  > `^`
  - aller à la fin de la ligne
  > `$`
  - aller au dernier caractère de la ligne
  > `g_`
  - aller à la prochaine occurrence *i*
  > `f`*i*
  - l'inverse de la commande ci-dessus
  > `F`*i*
  - aller à la *n*ième occurence de *i*
  > *n*`f`*i*
  - aller à la première ligne
  > `gg` ou `1G`
  - aller à la dernière ligne
  > `G`
  - aller à la ligne *N*
  > *N*`G`

- Indentation de texte
> `CTRL`+`V` et sélectionner le texte à indenter
  - pour indenter manuellement
  > `<` pour indenter à gauche et `>` pour indenter à droite
  - pour indenté automatiquement
  > `=`

### Gérer plusieurs écrans

- diviser l'écran horizontalement
> `:split`

> `CTRL` + `W` puis `s`

- diviser l'écran verticalement
> `:vsplit`

> `CTRL` + `W` puis `v`

- fermer l'écran courant
> `CTRL` + `W` puis `q`

- fermer tous les écrans sauf le courant
> `CTRL` + `W` puis `o`
 
- se déplacer dans les différents écrans
> `CTRL` + `W` ensuite `HAUT`/`BAS`/`GAUCHE`/`DROITE`

- gérer la taille de l'écran
> `CTRL` + `W` puis `<` pour aller à gauche et `>` pour aller à droite

> `CTRL` + `W` puis `-` pour descendre et `+` pour monter

### Quelques commandes
Les commandes peuvent s'additionner.

* Sauvegarder 
> `:w`

* Sauvegarder (si nécessaire) et quitter 
> `:x`

* Sauvegarder et quitter 
> `:wq`

* Quitter & quitter sans sauvegarder
> `:q` & `:q!`

### Quelques exemples

- Ajouter des commentaires sur plusieurs lignes
  - `CTRL`+`V` au premier caractère à la première ligne
  - sélectionner les lignes avec les flèches directionnels ou les raccourcies
  - `I` (i majuscule)
  - insérer les commentaires (exemple : *//*)
  - `ECHAP`

