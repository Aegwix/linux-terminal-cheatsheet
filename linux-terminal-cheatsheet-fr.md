# Linux Terminal Cheatsheet - FR

## Présentation du terminal
Un **terminal** est un outil qui permet d'interagir avec un système d'exploitation via des commandes textuelles, plutôt qu'à travers une interface graphique.
Processus global lorsque vous tapez une commande:
* __Saisie de la commande :__ Vous entrez une commande textuelle qui donne des instructions au système.
* __Traitement :__ Le shell interprète cette commande et exécute les actions correspondantes (comme copier un fichier, afficher une liste de dossiers, etc.).
* __Affichage du résultat :__ Le terminal retourne la réponse (ou un message d’erreur) basée sur la commande exécutée.
![Structure du travail](https://www.linuxtricks.fr/upload/terminal-shell-prompt-commande.png)


__Utilisation des commandes dans le Terminal:__  
     1.Commencez par ouvrir le terminal.  
     2.Taper des commandes.  
     3.Réponses visibles.  

## Table des matières

## ⌨ Raccourcis

### Terminal

### Bash

### Zsh

| **Raccourci**  | **Description** |
|---------------|----------------|
| `Ctrl + A`   | Aller au **début** de la ligne |
| `Ctrl + E`   | Aller à la **fin** de la ligne |
| `Alt + F`    | Aller au **mot suivant** |
| `Alt + B`    | Aller au **mot précédent** |
| `Ctrl + U`   | **Supprimer** tout avant le curseur |
| `Ctrl + K`   | **Supprimer** tout après le curseur |
| `Ctrl + W`   | Supprimer le **mot précédent** |
| `↑ (Flèche Haut)`  | Revenir à la **commande précédente** |
| `↓ (Flèche Bas)`   | Aller à la **commande suivante** |
| `!!`        | Exécuter la **dernière commande** |


### Vim

### Nano

## Commandes

### Terminal

### Bash

### Zsh

### Vim

### Nano

## Bash vs Zsh

### Bash

#### Introduction à Bash (Bourne Again Shell)

Bash est un interpréteur de commandes utilisé principalement sur les systèmes Unix et Linux. C'est une version améliorée du shell Bourne original (sh) et est désormais l'un des shells les plus populaires dans l'environnement Unix/Linux. Il permet aux utilisateurs d'exécuter des commandes en ligne de commande, d'automatiser des processus via des scripts, et d'interagir efficacement avec le système d'exploitation.

#### Points forts de Bash

- **Les scripts** ✍️  
  ➝ Bash permet la création de scripts complexes grâce à des structures de contrôle et à sa grande flexibilité. Il permet aussi d'automatiser les tâches répétitives et d'optimiser le flux de travail.

- **La portabilité** 🌍  
  ➝ Les scripts de Bash sont portables vers plusieurs distributions Linux et Unix. Cela permet de faciliter la création de solutions universelles pour les développeurs et administrateurs système.

- **Mémoire des commandes** 🧠  
  ➝ Bash possède des fonctionnalités permettant de compléter automatiquement les commandes, ce qui permet à la fois de gagner du temps et d'éviter les erreurs de saisie. De plus, il garde un historique des commandes précédentes, permettant de les réutiliser.

- **Gestion des processus** ⚙️  
  ➝ Bash offre la possibilité de gérer les processus d'arrière-plan (les interrompre, les suspendre ou les rediriger), offrant ainsi une meilleure flexibilité.


#### Points faibles de Bash

- **Complexité des scripts** 😕  
  ➝ Si l'utilisation des lignes de commande est assez simple pour les débutants, la compréhension de la syntaxe des scripts et la gestion des erreurs sont assez difficiles à maîtriser pour les débutants.

- **Manque d'interface graphique** 🖥️❌  
  ➝ Bash est principalement axé sur les lignes de commande et manque cruellement d'interfaces graphiques.

- **Les applications modernes** 📱💻  
  ➝ Bien qu'il soit performant pour la gestion des fichiers et des processus, il est cependant limité lorsqu'il s'agit d'exécuter ou de gérer les applications modernes nécessitant des environnements plus riches ou spécifiques, comme les interfaces graphiques par exemple.

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

### ⚔️ Comparaison : Bash vs Zsh  

Bash et Zsh sont deux des **interpréteurs de commandes** les plus populaires sous Unix et Linux.  
Ils permettent tous deux d’exécuter des commandes, de naviguer dans les fichiers et d’automatiser des tâches via des scripts.  
Cependant, bien qu’ils partagent des bases communes, leurs différences en termes de **fonctionnalités, personnalisation et performances** peuvent influencer le choix de l’utilisateur.  

#### 🛠️ **Fonctionnalités principales**  

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

#### 🎯 **Verdict argumenté**  

Le choix entre **Bash et Zsh** dépend essentiellement des **besoins et préférences de l’utilisateur**.  

- **Si l’objectif est la compatibilité maximale et la simplicité**, Bash est suffisant. Il est **déjà installé** sur la plupart des systèmes et bénéficie d’une **documentation extrêmement riche**.  
- **Si l’on recherche une expérience plus moderne, interactive et ergonomique**, Zsh est une alternative plus attrayante.  
- **Dans un contexte professionnel**, Zsh peut offrir un **gain de productivité** non négligeable grâce à son **autocomplétion avancée, sa gestion optimisée de l’historique et ses plugins**.  

Cependant, bien que Zsh offre plus de fonctionnalités, **il demande une configuration initiale** pour en tirer pleinement parti. Pour un utilisateur occasionnel, cette personnalisation peut **ne pas être nécessaire**.  

Dans l’ensemble, **Zsh est un excellent choix pour ceux qui passent beaucoup de temps dans le terminal**, tandis que Bash reste une valeur sûre pour son **universalité et sa simplicité d’utilisation**.  

## Installation

| Outils | Debian/Ubuntu <br>(`apt`) | Arch Linux <br>(`pacman`) | Documentation | 
| ------ | --- | --- | --- |
| **Bash** | `sudo apt install bash` | `sudo pacman -S bash` | [Documentation Bash](https://www.gnu.org/doc/doc.html) |
| **Zsh** | `sudo apt install zsh` | `sudo pacman -S zsh` | [Documentation Zsh](https://zsh.sourceforge.io/Doc/) |
| **Vim** | `sudo apt install vim` | `sudo pacman -S vim` | [Documentation Vim](https://vimdoc.sourceforge.net/) |
| **Nano** | `sudo apt install nano` | `sudo pacman -S nano` | [Documentation Nano](https://www.nano-editor.org/docs.php) |

Une fois l'installation terminée, vous pourrez désormais utiliser les commandes et raccourcis situés plus haut.

### Configuration

#### Bash and Zsh

Pour modifier et configurer votre shell, vous pouvez utiliser la commande `chsh` afin de choisir le chemin vers le shell à utiliser.

Vous pouvez également prompter `chsh -s <ins>PATH_AU_SHELL</ins>` afin d'insérer directement le cheminn vers le bon shell.

Une fois cela fait, il faut se déconnecter et reconnecter. En ouvrant votre terminal, le changement devrait être effectif. Pour en être sûr et certain, utiliser `echo $SHELL` afin de vérifier l'utilisation du bon shell.

Par exemple, pour zsh:

1. Utiliser `chsh -s /bin/zsh`
2. Se déconnecter et se reconnecter

Ceci changera le shell par défaut pour cet utilisateur à zsh.

#### Vim and Nano

**Configuring Vim**

Vim uses a special file called `.vimrc` (found in your home directory) to store settings.

**Steps to Configure Vim:**

1. **Open the configuration file:**

   ```zsh
   nano ~/.vimrc
   ```

2. **Add some basic settings:** (Copy & paste these)

   ```zsh
   set number          " Show line numbers
   syntax on           " Enable syntax highlighting
   set autoindent      " Auto-indent new lines
   set tabstop=4       " Set tab width to 4 spaces
   set shiftwidth=4    " Set indentation width to 4 spaces
   ```

3. **Save and exit in Nano:**  
   - Press `CTRL + X`, then `Y`, then `Enter`.

4. **Test Vim:**  
   Open Vim by typing:

   ```zsh
   vim testfile.txt
   ```

   Your settings should now be active!

**Configuring Nano**

Nano uses a configuration file called `.nanorc`.

**Steps to Configure Nano:**

1. **Open the configuration file:**

   ```zsh
   nano ~/.nanorc
   ```

2. **Add some useful settings:**

   ```zsh
   set linenumbers    # Show line numbers
   set tabsize 4      # Set tab width to 4 spaces
   set mouse          # Enable mouse support
   ```

3. **Save and exit in Nano:**  
   - Press `CTRL + X`, then `Y`, then `Enter`.

4. **Test Nano:**  
   Open a file in Nano to see if the changes work:

   ```zsh
   nano testfile.txt
   ```
