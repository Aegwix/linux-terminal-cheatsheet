# Linux Terminal Cheatsheet - FR

## Présentation du terminal
Un **terminal** est un outil qui permet d'interagir avec un système d'exploitation via des commandes textuelles, plutôt qu'à travers une interface graphique.
Processus global lorsque vous tapez une commande:
* __Saisie de la commande :__ Vous entrez une commande textuelle qui donne des instructions au système.
* __Traitement :__ Le shell interprète cette commande et exécute les actions correspondantes (comme copier un fichier, afficher une liste de dossiers, etc.).
* __Affichage du résultat :__ Le terminal retourne la réponse (ou un message d’erreur) basée sur la commande exécutée.

<img src=https://www.linuxtricks.fr/upload/terminal-shell-prompt-commande.png alt="Structure du travail" allign="left" width="400">  

__Utilisation des commandes dans le Terminal:__  
     1.Commencez par ouvrir le terminal.  
     2.Taper des commandes.  
     3.Réponses visibles.  

## Table des matières

## Raccourcis

### Terminal

### Bash

### Zsh

### Vim

#### Édition

| Raccourcis | Description |
| --- | --- |
|`i`| Mode insertion (avant le curseur).|
|`a`| Mode insertion (après le curseur).|
|`o`|Ajouter une nouvelle ligne sous celle en cours et entrer en mode insertion.|
|`0`|Ajouter une nouvelle ligne au-dessus de celle en cours et entrer en mode insertion.|
|`x`| Supprimer le caractère sous le curseur.|
|`dd`|Supprimer la ligne courante.|
|`d$`| Supprimer du curseur jusqu’à| la fin de la ligne.|
|`d^`|Supprimer du curseur jusqu’au début de la ligne.|
|`u`| Annuler la dernière modification.|
|`Ctrl + r`| Refaire une modification annulée.|
|`p`| Coller après le curseur.|
|`P`| Coller avant le curseur.|

#### Copier, couper et coller

| Raccourcis | Description |
| --- | --- |
|`yy`| Copier la ligne courante.|
|`Y`| Copier du curseur jusqu’à la fin de la ligne.|
|`yw`|Copier le mot courant.|
|`p`| Coller après le curseur.|
|`P`| Coller avant le curseur.|
|`d`+ mouvement (ex. `dw`)| Couper le texte spécifié.|

#### Gestion des fichiers

| Raccourcis | Description |
| --- | --- |
|`:w`| Sauvegarder le fichier.|
|`:q`| Quitter Vim.|
|`:wq` ou `ZZ`| Sauvegarder et quitter.|
|`:q!`| Quitter sans sauvegarder.|
|`:e nom_fichier`| Ouvrir un fichier.|
|`:n`| Passer au fichier suivant (si plusieurs fichiers sont ouverts)|.
|`:!commande`|Exécuter une commande shell (ex. :!ls).|

#### Gestion des fenêtres

| Raccourcis | Description |
| --- | --- |
|`:split` ou `:sp`| - Diviser la fenêtre horizontalement.|
|`:vsplit` ou `:vsp`| Diviser la fenêtre verticalement.|
|`Ctrl + w + h`| Aller à la fenêtre à gauche.|
|`Ctrl + w + l`| Aller à la fenêtre à droite.|
|`Ctrl + w + j`| Aller à la fenêtre en dessous.|
|`Ctrl + w + k`| Aller à la fenêtre au-dessus.|
|`:close`| Fermer la fenêtre en cours.|

### Nano

## Commandes

### Terminal

### Bash

### Zsh

### Vim

### Nano

## Bash vs Zsh

### Bash

### Zsh


#### Introduction à Zsh

Zsh est un interpréteur de commandes interactif et puissant utilisé dans les environnements Unix et Linux. Il offre une expérience fluide et efficace grâce à ses nombreuses fonctionnalités avancées. 
Très apprécié des développeurs et administrateurs systèmes, il permet une navigation rapide et une personnalisation poussée du terminal.

#### 🔹 Les points forts de Zsh

- **Autocomplétion intelligente** 🎯  
  ➝ Suggestions dynamiques pour les commandes et options.

- **Correction automatique** 🔍  
  ➝ Détecte et corrige les fautes de frappe en proposant la bonne commande.

- **Personnalisation avancée** 🎨  
  ➝ Thèmes et plugins via **Oh My Zsh** pour un terminal optimisé et stylé.

- **Gestion améliorée de l’historique** 📜  
  ➝ Recherche rapide des commandes précédentes et suppression des doublons. 

- **Navigation ultra-rapide** 🚀  
  ➝ Plugin **z** pour accéder instantanément aux dossiers les plus utilisés.

- **Alias et raccourcis puissants** ⚡  
  ➝ Création de commandes courtes pour accélérer l’exécution des tâches.

- **Compatibilité avec Bash** 🔄  
  ➝ Exécute sans problème les scripts Bash existants.

- **Séparation des chemins `$PATH`** 📁  
  ➝ `$PATH` est géré sous forme de tableau (`$path`), ce qui facilite la gestion.

#### 🔻 Les points faibles de Zsh

- **Consommation de ressources plus élevée** 🖥️  
  ➝ Plus gourmand en mémoire que Bash, surtout avec **Oh My Zsh** et plusieurs plugins activés.  

- **Temps de démarrage plus long** ⏳  
  ➝ Peut ralentir au lancement si trop de plugins ou thèmes lourds sont chargés.  

- **Compatibilité imparfaite avec certains scripts** ⚠️  
  ➝ Certains scripts écrits spécifiquement pour Bash peuvent nécessiter des ajustements.  

- **Configuration plus complexe** 🔧  
  ➝ Nécessite plus de personnalisation pour en tirer pleinement parti.  

- **Dépendance à Oh My Zsh pour les débutants** 🏗️  
  ➝ Beaucoup de fonctionnalités populaires nécessitent des frameworks supplémentaires.  

- **Moins de support natif sur certains systèmes** 📦  
  ➝ Pas installé par défaut sur toutes les distributions Linux et macOS (nécessite une installation manuelle).  

- **Apprentissage plus long pour les débutants** 📘  
  ➝ De nombreuses options et commandes avancées peuvent être déroutantes au début.  

- **Risque de conflits avec Bash** 🔄  
  ➝ Peut entraîner des erreurs si certaines configurations Bash sont incompatibles avec Zsh.  

- **Moins de documentation et de support en ligne que Bash** 🌐  
  ➝ La majorité des tutoriels et solutions en ligne sont orientés vers Bash.  


### Comparaison

## Installation

### Bash

### Zsh

### Vim

### Nano