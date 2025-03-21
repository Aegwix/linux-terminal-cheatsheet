# Linux Terminal Cheatsheet - En

## About the terminal

A **terminal** is a tool which allows users to interact directly with their operating systems through text prompts, rather than a graphic interface.

Here's how it usually works:

* **Inserting the prompt:** You write down a valid command that gives instructions to your system.
* **Processing:** The shell tries to understand the command and execute the corresponding action (copy a file, display a list of directories, etc.)
* **Displays results:** The terminal displays an appropriate response (or error message), according to the command.

<img src="https://www.linuxtricks.fr/upload/terminal-shell-prompt-commande.png" alt="Structure du travail" width="400" align='center'>  

**Use terminal commands:**  
     1. Open the terminal.  
     2. Write out the prompts.  
     3. See the results.  

## Table of content

* [About the terminal](#about-the-terminal)
* [Table of content](#table-of-content)
* [Terminal](#terminal)
  * [Terminal Shorcuts](#terminal-shortcuts)
  * [Terminal Commands](#terminal-commands)
* [Bash](#bash)
  * [Bash Shortcuts](#bash-shortcuts)
  * [Bash Commands](#bash-commands)
* [Zsh](#zsh)
  * [Zsh Shortcuts](#zsh-shortcuts)
  * [Zsh Commmands](#zsh-commands)
* [Vim](#vim)
  * [Vim Shortcuts](#vim-shortcuts)
* [Nano](#nano)
  * [Nano Shortcuts](#nano-shortcuts)
* [Bash vs Zsh](#bash-vs-zsh)
  * [Bash](#about-bash)
    * [Introduction](#bash-bourne-again-shell-introduction)
    * [Strong Points](#bash-strong-points)
    * [Weak Points](#bash-weak-points)
  * [Zsh](#about-zsh)
    * [Introduction](#zsh-introduction)
    * [Strong Points](#zsh-strong-points)
    * [Weak Points](#zsh-weak-points)
  * [Comparison](#comparison--bash-vs-zsh)
    * [Main functions](#main-functions)
    * [Final Verdict](#final-verdict)
* [Installation](#installation)
* [Configuration](#configuration)
  * [Bash and Zsh](#bash-and-zsh)
  * [Vim and Nano](#vim-and-nano)
    * [Configuration Vim](#configuring-vim)
    * [Configuration Nano](#configuring-nano)

## Terminal

 <img src="img/Untitled.jpeg" alt="Structure du travail" width="100" align='center'> 

### Terminal Shortcuts

#### 📌 Basic Control

| Shortcut | Description |
|-----------|-------------|
| `Ctrl + C` | Stops the current process |
| `Ctrl + Z` | Suspends the current process |
| `Ctrl + D` | Closes the terminal |
| `Ctrl + L` | Clears the terminal screen (equivalent to `clear`) |

#### 🕵️ Command Navigation

| Shortcut | Description |
|-----------|-------------|
| `Ctrl + A` | Moves the cursor to the beginning of the line |
| `Ctrl + E` | Moves the cursor to the end of the line |
| `Ctrl + U` | Deletes everything before the cursor |
| `Ctrl + K` | Deletes everything after the cursor |
| `Ctrl + W` | Deletes the word before the cursor |
| `Alt + B` | Moves the cursor back one word |
| `Alt + F` | Moves the cursor forward one word |

#### 🔄 Command History

| Shortcut | Description |
|-----------|-------------|
| `Ctrl + R` | Searches a command in the interactive history |
| `↑` / `↓` | Navigates through command history |
| `!n` | Executes command number `n` from the history |
| `!!` | Re-executes the last command |
| `!string` | Executes the last command containing `string` |

#### 📂 Managing Terminal Windows

| Shortcut | Description |
|-----------|-------------|
| `Ctrl + Shift + T` | Opens a new tab in the terminal |
| `Ctrl + Shift + W` | Closes the current tab |
| `Ctrl + Shift + N` | Opens a new terminal window |
| `Ctrl + PageUp/PageDown` | Switches between tabs |

#### 📑 Other Useful Tips

| Shortcut | Description |
|-----------|-------------|
| `Tab` | Auto-completes the command |
| `Ctrl + Shift + C` | Copies selected text |
| `Ctrl + Shift + V` | Pastes copied text |
| `Alt + .` | Repeats the last argument of the previous command |

### Terminal Commands

#### 📂 Files and Directories

| Command | Description |
|----------|-------------|
| `ls` | Lists files |
| `cd <directory>` | Changes directory |
| `pwd` | Displays the current directory |
| `mkdir <name>` | Creates a directory |
| `rm -r <name>` | Deletes a file/directory |
| `cp <source> <dest>` | Copies a file/directory |
| `mv <source> <dest>` | Moves or renames a file/directory |

#### 📜 Viewing and Editing Files

| Command | Description |
|----------|-------------|
| `cat <file>` | Displays file content |
| `less <file>` | Paged reading |

#### 🔍 Searching

| Command | Description |
|----------|-------------|
| `find <directory> -name <name>` | Searches for a file |
| `grep <word> <file>` | Searches for a word in a file |

#### 📡 Network

| Command | Description |
|----------|-------------|
| `ping <address>` | Checks connection |
| `wget <URL>` | Downloads a file |
| `curl <URL>` | Retrieves a web page |

#### 🛑 System

| Command | Description |
|----------|-------------|
| `shutdown -h now` | Shuts down the system |
| `reboot` | Reboots the system |
| `df -h` | Shows available disk space |
| `free -h` | Displays used memory |

#### 📦 Package Management (Ubuntu/Debian)

| Command | Description |
|----------|-------------|
| `sudo apt update && apt upgrade` | Updates the system |
| `sudo apt install <package>` | Installs a software package |
| `sudo apt remove <package>` | Uninstalls a software package |

## Bash

<img src="img/Bash.png" alt="Structure du travail" width="100" align='center'> 

### Bash Shortcuts

| Shortcut | Function |
|------------|-------------------------|
| `Ctrl + R` | Search for a command in the history in real time (reverse search) |
| `Ctrl + G` | Exit history search (`Ctrl + R`) without executing a command |
| `Ctrl + O` | Execute the command found via `Ctrl + R` without removing it from history |
| `Ctrl + X + E` | Open the default text editor to modify the current command |
| `Ctrl + X + Ctrl + E` | Same function as `Ctrl + X + E` (compatible with more environments) |
| `Ctrl + T` | Swap the order of the last two typed characters |
| `Alt + .` | Retrieve the last argument of the previous command (equivalent to ` !$`) |
| `Alt + *` | Expand a file pattern (`*.txt` becomes all `.txt` files) |
| `Alt + U` | Convert the word under the cursor to uppercase |
| `Alt + L` | Convert the word under the cursor to lowercase |
| `Alt + C` | Capitalize the first letter of the word under the cursor |
| `Alt + T` | Swap the order of the last two typed words |
| `Alt + D` | Delete the word after the cursor |
| `Alt + Backspace` | Delete the word before the cursor |

### Bash Commands

| Command | Function |
|---|---|
| `alias <alias_name>='<command>'` | Create an alias for a command |
| `unalias <alias_name>` | Remove an alias |
| `history` | Show the history of previous commands |
| `!!` | Re-run the last command |
| `!<num>` | Execute the command corresponding to number `<num>` in history |
| `export <variable>=<value>` | Create an environment variable (shared between processes) |
| `source <file>` | Execute a script in the current shell without opening a new process |
| `printf "<format>"` | Display formatted text (more powerful than `echo`) |
| `set` | Display or set environment variables or shell options |
| `declare` | Declare variables with attributes (e.g., `-a` for arrays) |
| `exec <command>` | Replace the current process with another one without creating a new shell |
| `test <condition>` | Evaluate a condition (e.g., string comparison, files) |

## Zsh

<img src="img/Zsh.png" alt="Structure du travail" width="100" align='center'>

### Zsh Shortcuts

| Shortcut  | Description |
|---------------|----------------|
| `Ctrl + A`   | Go to the **beginning** of the line |
| `Ctrl + E`   | Go to the **end** of the line |
| `Alt + F`    | Move forward one **word** |
| `Alt + B`    | Move backward one **word** |
| `Ctrl + U`   | **Delete** everything before the cursor |
| `Ctrl + K`   | **Delete** everything after the cursor |
| `Ctrl + W`   | Delete the **previous word** |
| `↑ (Up Arrow)`  | Go back to the **previous command** |
| `↓ (Down Arrow)`   | Move to the **next command** |
| `!!`        | Execute the **last command** |

### Zsh Commands

| Command  | Description |
|--------------|----------------|
| `echo "text"`  | Display text on the screen |
| `cd`  | Change directory |
| `pwd`  | Show the current directory |
| `ls`  | List files and directories |
| `mkdir <folder_name>`  | Create a new directory |
| `rmdir <folder_name>`  | Remove an empty directory |
| `rm <file_name>`  | Delete a file |
| `rm -r <folder_name>`  | Delete a folder and its contents |
| `cp <file_name> <destination>`  | Copy a file |
| `mv <file_name> <destination>`  | Move or rename a file |
| `touch <file_name>`  | Create an empty file |
| `cat <file_name>`  | Display the contents of a file |
| `nano <file_name>`  | Edit a file with Nano |

## Vim

<img src="img/VIM.png" alt="Structure du travail" width="100" align='center'>

### Vim Shortcuts

#### Édition

| Raccourcis | Description |
| --- | --- |
|`i`| Mode insertion (avant le curseur).|
|`a`| Mode insertion (après le curseur).|
|`o`|Ajouter une nouvelle ligne sous celle en cours et entrer en mode insertion.|
|`0`|Ajouter une nouvelle ligne au-dessus de celle en cours et entrer en mode insertion.|
|`x`| Supprimer le caractère sous le curseur.|
|`dd`|Supprimer la ligne courante.|
|`d$`| Supprimer du curseur jusqu’à la fin de la ligne.|
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
|`:n`| Passer au fichier suivant (si plusieurs fichiers sont ouverts)|
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

## Nano
 
 <img src="img/nanonew.jpg" alt="Structure du travail" width="100" align='center'>

### Nano Shortcuts

| Raccourci | Fonction |
|---|---|
| `Ctrl + G` | Affiche l'aide de Nano |
| `Ctrl + X` | Quitte l'éditeur (avec confirmation si des modifications ont été faites) |
| `Ctrl + O` | Sauvegarde le fichier sans quitter |
| `Ctrl + R` | Insère un fichier dans le texte en cours |
| `Ctrl + W` | Recherche un mot ou une phrase dans le fichier |
| `Ctrl + K` | Coupe la ligne courante |
| `Ctrl + U` | Colle la dernière ligne coupée |
| `Ctrl + J` | Justifie le paragraphe (alignement du texte) |
| `Ctrl + T` | Vérifie l'orthographe (si un correcteur est installé) |
| `Ctrl + C` | Affiche le numéro de ligne et de colonne du curseur |
| `Ctrl + _` | Se déplace vers une ligne et une colonne spécifiques |
| `Alt + U` | Annule la dernière action |
| `Alt + E` | Refait l’action annulée |
| `Alt + 6` | Copie la ligne courante |
| `Alt + V` | Permet de faire défiler l'écran vers le haut |
| `Alt + ]` | Se déplace vers la prochaine parenthèse fermante `)` ou `]` |
| `Alt + [` | Se déplace vers la parenthèse ouvrante précédente `(` ou `[` |

## Bash vs Zsh

### About Bash

#### Bash (Bourne Again Shell) Introduction

Bash est un interpréteur de commandes utilisé principalement sur les systèmes Unix et Linux. C'est une version améliorée du shell Bourne original (sh) et est désormais l'un des shells les plus populaires dans l'environnement Unix/Linux. Il permet aux utilisateurs d'exécuter des commandes en ligne de commande, d'automatiser des processus via des scripts, et d'interagir efficacement avec le système d'exploitation.

#### Bash Strong Points

* **Les scripts** ✍️  
  ➝ Bash permet la création de scripts complexes grâce à des structures de contrôle et à sa grande flexibilité. Il permet aussi d'automatiser les tâches répétitives et d'optimiser le flux de travail.

* **La portabilité** 🌍  
  ➝ Les scripts de Bash sont portables vers plusieurs distributions Linux et Unix. Cela permet de faciliter la création de solutions universelles pour les développeurs et administrateurs système.

* **Mémoire des commandes** 🧠  
  ➝ Bash possède des fonctionnalités permettant de compléter automatiquement les commandes, ce qui permet à la fois de gagner du temps et d'éviter les erreurs de saisie. De plus, il garde un historique des commandes précédentes, permettant de les réutiliser.

* **Gestion des processus** ⚙️  
  ➝ Bash offre la possibilité de gérer les processus d'arrière-plan (les interrompre, les suspendre ou les rediriger), offrant ainsi une meilleure flexibilité.

#### Bash Weak Points

* **Complexité des scripts** 😕  
  ➝ Si l'utilisation des lignes de commande est assez simple pour les débutants, la compréhension de la syntaxe des scripts et la gestion des erreurs sont assez difficiles à maîtriser pour les débutants.

* **Manque d'interface graphique** 🖥️❌  
  ➝ Bash est principalement axé sur les lignes de commande et manque cruellement d'interfaces graphiques.

* **Les applications modernes** 📱💻  
  ➝ Bien qu'il soit performant pour la gestion des fichiers et des processus, il est cependant limité lorsqu'il s'agit d'exécuter ou de gérer les applications modernes nécessitant des environnements plus riches ou spécifiques, comme les interfaces graphiques par exemple.

### About Zsh

#### Zsh Introduction

Zsh est comme Bsh un interpréteur de commandes interactif puissant. Il est utilisé dans les environnements Unix et Linux, et offre une expérience fluide et efficace grâce à ses nombreuses fonctionnalités avancées.
Il est un shell très apprécié des développeurs et administrateurs systèmes car il permet une navigation rapide et une personnalisation poussée du terminal.

#### Zsh Strong Points

* **Autocomplétion intelligente** 🎯  
  ➝ Suggestions dynamiques pour les commandes et options.

* **Correction automatique** 🔍  
  ➝ Détecte et corrige les fautes de frappe en proposant la bonne commande.

* **Personnalisation avancée** 🎨  
  ➝ Thèmes et plugins via **Oh My Zsh** pour un terminal optimisé et stylé.

* **Gestion améliorée de l’historique** 📜  
  ➝ Recherche rapide des commandes précédentes et suppression des doublons.

* **Navigation ultra-rapide** 🚀  
  ➝ Plugin **z** pour accéder instantanément aux dossiers les plus utilisés.

* **Alias et raccourcis puissants** ⚡  
  ➝ Création de commandes courtes pour accélérer l’exécution des tâches.

* **Compatibilité avec Bash** 🔄  
  ➝ Exécute sans problème les scripts Bash existants.

* **Séparation des chemins `$PATH`** 📁  
  ➝ `$PATH` est géré sous forme de tableau (`$path`), ce qui facilite la gestion.

#### Zsh Weak Points

* **Consommation de ressources plus élevée** 🖥️  
  ➝ Plus gourmand en mémoire que Bash, surtout avec **Oh My Zsh** et plusieurs plugins activés.  

* **Temps de démarrage plus long** ⏳  
  ➝ Peut ralentir au lancement si trop de plugins ou thèmes lourds sont chargés.  

* **Compatibilité imparfaite avec certains scripts** ⚠️  
  ➝ Certains scripts écrits spécifiquement pour Bash peuvent nécessiter des ajustements.  

* **Configuration plus complexe** 🔧  
  ➝ Nécessite plus de personnalisation pour en tirer pleinement parti.  

* **Dépendance à Oh My Zsh pour les débutants** 🏗️  
  ➝ Beaucoup de fonctionnalités populaires nécessitent des frameworks supplémentaires.  

* **Moins de support natif sur certains systèmes** 📦  
  ➝ Pas installé par défaut sur toutes les distributions Linux et macOS (nécessite une installation manuelle).  

* **Apprentissage plus long pour les débutants** 📘  
  ➝ De nombreuses options et commandes avancées peuvent être déroutantes au début.  

* **Risque de conflits avec Bash** 🔄  
  ➝ Peut entraîner des erreurs si certaines configurations Bash sont incompatibles avec Zsh.  

* **Moins de documentation et de support en ligne que Bash** 🌐  
  ➝ La majorité des tutoriels et solutions en ligne sont orientés vers Bash.  

### Comparison : Bash vs Zsh  

Bash et Zsh sont deux des **interpréteurs de commandes** les plus populaires sous Unix et Linux.  
Ils permettent tous deux d’exécuter des commandes, de naviguer dans les fichiers et d’automatiser des tâches via des scripts.  
Cependant, bien qu’ils partagent des bases communes, leurs différences en termes de **fonctionnalités, personnalisation et performances** peuvent influencer le choix de l’utilisateur.  

#### Main Functions

| Fonctionnalité          | Bash ✅ | Zsh ✅ |
|-------------------------|--------|--------|
| Autocomplétion          | Basique | Avancée (suggestions dynamiques) |
| Correction automatique  | ❌ Non  | ✅ Oui (corrige les fautes de frappe) |
| Personnalisation       | Limitée | Très avancée avec **Oh My Zsh** |
| Gestion de l’historique | Standard | ✅ Améliorée (suppression des doublons, partage entre sessions) |
| Navigation rapide       | ❌ Non | ✅ Oui (*plugin z*, **cd amélioré**) |
| Séparation `$PATH`      | ❌ Non | ✅ Oui (*géré en tableau*, facilite l’édition) |
| Scripts Bash            | ✅ Oui | ✅ Oui (*compatible avec Bash*) |
| Gestion des processus   | ✅ Oui | ✅ Oui |
| Installation par défaut | ✅ Oui (Linux/macOS) | ❌ Non (doit être installé manuellement) |

#### Final verdict

Le choix entre **Bash et Zsh** dépend essentiellement des **besoins et préférences de l’utilisateur**.  

* **Si l’objectif est la compatibilité maximale et la simplicité**, Bash est suffisant. Il est **déjà installé** sur la plupart des systèmes et bénéficie d’une **documentation importante**.  
* **Si l’on recherche une expérience plus moderne, interactive et ergonomique**, Zsh est une alternative plus intéréssante.  
* **Dans un contexte professionnel**, Zsh peut offrir un **gain de productivité** non négligeable grâce à son **autocomplétion avancée, sa gestion optimisée de l’historique et ses plugins**.  

Cependant, bien que Zsh offre plus de fonctionnalités, **il demande une configuration initiale** pour en tirer pleinement parti. Pour un utilisateur occasionnel, cette personnalisation peut **ne pas être nécessaire**.  

Dans l’ensemble, **Zsh est un excellent choix pour ceux qui passent beaucoup de temps dans le terminal**, tandis que Bash reste une valeur sûre pour **sa simplicité d’utilisation**.  

## Installation

| Outils | Debian/Ubuntu (`apt`) | Arch Linux  (`pacman`) | Documentation |
| ------ | --- | --- | --- |
| **Bash** | `sudo apt install bash` | `sudo pacman -S bash` | [Documentation Bash](https://www.gnu.org/doc/doc.html) |
| **Zsh** | `sudo apt install zsh` | `sudo pacman -S zsh` | [Documentation Zsh](https://zsh.sourceforge.io/Doc/) |
| **Vim** | `sudo apt install vim` | `sudo pacman -S vim` | [Documentation Vim](https://vimdoc.sourceforge.net/) |
| **Nano** | `sudo apt install nano` | `sudo pacman -S nano` | [Documentation Nano](https://www.nano-editor.org/docs.php) |

Une fois l'installation terminée, vous pourrez désormais utiliser les commandes et raccourcis situés plus haut.

## Configuration

### Bash and Zsh

Pour modifier et configurer votre shell, vous pouvez utiliser la commande `chsh` afin de choisir le chemin vers le shell à utiliser.

Vous pouvez également prompter `chsh -s <ins>PATH_AU_SHELL</ins>` afin d'insérer directement le chemin vers le bon shell.

Une fois cela fait, il faut redémarrer la session. En ouvrant votre terminal, le changement devrait être effectif. Pour en être sûr et certain, utiliser `echo $SHELL` afin de vérifier que vous utilisez le bon shell.

Par exemple, pour zsh:

1. Utiliser `chsh -s /bin/zsh`
2. Redémarrer la session

Ceci changera le shell par défaut pour cet utilisateur à zsh.

### Vim and Nano

#### Configuring Vim

Vim utilise un fichier spécifique appelé `.vimrc` (situé dans votre répertoire personnel) pour stocker les paramètres.

**Étapes pour configurer Vim :**

1. **Ouvrir le fichier de configuration :**

   ```zsh
   nano ~/.vimrc
   ```

2. **Ajouter quelques paramètres de base :** (Copiez-collez ces lignes)

   ```zsh
   set number          " Afficher les numéros de ligne
   syntax on           " Activer la coloration syntaxique
   set autoindent      " Auto-indent des nouvelles lignes
   set tabstop=4       " Définir la largeur des tabulations à 4 espaces
   set shiftwidth=4    " Définir la largeur d'indentation à 4 espaces
   ```

3. **Enregistrer et quitter Nano :**  
   * Appuyez sur ``CTRL + X``, puis ``Y``, puis ``Entrée``.

4. **Tester Vim :**  
   Ouvrez Vim en tapant :

   ```zsh
   vim testfile.txt
   ```

   Vos paramètres devraient maintenant être actifs !

#### Configuring Nano

Nano utilise un fichier de configuration appelé `.nanorc`.

**Étapes pour configurer Nano :**

1. **Ouvrir le fichier de configuration :**

   ```zsh
   nano ~/.nanorc
   ```

2. **Ajouter quelques paramètres utiles :**

   ```zsh
   set linenumbers    # Afficher les numéros de ligne
   set tabsize 4      # Définir la largeur des tabulations à 4 espaces
   set mouse          # Activer la prise en charge de la souris
   ```

3. **Enregistrer et quitter Nano :**  
   * Appuyez sur `CTRL + X`, puis `Y`, puis `Entrée`.

4. **Tester Nano :**  
   Ouvrez un fichier dans Nano pour voir si les modifications fonctionnent :

   ```zsh
   nano testfile.txt
   ```
