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


