<!-- TOC -->

- [Workshop Instructions](#workshop-instructions)
- [Workshop Abstract](#workshop-abstract)
- [Module 1 - A (re)introduction to the Shell](#module-1---a-reintroduction-to-the-shell)
  - [Navigation](#navigation)
    - [Working with Files](#working-with-files)
    - [Package Managers](#package-managers)
    - [History](#history)
    - [Multitasking](#multitasking)
- [Module 1 - Exercises](#module-1---exercises)
  - [Exercise 1: Navigating and Working with Files and Directories (Time: 4 minutes)](#exercise-1-navigating-and-working-with-files-and-directories-time-4-minutes)
    - [Bonus](#bonus)
  - [Exercise 2: Viewing Files and Using Package Manager (Time: 3 minutes)](#exercise-2-viewing-files-and-using-package-manager-time-3-minutes)
  - [Exercise 3: Using History and Multitasking (Time: 3 minutes)](#exercise-3-using-history-and-multitasking-time-3-minutes)
- [Module 2 - Enhancing Bash and Embracing Zsh](#module-2---enhancing-bash-and-embracing-zsh)
  - [Elevating the Bash Experience](#elevating-the-bash-experience)
    - [Installing New Commands](#installing-new-commands)
    - [Creating Aliases](#creating-aliases)
  - [Transitioning to Zsh with OhMyZsh](#transitioning-to-zsh-with-ohmyzsh)
    - [Setting Up Zsh](#setting-up-zsh)
    - [Implementing Themes](#implementing-themes)
  - [Enhancing Zsh with Plugins](#enhancing-zsh-with-plugins)
    - [Adding Useful Plugins](#adding-useful-plugins)
    - [Exploring Plugin Functionalities](#exploring-plugin-functionalities)
  - [Module 2 - Exercise 1 Enhancing Bash with Aliases and tf Command](#module-2---exercise-1-enhancing-bash-with-aliases-and-tf-command)
    - [1. Install the “tf” command](#1-install-the-tf-command)
  - [Module 2 - Exercise 2 - Setting up and Customizing oh-my-zsh](#module-2---exercise-2---setting-up-and-customizing-oh-my-zsh)
- [Module 3 - Quick Reference Guide: Composing Commands with Pipes and Redirects](#module-3---quick-reference-guide-composing-commands-with-pipes-and-redirects)
  - [Commands \& Concepts](#commands--concepts)
  - [Useful Combinations](#useful-combinations)
  - [Module 3 - Exercises: Composing Commands with Pipes and Redirects](#module-3---exercises-composing-commands-with-pipes-and-redirects)
    - [Exercise 1](#exercise-1)
      - [Task](#task)
        - [Steps](#steps)
    - [Exercise 2](#exercise-2)
      - [Task](#task-1)
        - [Steps](#steps-1)
    - [Exercise 3](#exercise-3)
      - [Task](#task-2)
        - [Steps](#steps-2)
    - [Exercise 4](#exercise-4)
      - [Task](#task-3)
        - [Steps](#steps-3)
    - [Exercise 5](#exercise-5)
      - [Task](#task-4)
        - [Steps](#steps-4)
    - [Additional Exercises](#additional-exercises)
      - [Exercise 6](#exercise-6)
      - [Task](#task-5)
        - [Steps](#steps-5)
    - [Exercise 7](#exercise-7)
      - [Task](#task-6)
        - [Steps](#steps-6)
    - [Exercise 8](#exercise-8)
      - [Task](#task-7)
        - [Steps](#steps-7)
- [Module 4 Reference Guide - Manipulating Files and Text](#module-4-reference-guide---manipulating-files-and-text)
  - [1. `find` - Locate Files and Directories](#1-find---locate-files-and-directories)
    - [Common Options:](#common-options)
    - [Examples:](#examples)
  - [2. `grep` - Search Text using Patterns](#2-grep---search-text-using-patterns)
    - [Common Options:](#common-options-1)
    - [Examples:](#examples-1)
  - [3. `sed` - Stream Editor](#3-sed---stream-editor)
    - [Common Options:](#common-options-2)
    - [Examples:](#examples-2)
  - [4. `xargs` - Build and Execute Command Lines from Standard Input](#4-xargs---build-and-execute-command-lines-from-standard-input)
    - [Common Options:](#common-options-3)
    - [Examples:](#examples-3)
  - [5. Logical Operators in the Shell](#5-logical-operators-in-the-shell)
    - [Examples:](#examples-4)
    - [Exercises:](#exercises)
  - [Vim Basic Guide - A Command-Line Text Editor](#vim-basic-guide---a-command-line-text-editor)
    - [1. Launching and Exiting Vim](#1-launching-and-exiting-vim)
      - [Commands:](#commands)
    - [2. Navigating Within Vim](#2-navigating-within-vim)
      - [Commands:](#commands-1)
    - [3. Editing Text](#3-editing-text)
      - [Modes:](#modes)
      - [Commands:](#commands-2)
    - [4. Searching and Replacing](#4-searching-and-replacing)
      - [Commands:](#commands-3)
    - [Tips](#tips)
  - [Summary](#summary)
- [Module 4 Exercises - Manipulating Files and Text](#module-4-exercises---manipulating-files-and-text)
- [Module 5 - Connecting to the world and Manipulating Data Quick Reference](#module-5---connecting-to-the-world-and-manipulating-data-quick-reference)
  - [curl](#curl)
    - [Common Commands and Flags:](#common-commands-and-flags)
    - [Example Usage:](#example-usage)
  - [jq](#jq)
    - [Common Commands and Flags:](#common-commands-and-flags-1)
  - [Example Usage:](#example-usage-1)
  - [A Useful Trick (HT Craig Walls \& Brian Sletten)](#a-useful-trick-ht-craig-walls--brian-sletten)

<!-- /TOC -->ons-1)
      - [Examples:](#examples-1)
    - [3. `sed` - Stream Editor](#3-sed---stream-editor)
      - [Common Options:](#common-options-2)
      - [Examples:](#examples-2)
    - [4. `xargs` - Build and Execute Command Lines from Standard Input](#4-xargs---build-and-execute-command-lines-from-standard-input)
      - [Common Options:](#common-options-3)
      - [Examples:](#examples-3)
    - [5. Logical Operators in the Shell](#5-logical-operators-in-the-shell)
      - [Examples:](#examples-4)
      - [Exercises:](#exercises)
    - [Vim Basic Guide - A Command-Line Text Editor](#vim-basic-guide---a-command-line-text-editor)
      - [1. Launching and Exiting Vim](#1-launching-and-exiting-vim)
        - [Commands:](#commands)
      - [2. Navigating Within Vim](#2-navigating-within-vim)
        - [Commands:](#commands-1)
      - [3. Editing Text](#3-editing-text)
        - [Modes:](#modes)
        - [Commands:](#commands-2)
      - [4. Searching and Replacing](#4-searching-and-replacing)
        - [Commands:](#commands-3)
      - [Tips](#tips)
    - [Summary](#summary)
  - [Module 4 Exercises - Manipulating Files and Text](#module-4-exercises---manipulating-files-and-text)
  - [Module 5 - Connecting to the world and Manipulating Data Quick Reference](#module-5---connecting-to-the-world-and-manipulating-data-quick-reference)
    - [curl](#curl)
      - [Common Commands and Flags:](#common-commands-and-flags)
      - [Example Usage:](#example-usage)
    - [jq](#jq)
      - [Common Commands and Flags:](#common-commands-and-flags-1)
    - [Example Usage:](#example-usage-1)
    - [A Useful Trick (HT Craig Walls \& Brian Sletten)](#a-useful-trick-ht-craig-walls--brian-sletten)

<!-- /TOC -->l - From Novice to Wizard

## Workshop Instructions

To get ready for this workshop, you’ll need a linux environment of some sort. Running this workshop in the container is recommended to keep all commands consistent and ensure no side-effects on your current machine.

Container Instructions
1. Install container runtime (docker, rancher, etc)
2. On Powershell or CMD, or Mac Terminal – execute the following command `docker pull carducci/wizard-workshop:latest`
3. Once the image downloads type the following: `docker run –it carducci/wizard-workshop`

Alternatively:

If you’re on a mac, open the terminal (note, your package manager and shell will be different)
If you’re on Windows, either open a terminal to the Linux Subsystem (note, your package manager and shell may be different depending on which distro you're using)

## Workshop Abstract

The Linux command line is powerful, but for those of us who weren't “borne” into that world, it can be a bit daunting. If the extent of your usage of the command line is limited to a handful of memorized git commands, npm cli, and the occasional copy and paste one-liner from the web, this session is for you.

## Module 1 - A (re)introduction to the Shell

Below is a summary of concepts taught in this module of the workshop.

### Navigation

- `~`: Represents the home directory
- `pwd`: Display the current working directory
- `ls`: List directory contents
  - `-a`: Show hidden files
  - `-l`: Show detailed listing
  - `-al`: Show detailed listing including hidden files
- `cd <directory>`: Change the current directory
- `cd ~`: Go back to the home directory
- `cd -`: Return to the previous directory
- `mkdir <directory_name>`: Create a new directory
- `touch <file_name>`: Create a new file or update timestamps

#### Working with Files

- `cp <source> <destination>`: Copy files or directories
- `mv <source> <destination>`: Move or rename files or directories
- `rm <file_name>`: Remove a file
  - `-r`: Remove directories recursively
- `rmdir <directory_name>`: Remove an empty directory
- `cat <file_name>`: Display file content
- `head <file_name>`: Display the beginning of a file
  - `-n <number>`: Specify the number of lines to display
- `tail <file_name>`: Display the end of a file
  - `-n <number>`: Specify the number of lines to display
- `clear`: Clear terminal screen
- `more <file_name>`: Scroll through file content
- `less <file_name>`: Scroll through file content with more functionality
- `man <command>`: Display the manual page for a command
- `echo <string>`: Print string to the terminal
  - `echo $PATH`: Display the PATH environment variable
- `printenv`: Display environment variables
- `whereis <command>`: Locate the binary, source, and manual page for a command

#### Package Managers

- `apt-get install <package_name>`: Install a package (Debian-based distributions)
  - Use `sudo` for elevated privileges
- `which <command>`: Check if a command is installed and show its location

#### History

- `history`: View command history
- `!!`: Repeat the last command
- `!<number>`: Execute a command from the history using its number

#### Multitasking

- `Ctrl-Z`: Send a running process to the background
- `fg`: Bring a background process to the foreground
- `fg %<job_number>`: Specify which background process to bring to the foreground
- `jobs`: List background processes

*Note: Replace `<placeholders>` with actual values when using the commands.*

## Module 1 - Exercises

### Exercise 1: Navigating and Working with Files and Directories (Time: 4 minutes)

1. Navigate to your home directory and use `pwd` to confirm your current directory. What is the output?

2. Create a new directory named `workshop_practice`. Then, navigate into this directory.

3. Inside `workshop_practice`, create four new files named `file1.txt`, `file2.txt`, `file3.txt`, and `file4.txt` using the `touch` command.

4. Use the `ls` command to list the files in `workshop_practice`. Now, use the `ls -l` command to view details of these files. What differences do you notice in the output of these two commands?

5. Use the `cp` command to copy `file1.txt` to a new file named `file1_copy.txt`.

6. Now, rename `file2.txt` to `file2_renamed.txt` using the `mv` command.

7. Remove `file3.txt` using the `rm` command.

8. Verify the changes made in steps 5, 6, and 7 by using the `ls -l` command.

#### Bonus

9. Use `mkdir` to create a subdirectory named `subdir1` inside `workshop_practice`.

10. Move `file4.txt` into `subdir1` using the `mv` command.

### Exercise 2: Viewing Files and Using Package Manager (Time: 3 minutes)

1. Navigate back to your home directory and use the `cat` command to view the contents of the `.bashrc` file (if available).

2. Use the `head` command to view the first 10 lines of the `.bashrc` file. Now, try viewing the first 5 lines.

3. Similarly, use the `tail` command to view the last 10 and then the last 5 lines of the `.bashrc` file.

4. Use the `less` command to open the `.bashrc` file and scroll up and down a few lines. Exit using `q`.

5. Check if the `nano` text editor is installed using the `which` command. If not, install it using the `apt-get install nano` command (use `sudo` if necessary).

### Exercise 3: Using History and Multitasking (Time: 3 minutes)

1. Execute the following commands sequentially:

```bash
echo "Hello World 1"
echo "Hello World 2"
echo "Hello World 3"
```

2. Use the `history` command to view the list of recently executed commands.

3. Use the double bang (`!!`) to repeat the last command.

4. Try bringing up previous commands using the up arrow key and execute any of them.

5. Pick a command from your history list and execute it using the `!number` syntax (replace `number` with the actual number of the command in the history list).

-----

## Module 2 - Enhancing Bash and Embracing Zsh

In this module, we delve deeper into the Linux shell environment, exploring the extensibility of bash and the advantages of using zsh with OhMyZsh. Below is a summary of the key concepts and commands introduced in this module.

### Elevating the Bash Experience

#### Installing New Commands
- `pip3 install thefuck --user`: Install 'thefuck' utility using pip.
- `export PATH=/home/wizard/.local/bin:$PATH`: Set the PATH to recognize the newly installed utility.
- `eval $(thefuck --alias drat)`: Create an alias `drat` to easily use 'thefuck' utility.
- `source ~/.bashrc`: Re-run the bash configuration file to apply the new changes.

#### Creating Aliases
- `nano ~/.bashrc`: Open the bash configuration file to add custom aliases.
- `alias restartbash="source ~/.bashrc"`: Create a new alias to source the `.bashrc` file easily.

### Transitioning to Zsh with OhMyZsh

#### Setting Up Zsh
- Zsh: An advanced shell with improved features compared to bash, also backward compatible with bash scripts.
- OhMyZsh: A framework for managing zsh configurations, offering plugins and themes to enhance the terminal experience.
- `wget https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh`: Download the OhMyZsh installation script.
- `sh install.sh`: Run the installation script to install OhMyZsh.

#### Implementing Themes
- Powerlevel10k: A powerful theme to augment the zsh terminal experience.
- `git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k`: Clone the Powerlevel10k theme repository.
- Set `ZSH_THEME="powerlevel10k/powerlevel10k"` in `~/.zshrc`: Configure zsh to use the Powerlevel10k theme.
- `source ~/.zshrc`: Apply the new theme configuration.

### Enhancing Zsh with Plugins

#### Adding Useful Plugins
- Plugins: Extensions that add functionalities to the zsh shell.
- Plugins Installation: Use `git clone` command to download and install various plugins like zsh-syntax-highlighting, zsh-autosuggestions, autojump, and zsh-z.
- Configuring Plugins: Edit `~/.zshrc` file to include the list of installed plugins in the `plugins=(...)` section.

#### Exploring Plugin Functionalities
- History Navigation: Navigate through command history using partial matches and arrow keys.
- Autosuggestions: Use tab to get suggestions for completing commands.
- Syntax Highlighting: Get instant feedback on command syntax with color indicators.
- autojump: Quickly navigate to previously visited directories using `j` followed by part of the directory name.
- Directory Navigation: Use tab to explore available folders while typing a path.

*Note: Replace `<placeholders>` with actual values when using the commands.*

### Module 2 - Exercise 1 Enhancing Bash with Aliases and tf Command

In this set of exercises, you will enhance your bash environment by adding useful aliases and integrating the "tf" command, a powerful tool to correct previous console commands quickly. Follow the steps below to accomplish these tasks:

#### 1. Install the “tf” command

_Note: The "tf" command depends on Python 3. If you don't have Python 3 installed, You will need to install it using your package manager._

```bash
sudo apt-get install python3-dev python3-pip python3-setuptools
```

1. First, install the "tf" command, a utility that helps to correct errors in the previously entered console commands. Follow the [installation instructions](https://github.com/nvbn/thefuck) to get it set up in your environment. Here is a quick start command to install it using pip:

```bash
pip3 install thefuck --user
```

2. Add the Alias "drat" to Your .bashrc File
Next, open your .bashrc file in a text editor (like nano) and add an alias for the "tf" command, renaming it to "drat". This will allow you to use "drat" as a shorthand command. Here's how you can do it:

```bash
nano ~/.bashrc
```

In the file, add the following line:

```bash
eval $(thefuck --alias drat)
```

3. Reload your bash configuration to make the changes take effect in the current session.

You need to source the .bashrc file. Use the command below to do this:

```bash
source ~/.bashrc
```

4. Try it out: Test the new alias by deliberately typing an incorrect command and then using "drat" to correct it. Here's a sequence to demonstrate this:

```bash
apt update
drat
```

"drat" should suggest the corrected command, which, in this case, would be `sudo apt update`.

5. Add Additional Aliases for Common Commands to Your .bashrc

Adding aliases can save you time on frequently used commands. Open the .bashrc file again and add aliases for other common commands that you use regularly. Here are a couple of examples:

First, open your bash configuration:

```bash
nano ~/.bashrc
```

Add lines like the following to create new aliases:

```bash
alias restartbash="source ~/.bashrc"
alias gpo="git push origin"
```

Save and exit the editor. Remember to source the .bashrc file again to apply the changes:

Now you can use `restartbash` to reload the .bashrc file and `gpo` to push changes to an origin repository in git.

### Module 2 - Exercise 2 - Setting up and Customizing oh-my-zsh

In this series of exercises, you will be installing and configuring "oh my zsh" along with a number of plugins and themes to enhance your terminal experience. Make sure to follow each step carefully to fully set up your shell environment.

1. Install oh my zsh

Start by installing "oh my zsh", a community-driven framework for managing zsh configuration. Use the following commands to download and run the installation script:

```bash
wget https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh
sh install.sh
```

2. Install the Powerlevel10k Theme (Optional – Install the Recommended Fonts)

Next, enhance your zsh experience with the Powerlevel10k theme, which offers a visually appealing and fast prompt. Follow the [instructions here](https://github.com/romkatv/powerlevel10k#oh-my-zsh) to install and set it up. Optionally, install the recommended fonts to make the most out of the theme's capabilities.

3. Update .zshrc, Source .zshrc, and Configure Your Theme

Update your .zshrc configuration file with your preferred settings, then source the file to apply the changes. Afterwards, configure the Powerlevel10k theme to suit your preferences:

(look for the line that begins `ZSH_THEME=`)

```bash
nano ~/.zshrc
source ~/.zshrc
```

4. Install autojump Using the Package Manager
Install "autojump", a faster way to navigate your filesystem, using your package manager. For instance, on Ubuntu, you can use:

```bash
sudo apt install autojump
```

5. Clone the syntax-highlighting plugin

Clone the syntax-highlighting plugin to add syntax highlighting to your zsh prompt using the command below:

```bash
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
```

6. Clone the zsh autosuggestions plugin

Next, clone the zsh-autosuggestions plugin to get helpful suggestions based on your command history:

```bash
git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
```

7. Clone the autojump Plugin

```bash
git clone https://github.com/wting/autojump.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/autojump
```

8. Add Plugins to .zshrc and Source .zshrc

Open your .zshrc file and add the plugins that you've cloned to the plugins section. After adding the plugins, source your .zshrc file to apply the changes:

```bash
nano ~/.zshrc
# Add plugins to the list, for example: plugins=(git zsh-autosuggestions zsh-syntax-highlighting autojump zsh-z)
source ~/.zshrc
```

9. Experiment with AutoJump

Now that you have autojump installed and configured, experiment with it to navigate through directories faster. Use commands like `j <directory_substring>` to jump to directories:

```bash
j <directory_substring>
```

_Note: You will need to navigate to a few directories first to populate your zsh history.

10. Explore Your Shell with Superpowers
With your now supercharged zsh setup, take some time to explore and enjoy the new capabilities and enhancements. Experiment with different plugins, themes, and settings to make your shell truly your own.

Remember, you can always refer to the documentation of each plugin and theme to explore more features and customization options.

----

## Module 3 - Quick Reference Guide: Composing Commands with Pipes and Redirects

### Commands & Concepts

1. **Pipes (`|`)**:
   - **Purpose**: To pass the output of one command as input to another command.
   - **Usage**: `command1 | command2`

2. **Redirects (`>` and `>>`)**:
   - **Purpose**: To direct the output of a command into a file.
   - **`>`**: Overwrites the file with the output.
   - **`>>`**: Appends the output to the existing content of the file.
   - **Usage**: `command > filename` or `command >> filename`

3. **seq**:
   - **Purpose**: Generate a sequence of numbers.
   - **Flags**:
     - **number**: Upper limit of the sequence.
   - **Usage**: `seq number`

4. **shuf**:
   - **Purpose**: Shuffle the lines of the output randomly.
   - **Common Flags**:
     - **-n**: Output only the specified number of lines.
   - **Usage**: `command | shuf` or `shuf -n number filename`

5. **cat**:
   - **Purpose**: Concatenate and display file content.
   - **Usage**: `cat filename`

6. **cut**:
   - **Purpose**: Extract specific fields from lines in a file.
   - **Flags**:
     - **-f**: Specifies the field number to be extracted.
     - **-d**: Specifies the delimiter.
   - **Usage**: `cut -f field_number -d 'delimiter' filename`

7. **wc**:
   - **Purpose**: Count the number of lines, words, and bytes in a file.
   - **Common Flags**:
     - **-l**: Count the number of lines.
     - **-w**: Count the number of words.
   - **Usage**: `wc filename` or `command | wc -l`

8. **xargs**:
   - **Purpose**: Construct and execute command lines from standard input.
   - **Flags**:
     - **-L**: Specify the number of lines of input to group together.
     - **-I {}**: Replace occurrences of {} in the initial arguments with names read from standard input.
   - **Usage**: `command | xargs -L number command2` or `command | xargs -I {} command2 {}`

9.  **printf**:
    - **Purpose**: Format and print data.
    - **Usage**: `printf "format_string" arguments`

10. **mkdir and cd (via 'take' alias in zsh)**:
    - **Purpose**: Create a new directory and move into it in a single command (zsh only).
    - **Usage**: `take directoryname`

### Useful Combinations

- Counting number of users: `cat /etc/passwd | cut -f 1 -d : | wc -l`
- Creating files named after users: `cat /etc/passwd | cut -f 1 -d : | xargs -I {} touch file_for_{}`

Remember, mastering the combination of these commands and flags can greatly enhance your ability to efficiently manage and manipulate files and data within a Unix-like system.

### Module 3 - Exercises: Composing Commands with Pipes and Redirects

#### Exercise 1

##### Task
Create a directory called `composition_playground` and navigate to this new directory in one command.

###### Steps
1. Use a command that combines `mkdir` and `cd` to create and navigate to the directory in one step.

#### Exercise 2

##### Task
Create a file called `sequential_numbers.txt` that contains a sequence of numbers from 1 to 100.

###### Steps
1. Use the `seq` command to generate a sequence of numbers from 1 to 100.
2. Redirect the output to a file named `sequential_numbers.txt`.

#### Exercise 3

##### Task
Shuffle the contents of `sequential_numbers.txt` and save the result in a new file called `shuffled_numbers.txt`.

###### Steps
1. Use the `cat` command to display the contents of `sequential_numbers.txt`.
2. Pipe the output to the `shuf` command to shuffle the numbers.
3. Redirect the shuffled output to a new file called `shuffled_numbers.txt`.

#### Exercise 4

##### Task
Sort the shuffled numbers in `shuffled_numbers.txt` in ascending order and append the result to `sequential_numbers.txt`.

###### Steps
1. Use the `cat` command to display the contents of `shuffled_numbers.txt`.
2. Pipe the output to the `sort` command to sort the numbers in ascending order.
3. Redirect the sorted output to `sequential_numbers.txt` using the append (`>>`) operator.

#### Exercise 5

##### Task
Using only the `echo` and `xargs` commands in a single command line, create files named `foo`, `bar`, and `baz`.

###### Steps
1. Use the `echo` command to output the strings "foo", "bar", and "baz", separated by spaces.
2. Pipe the output to the `xargs` command (omitting the `-L` flag) to create files with these names.

_(Hint: Use spaces as delimiters in the `echo` command and omit the `-L` flag in `xargs` to create multiple files.)_

#### Additional Exercises

##### Exercise 6

##### Task
Create a file containing the usernames from `/etc/passwd` sorted in reverse alphabetical order.

###### Steps
1. Use the `cat` command to display the contents of `/etc/passwd`.
2. Extract usernames using the `cut` command with appropriate flags.
3. Sort the usernames in reverse alphabetical order using the `sort` command with appropriate flags.
4. Redirect the output to a new file.

#### Exercise 7

##### Task
Count the number of files in the `composition_playground` directory.

###### Steps
1. Use the `ls` command to list the files in the `composition_playground` directory.
2. Pipe the output to the `wc` command with the `-l` flag to count the number of files.

#### Exercise 8

##### Task
Create a script called `user_greetings.sh` that generates a greeting for each user listed in `/etc/passwd`.

###### Steps
1. Use the `printf` command with a parameterized string to create greetings.
2. Utilize `xargs` to apply this command to each username extracted from `/etc/passwd`.
3. Redirect the output to a script file named `user_greetings.sh`.
4. (Optional) Run the script to see the greetings displayed in the terminal.

Please note that these exercises are designed to gradually build your skills in composing commands with pipes and redirects. Feel free to refer back to the module content as needed while working through them.

----

## Module 4 Reference Guide - Manipulating Files and Text

### 1. `find` - Locate Files and Directories

**Usage**: `find [location(s)] [expression]`

#### Common Options:

- `-name` : Search for items by name (case-sensitive).
- `-iname` : Search for items by name (case-insensitive).
- `-type` : Specify the type of item to find (`f` for files, `d` for directories).
- `-o` : Logical OR; used to combine two search criteria where either condition can be true.
  
#### Examples:

- `find . -name wizard` : Search for items named 'wizard' in the current directory.
- `find . -name *wizard` : Search for items with names ending with 'wizard' in the current directory.
- `find / -type d -iname "*wizard*"` : Search for directories with names containing the string 'wizard' (case-insensitive) in the root directory.

### 2. `grep` - Search Text using Patterns

**Usage**: `grep [options] [pattern] [file/directory]`

#### Common Options:

- `-i` : Case insensitive search.
- `-l` : Only display filenames where the pattern is found.
- `-v` : Invert match; find lines that do not match the pattern.
- `-E` : Use extended regular expressions.

#### Examples:

- `grep "wizard" ~/.zshrc` : Search for the string 'wizard' in the .zshrc file.
- `history | grep "wizard$"` : Search for commands ending with 'wizard' in the command history.

### 3. `sed` - Stream Editor

**Usage**: `sed [options] [expression] [file]`

#### Common Options:

- `-i` : Edit files in place (makes changes directly to the original file).
- `-e` : Allows the use of multiple editing commands.
- `s` : Substitution command, typically used as `s/old/new/g` where `g` signifies global replacement.

#### Examples:

- `sed 's/Hello there/howdy/g' user_greetings.txt` : Replace 'Hello there' with 'howdy' globally in the file 'user_greetings.txt'.
- `sed 's/Hello there/howdy/g' user_greetings.txt > cowboy_greetings.txt` : Save the modified output to a new file 'cowboy_greetings.txt'.

### 4. `xargs` - Build and Execute Command Lines from Standard Input

**Usage**: `xargs [options] [command]`

#### Common Options:

- `-I` : Specify a placeholder that will be replaced by the line of input.
- `-0` : Expect NUL (\0) character as a separator instead of whitespace.
- `-L` : Specify the number of lines of input to be used for each command execution.

#### Examples:

- `find . -type f -name "*.txt" | xargs grep -l "pattern"` : Find text files containing the "pattern" and display the filenames.

### 5. Logical Operators in the Shell

- `&&` : Logical AND; executes the second command only if the first command is successful.
- `||` : Logical OR; executes the second command only if the first command fails.

#### Examples:

- `command1 && command2` : Executes 'command2' only if 'command1' succeeds.
- `command1 || command2` : Executes 'command2' only if 'command1' fails.

#### Exercises:

- Utilize `find` to locate files with a specific extension in a directory tree.
- Use `grep` to search for specific patterns within files located by `find`.
- Create a pipeline with `find`, `grep`, and `sed` to locate files, identify a specific pattern, and replace the pattern within each file.
- Explore the usage of `&&` and `||` operators to create complex command pipelines with conditional execution.

### Vim Basic Guide - A Command-Line Text Editor

Vim is a powerful text editor used in the CLI (Command Line Interface). Here is a basic guide to get you started with some of the most common Vim commands:

#### 1. Launching and Exiting Vim

##### Commands:

- `vim [filename]` : Launch Vim and open the specified file, or create a new one if it does not exist.
- `:w` : Save the current file (write).
- `:q` : Quit Vim (you'll need to save any changes before quitting).
- `:wq` or `:x` : Save the current file and quit Vim.
- `:q!` : Quit Vim without saving changes.
- `ZZ` : Save the current file and quit Vim (similar to `:wq`).

#### 2. Navigating Within Vim

##### Commands:

- `h` : Move the cursor left by one character.
- `j` : Move the cursor down by one line.
- `k` : Move the cursor up by one line.
- `l` : Move the cursor right by one character.
- `G` : Move to the end of the file.
- `gg` : Move to the beginning of the file.
- `:[number]` : Move to the line specified by [number].

#### 3. Editing Text

##### Modes:

- `i` : Enter insert mode (allows you to insert text at the cursor position).
- `Esc` : Exit insert mode and return to command mode (default mode).
- `a` : Enter insert mode with the cursor moved one character to the right.
- `o` : Create a new line below the current line and enter insert mode.
- `O` : Create a new line above the current line and enter insert mode.
- `u` : Undo the last change.
- `Ctrl+r` : Redo the last undone change.

##### Commands:

- `dd` : Delete the current line.
- `D` : Delete from the current cursor position to the end of the line.
- `dw` : Delete from the current cursor position to the end of the word.
- `x` : Delete the character under the cursor.
  
#### 4. Searching and Replacing

##### Commands:

- `/[pattern]` : Search forward in the file for [pattern].
- `?[pattern]` : Search backward in the file for [pattern].
- `n` : Repeat the last search in the same direction.
- `N` : Repeat the last search in the opposite direction.
- `:%s/[old]/[new]/g` : Replace all instances of [old] with [new] globally in the file.
- `:%s/[old]/[new]/gc` : Replace all instances of [old] with [new], with a prompt for confirmation for each instance.

#### Tips

- While in command mode, typing `:` allows you to enter commands and execute Vimscript.
- You can combine several commands by separating them with `|`. For instance, `:w | q` will save and then quit.
- You can customize Vim extensively through the `.vimrc` configuration file, allowing you to create a personalized workflow.

Remember, Vim has a steep learning curve, but with practice, it can become a highly efficient and personalized text editor. Start with the basics and gradually explore more advanced commands and configurations as you become comfortable.

### Summary

Remember, these commands and options form powerful tools for file and text manipulation on Unix-like systems. Experiment with different combinations to build complex pipelines that can automate many aspects of system and file management.

## Module 4 Exercises - Manipulating Files and Text


1. **Exploring `find` command:**
   
   a. Use the `find` command to locate all `.txt` files in your current directory.
   
   b. Use the `find` command to find all directories with the name "project" (case insensitive) in your system.
   
   c. Try finding files modified in the last 7 days in your document directory.

2. **Utilizing `grep` command:**

   a. Use `grep` to search for your username all directories.
   
   b. Download this word list into your `~` directory: `wget https://magician.codes/words.txt` and grep for words that can be made on a calculator (only using some combination of these letters: `BEHILOS`) hint: the regex is `ˆ[behilos]*$`
   
3. **Working with `sed` command:**

   a. Create a text file named "sample.txt" and add some text lines including "Hello World". Use `sed` to replace "World" with "Linux" and save the output to a new file.
   
4. **Practicing Vim skills:**

   a. Create a new file using Vim and practice inserting text in different modes (insert mode, append mode).
   
   b. Practice navigating through the file using `h`, `j`, `k`, `l`, and jumping to the beginning and the end of the file with `gg` and `G`.
   
   c. Try editing the file by deleting lines, undoing changes, and then saving your changes.

5. **Combining commands:**
   
   a. Use `grep` to search for a particular pattern in the output of the `history` command and then use `sed` to replace a string pattern in the resulting output.
   
6. **Bonus Exercises Vim:**

a. Launch Vim and create a new file with some content.
b. Use navigation commands to move around the file.
c. Edit the text using different modes and commands.
d. Practice searching for text and making global replacements.
e. Save your changes, or practice exiting without saving to discard changes.

Feel free to explore further and experiment with different flags and options for each command to deepen your understanding.

----

## Module 5 - Connecting to the world and Manipulating Data Quick Reference

### curl

**Purpose**: `curl` is a command-line tool for transferring data with URLs. It supports various protocols including HTTP, HTTPS, FTP, and more.

#### Common Commands and Flags:

1. **`curl [URL]`** 
   - Purpose: Fetches the URL's content to the console.
   
2. **`curl -o [filename] [URL]`**
   - `-o`: Specifies the output file where the result will be saved instead of being displayed on the console.
   
3. **`curl -O [URL]`**
   - `-O`: Downloads the file from the URL and keeps the original file name.
   
4. **`curl -I [URL]`**
   - `-I`: Fetches only the HTTP headers from the response, to check the status or properties of the document.
   
5. **`curl -X [HTTP_METHOD] [URL]`**
   - `-X`: Specifies a custom request method to use when communicating with the HTTP server (e.g., GET, POST, PUT).
   
6. **`curl -d "[DATA]" [URL]`**
   - `-d`: Sends the specified data in a POST request to the HTTP server.

7. **`curl -u [username:password] [URL]`**
   - `-u`: Provides username and password to the server for authentication.
   
8. **`curl -v [URL]`**
   - `-v`: Makes curl show more details and information about the transfer (verbose mode).

9. **`curl -L [URL]`**
   - `-L`: Tells curl to follow HTTP redirects.

#### Example Usage:

1. Download a file and save it with a specific name:

```bash
curl -o example.html http://www.example.com/index.html
```

2. Make a POST request with data:

```bash
curl -X POST -d "param1=value1&param2=value2" http://www.example.com/endpoint
```


---

### jq

**Purpose**: `jq` is a lightweight and flexible command-line JSON processor. It is like sed for JSON data – you can use it to slice, filter, map, and transform structured data.

#### Common Commands and Flags:

1. **`jq '.' [file]`**
- Purpose: Pretty-prints the JSON file.

2. **`jq '.[key]' [file]`**
- Purpose: Filters the JSON data by key.

3. **`jq '.[key1, key2]' [file]`**
- Purpose: Filters the JSON data by multiple keys.

4. **`jq '.[start:end]' [file]`**
- Purpose: Slices an array from start to end index.

5. **`jq 'map(expression)' [file]`**
- Purpose: Applies a transformation to each element in an array.

6. **`jq 'select(expression)' [file]`**
- Purpose: Selects elements that match the given expression.

7. **`jq 'length' [file]`**
- Purpose: Returns the length of arrays or objects.

### Example Usage:

1. Pretty-print a JSON file:

```bash
jq '.' data.json
```

2. Get a value from a JSON file by key:

```bash
jq '.name' data.json
```

3. Filtering multiple keys from a JSON file:

```bash
jq '.name, .age' data.json
```

4. Transform JSON data using map:

```bash
jq 'map(. + { "newKey": "newValue" })' data.json
```

Note: For both `curl` and `jq`, more advanced options and flags can be explored by referring to their respective man pages (`man curl`, `man jq`) or their online documentation.

### A Useful Trick (HT Craig Walls & Brian Sletten)

```bash
export ACCESS_TOKEN=`curl http://localhost:8080/oauth/token` \
-d "grant_type=password&username=habuma&password=password" \
-H "Content-type:application/x-www-form-urlencoded; charset=utf-8" \
-u myclient:secret --silent | js -r ".access_token"

curl localhost:8080/secured -H "Authorization: Bearer $ACCESS_TOKEN"
```
