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
  * [Comparison](#comparison-bash-vs-zsh)
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
### About Zsh

#### Zsh Introduction

Like Bash, Zsh is a powerful interactive command interpreter. It is used in Unix and Linux environments and offers a smooth and efficient experience thanks to its many advanced features.  
It is highly appreciated by developers and system administrators as it allows fast navigation and extensive terminal customization.

#### Zsh Strong Points

* **Smart Auto-completion** 🎯  
  ➝ Dynamic suggestions for commands and options.

* **Auto-correction** 🔍  
  ➝ Detects and corrects typos by suggesting the correct command.

* **Advanced Customization** 🎨  
  ➝ Themes and plugins via **Oh My Zsh** for an optimized and stylish terminal.

* **Enhanced Command History Management** 📜  
  ➝ Quick search for previous commands and removal of duplicates.

* **Ultra-fast Navigation** 🚀  
  ➝ **z** plugin for instant access to the most frequently used directories.

* **Powerful Aliases and Shortcuts** ⚡  
  ➝ Create short commands to speed up task execution.

* **Bash Compatibility** 🔄  
  ➝ Runs existing Bash scripts without issues.

* **Separated `$PATH` Management** 📁  
  ➝ `$PATH` is handled as an array (`$path`), making it easier to manage.

#### Zsh Weak Points

* **Higher Resource Consumption** 🖥️  
  ➝ More memory-intensive than Bash, especially with **Oh My Zsh** and multiple plugins enabled.

* **Longer Startup Time** ⏳  
  ➝ Can slow down on launch if too many heavy plugins or themes are loaded.

* **Imperfect Compatibility with Some Scripts** ⚠️  
  ➝ Some scripts specifically written for Bash may require adjustments.

* **More Complex Configuration** 🔧  
  ➝ Requires more customization to fully take advantage of its features.

* **Dependency on Oh My Zsh for Beginners** 🏗️  
  ➝ Many popular features require additional frameworks.

* **Less Native Support on Some Systems** 📦  
  ➝ Not installed by default on all Linux distributions and macOS (requires manual installation).

* **Longer Learning Curve for Beginners** 📘  
  ➝ Many advanced options and commands can be overwhelming at first.

* **Potential Conflicts with Bash** 🔄  
  ➝ Can cause errors if some Bash configurations are incompatible with Zsh.

* **Less Online Documentation and Support than Bash** 🌐  
  ➝ Most tutorials and online solutions are geared towards Bash.

### Comparison: Bash vs Zsh  

Bash and Zsh are two of the most popular **command interpreters** on Unix and Linux.  
Both allow users to exe### About Zsh

#### Zsh Introduction

Like Bash, Zsh is a powerful interactive command interpreter. It is used in Unix and Linux environments and offers a smooth and efficient experience thanks to its many advanced features.  
It is highly appreciated by developers and system administrators as it allows fast navigation and extensive terminal customization.

#### Zsh Strong Points

* **Smart Auto-completion** 🎯  
  ➝ Dynamic suggestions for commands and options.

* **Auto-correction** 🔍  
  ➝ Detects and corrects typos by suggesting the correct command.

* **Advanced Customization** 🎨  
  ➝ Themes and plugins via **Oh My Zsh** for an optimized and stylish terminal.

* **Enhanced Command History Management** 📜  
  ➝ Quick search for previous commands and removal of duplicates.

* **Ultra-fast Navigation** 🚀  
  ➝ **z** plugin for instant access to the most frequently used directories.

* **Powerful Aliases and Shortcuts** ⚡  
  ➝ Create short commands to speed up task execution.

* **Bash Compatibility** 🔄  
  ➝ Runs existing Bash scripts without issues.

* **Separated `$PATH` Management** 📁  
  ➝ `$PATH` is handled as an array (`$path`), making it easier to manage.

#### Zsh Weak Points

* **Higher Resource Consumption** 🖥️  
  ➝ More memory-intensive than Bash, especially with **Oh My Zsh** and multiple plugins enabled.

* **Longer Startup Time** ⏳  
  ➝ Can slow down on launch if too many heavy plugins or themes are loaded.

* **Imperfect Compatibility with Some Scripts** ⚠️  
  ➝ Some scripts specifically written for Bash may require adjustments.

* **More Complex Configuration** 🔧  
  ➝ Requires more customization to fully take advantage of its features.

* **Dependency on Oh My Zsh for Beginners** 🏗️  
  ➝ Many popular features require additional frameworks.

* **Less Native Support on Some Systems** 📦  
  ➝ Not installed by default on all Linux distributions and macOS (requires manual installation).

* **Longer Learning Curve for Beginners** 📘  
  ➝ Many advanced options and commands can be overwhelming at first.

* **Potential Conflicts with Bash** 🔄  
  ➝ Can cause errors if some Bash configurations are incompatible with Zsh.

* **Less Online Documentation and Support than Bash** 🌐  
  ➝ Most tutorials and online solutions are geared towards Bash.

### Comparison: Bash vs Zsh  

Bash and Zsh are two of the most popular **command interpreters** on Unix and Linux.  
Both allow users to execute commands, navigate files, and automate tasks through scripts.  
However, despite their shared foundations, their differences in **features, customization, and performance** can influence a user's choice.
cute commands, navigate files, and automate tasks through scripts.  
However, despite their shared foundations, their differences in **features, customization, and performance** can influence a user's choice.

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
| `cat <file>` | Display### About Zsh

#### Zsh Introduction

Like Bash, Zsh is a powerful interactive command interpreter. It is used in Unix and Linux environments and offers a smooth and efficient experience thanks to its many advanced features.  
It is highly appreciated by developers and system administrators as it allows fast navigation and extensive terminal customization.

#### Zsh Strong Points

* **Smart Auto-completion** 🎯  
  ➝ Dynamic suggestions for commands and options.

* **Auto-correction** 🔍  
  ➝ Detects and corrects typos by suggesting the correct command.

* **Advanced Customization** 🎨  
  ➝ Themes and plugins via **Oh My Zsh** for an optimized and stylish terminal.

* **Enhanced Command History Management** 📜  
  ➝ Quick search for previous commands and removal of duplicates.

* **Ultra-fast Navigation** 🚀  
  ➝ **z** plugin for instant access to the most frequently used directories.

* **Powerful Aliases and Shortcuts** ⚡  
  ➝ Create short commands to speed up task execution.

* **Bash Compatibility** 🔄  
  ➝ Runs existing Bash scripts without issues.

* **Separated `$PATH` Management** 📁  
  ➝ `$PATH` is handled as an array (`$path`), making it easier to manage.

#### Zsh Weak Points

* **Higher Resource Consumption** 🖥️  
  ➝ More memory-intensive than Bash, especially with **Oh My Zsh** and multiple plugins enabled.

* **Longer Startup Time** ⏳  
  ➝ Can slow down on launch if too many heavy plugins or themes are loaded.

* **Imperfect Compatibility with Some Scripts** ⚠️  
  ➝ Some scripts specifically written for Bash may require adjustments.

* **More Complex Configuration** 🔧  
  ➝ Requires more customization to fully take advantage of its features.

* **Dependency on Oh My Zsh for Beginners** 🏗️  
  ➝ Many popular features require additional frameworks.

* **Less Native Support on Some Systems** 📦  
  ➝ Not installed by default on all Linux distributions and macOS (requires manual installation).

* **Longer Learning Curve for Beginners** 📘  
  ➝ Many advanced options and commands can be overwhelming at first.

* **Potential Conflicts with Bash** 🔄  
  ➝ Can cause errors if some Bash configurations are incompatible with Zsh.

* **Less Online Documentation and Support than Bash** 🌐  
  ➝ Most tutorials and online solutions are geared towards Bash.

### Comparison: Bash vs Zsh  

Bash and Zsh are two of the most popular **command interpreters** on Unix and Linux.  
Both allow users to execute commands, navigate files, and automate tasks through scripts.  
However, despite their shared foundations, their differences in **features, customization, and performance** can influence a user's choice.
s file content |
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

#### **Editing**  

| **Shortcut** | **Description** |
| --- | --- |
| `i` | Insert mode (before the cursor). |
| `a` | Insert mode (after the cursor). |
| `o` | Add a new line below the current one and enter insert mode. |
| `O` | Add a new line above the current one and enter insert mode. |
| `x` | Delete the character under the cursor. |
| `dd` | Delete the current line. |
| `d$` | Delete from the cursor to the end of the line. |
| `d^` | Delete from the cursor to the beginning of the line. |
| `u` | Undo the last change. |
| `Ctrl + r` | Redo an undone change. |
| `p` | Paste after the cursor. |
| `P` | Paste before the cursor. |

#### **Copy, Cut, and Paste**  

| **Shortcut** | **Description** |
| --- | --- |
| `yy` | Copy the current line. |
| `Y` | Copy from the cursor to the end of the line. |
| `yw` | Copy the current word. |
| `p` | Paste after the cursor. |
| `P` | Paste before the cursor. |
| `d` + movement (e.g., `dw`) | Cut the specified text. |

#### **File Management**  

| **Shortcut** | **Description** |
| --- | --- |
| `:w` | Save the file. |
| `:q` | Quit Vim. |
| `:wq` or `ZZ` | Save and quit. |
| `:q!` | Quit without saving. |
| `:e filename` | Open a file. |
| `:n` | Switch to the next file (if multiple files are open). |
| `:!command` | Execute a shell command (e.g., `:!ls`). |

#### **Window Management**  

| **Shortcut** | **Description** |
| --- | --- |
| `:split` or `:sp` | Split the window horizontally. |
| `:vsplit` or `:vsp` | Split the window vertically. |
| `Ctrl + w + h` | Move to the window on the left. |
| `Ctrl + w + l` | Move to the window on the right. |
| `Ctrl + w + j` | Move to the window below. |
| `Ctrl + w + k` | Move to the window above. |
| `:close` | Close the current window. |

## **Nano**  

<img src="img/nanonew.jpg" alt="Structure du travail" width="100" align='center'>

### **Nano Shortcuts**  

| **Shortcut** | **Function** |
|---|---|
| `Ctrl + G` | Display Nano's help menu. |
| `Ctrl + X` | Exit the editor (with confirmation if modifications were made). |
| `Ctrl + O` | Save the file without exiting. |
| `Ctrl + R` | Insert a file into the current text. |
| `Ctrl + W` | Search for a word or phrase in the file. |
| `Ctrl + K` | Cut the current line. |
| `Ctrl + U` | Paste the last cut line. |
| `Ctrl + J` | Justify the paragraph (align text). |
| `Ctrl + T` | Check spelling (if a spell checker is installed). |
| `Ctrl + C` | Show the cursor’s current line and column number. |
| `Ctrl + _` | Move to a specific line and column. |
| `Alt + U` | Undo the last action. |
| `Alt + E` | Redo the undone action. |
| `Alt + 6` | Copy the current line. |
| `Alt + V` | Scroll up the screen. |
| `Alt + ]` | Move to the next closing parenthesis `)` or `]`. |
| `Alt + [` | Move to the previous opening parenthesis `(` or `[`. |

## Bash vs Zsh

### About Bash

#### Bash (Bourne Again Shell) Introduction

Bash is a command interpreter mainly used on Unix and Linux systems. It is an improved version of the original Bourne shell (sh) and is now one of the most popular shells in the Unix/Linux environment. It allows users to execute commands in the command line, automate processes via scripts, and interact efficiently with the operating system.

#### Bash Strong Points

* **Scripting** ✍️  
  ➝ Bash enables the creation of complex scripts thanks to control structures and its great flexibility. It also allows the automation of repetitive tasks and workflow optimization.

* **Portability** 🌍  
  ➝ Bash scripts are portable across multiple Linux and Unix distributions. This makes it easier to create universal solutions for developers and system administrators.

* **Command Memory** 🧠  
  ➝ Bash has features that enable command auto-completion, saving time and reducing typing errors. Additionally, it keeps a history of previous commands, allowing users to reuse them easily.

* **Process Management** ⚙️  
  ➝ Bash provides the ability to manage background processes (interrupt, suspend, or redirect them), offering better flexibility.

#### Bash Weak Points

* **Script Complexity** 😕  
  ➝ While using command lines is relatively simple for beginners, understanding script syntax and error handling can be challenging to master.

* **Lack of a Graphical Interface** 🖥️❌  
  ➝ Bash is primarily command-line oriented and lacks graphical interfaces.

* **Modern Applications** 📱💻  
  ➝ Although it excels at managing files and processes, Bash is limited when it comes to running or managing modern applications that require richer or more specific environments, such as graphical interfaces.

### About Zsh

#### Zsh Introduction

Like Bash, Zsh is a powerful interactive command interpreter. It is used in Unix and Linux environments and offers a smooth and efficient experience thanks to its many advanced features.  
It is highly appreciated by developers and system administrators as it allows fast navigation and extensive terminal customization.

#### Zsh Strong Points

* **Smart Auto-completion** 🎯  
  ➝ Dynamic suggestions for commands and options.

* **Auto-correction** 🔍  
  ➝ Detects and corrects typos by suggesting the correct command.

* **Advanced Customization** 🎨  
  ➝ Themes and plugins via **Oh My Zsh** for an optimized and stylish terminal.

* **Enhanced Command History Management** 📜  
  ➝ Quick search for previous commands and removal of duplicates.

* **Ultra-fast Navigation** 🚀  
  ➝ **z** plugin for instant access to the most frequently used directories.

* **Powerful Aliases and Shortcuts** ⚡  
  ➝ Create short commands to speed up task execution.

* **Bash Compatibility** 🔄  
  ➝ Runs existing Bash scripts without issues.

* **Separated `$PATH` Management** 📁  
  ➝ `$PATH` is handled as an array (`$path`), making it easier to manage.

#### Zsh Weak Points

* **Higher Resource Consumption** 🖥️  
  ➝ More memory-intensive than Bash, especially with **Oh My Zsh** and multiple plugins enabled.

* **Longer Startup Time** ⏳  
  ➝ Can slow down on launch if too many heavy plugins or themes are loaded.

* **Imperfect Compatibility with Some Scripts** ⚠️  
  ➝ Some scripts specifically written for Bash may require adjustments.

* **More Complex Configuration** 🔧  
  ➝ Requires more customization to fully take advantage of its features.

* **Dependency on Oh My Zsh for Beginners** 🏗️  
  ➝ Many popular features require additional frameworks.

* **Less Native Support on Some Systems** 📦  
  ➝ Not installed by default on all Linux distributions and macOS (requires manual installation).

* **Longer Learning Curve for Beginners** 📘  
  ➝ Many advanced options and commands can be overwhelming at first.

* **Potential Conflicts with Bash** 🔄  
  ➝ Can cause errors if some Bash configurations are incompatible with Zsh.

* **Less Online Documentation and Support than Bash** 🌐  
  ➝ Most tutorials and online solutions are geared towards Bash.

### Comparison: Bash vs Zsh  

Bash and Zsh are two of the most popular **command interpreters** on Unix and Linux.  
Both allow users to execute commands, navigate files, and automate tasks through scripts.  
However, despite their shared foundations, their differences in **features, customization, and performance** can influence a user's choice.

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
