# Les bases de Linux

## Définition
- Linux
> C'est un noyaux (kernel en anglais), qui peut être comparé avec un chef d'orchestre qui controle à la fois le materiel de l'ordinateur avec les logiciels exécuté par la distribution.
- Distribution
> C'est ensemble des logiciels qui 

## Le système de fichier de Linux (Filesystem)
La racine du système de fichier linux est représenté par `/`.

Il existe ensuite des dossiers, ainsi que des sous dossiers, sous sous dossiers, etc qui définisent l'ensemble des dossiers de la distribution linux. Chaques `/` sert à la séparation entre chaque dossiers.

Exemple : le chemin `/home/akipe/Documents/yolo.txt` dispose de 3 dossiers (les dossiers "home", le dossier enfant "akipe", le dossier sous enfant "Documents") avec à la fin le fichier "yolo.txt".

Voici la liste des quelques dossiers importants avec leurs utilité (attention, cela peut changer en fonction des distributions linux) : 

- `/boot`
C'est l'ensenble de fichiers nécéssaire pour le démarrage de la distribution linux.
- `/bin` 
Dossier qui rassemble l'ensemble des binaires/applications éxecutable par l'utilisateur.
- `/sbin`
Dossier similaire au dossier `/bin`, mais résérvé aux supers utilisateurs (s"udo"bin)
- `/var`
Dossier où sonht stocké l'ensemble des données des applications et l'ensemble des logs.
- `/dev`
Interraction avec les disques
- `/proc`
Tout ce qui concerne les processuces du système
- `/home`
Dossier qui rassemble les dossiers des utilisateurs
- `/lib` et `/lib64`
L'ensemble des librairies pour les applications.

TOUT est filesystem.
