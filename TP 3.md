## Wassim MEYYAH - 3ICS

# 1. Commandes de base

### 1 - 
Pour mettre à jour le système, on utilise d'abord la commande ```apt update``` puis ```apt upgrade```

### 2 - 
Pour créer un alias permanent, il faut se rendre dans le fichier ```~/.bashrc``` et y définir un nouvel alias ```alias maj='sudo apt update ; sudo apt upgrade'```. Il faut ensuite forcer le redémarrage de Ubuntu afin de rendre les modifications effectives à l'aide de la commande ```source ~/.bashrc```. L'alias est désormais mis en ligne.

### 3 - 
Pour obtenir les 5 derniers paquets  installés par la machine, on utilise la commande ```tail -5 /var/log/dpkg.log'

### 4 -


### 5 - 
Pour compter les paquets installés, on peut utiliser ```dpkg --list | wc -l``` : on obtient un nombre de 611 paquets. On peut aussi compter les paquets en utilisant ```apt list --installed | wc -l```, on en compte 607. Cette différence s'explique par des lignes de texte ajoutées au début du fichier dpkg. 

### 6 - 
Pour déterminer combien de paquets sont disponibles en téléchargement sur les dépôts Ubuntu, on utilise la commande ```apt list | wc -l```. On voit qu'il y en a 68744 
