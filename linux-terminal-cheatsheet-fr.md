# Linux Terminal Cheatsheet - FR

## Présentation du terminal

## Table des matières

## Raccourcis

### Terminal

### Bash

### Zsh

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

### Zsh

### Comparaison

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
