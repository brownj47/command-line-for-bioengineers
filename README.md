# command-line-for-bioengineers

This repositiory hosts the content for my short course teaching command line literacy for bioengineers. 

## What is the Command Line?
The command line interface or CLI refers to a text-based interface for interacting with an operating system. Operating systems include Mac, Windows, and Linux. You access the CLI through a "shell." Popular shell programs include bash, zsh (Mac), Powershell (Windows). 

Within a CLI, you interact with the operating system by sending text commands. An example command is shown below. 


```sh
pwd
```
`pwd` stands for "Print Working Directory" and causes the shell to print out the current location of the command prompt. 

## Why Use the Command Line?
The command line is a powerful tool for bioengineers and scientists for several reasons:
1. **Automation**: You can write scripts to automate repetitive tasks, saving time and reducing errors.
2. **Efficiency**: Many tasks can be performed faster via the command line than through a graphical user interface (GUI).
3. **Remote Access**: You can access and control remote servers or systems via the command line.
4. **Version Control**: Command line tools like Git allow for efficient version control of code and documents.      
5. **Data Processing**: Command line tools can handle large datasets and perform complex data manipulations efficiently.

## Getting Started
To get started with the command line, you need to open a terminal application. The terminal is a program that provides a command line interface.
- On **Mac**, you can find the Terminal application in Applications > Utilities.        
- On **Windows**, you can use Command Prompt or PowerShell, which can be found in the Start menu.
- On **Linux**, you can usually find the terminal in the applications menu or by pressing `Ctrl + Alt + T`.

## Basic Navigation
To navigate the file system using the command line, you can use the following commands:
- `pwd`: Print the current working directory.
- `ls`: List the files and directories in the current directory.
- `cd <directory>`: Change to the specified directory. For example, `cd Documents` will move you into the Documents directory.
- `cd ..`: Move up one directory level.
- `cd ~`: Move to your home directory.
- `mkdir <directory>`: Create a new directory with the specified name.
- `rmdir <directory>`: Remove an empty directory.
- `rm <file>`: Remove a file. Use `rm -r <directory>` to remove a directory and its contents recursively.
- `cp <source> <destination>`: Copy a file or directory from source to destination.
- `mv <source> <destination>`: Move or rename a file or directory.  

## Terminal Commands Cheat Sheet
Command line commands can be used to navigate the file system, manipulate files, and run programs. Below is a cheat sheet of common commands.
| Command | Description |
|---------|-------------|   
| `pwd` | Print Working Directory - shows the current directory |
| `ls` | List files in the current directory |
| `cd` | Change Directory - move to a different directory |
| `mkdir` | Make Directory - create a new directory |
| `touch` | Create an empty file or update the timestamp of an existing file |
| `cp` | Copy - copy a file or directory |
| `mv` | Move - move or rename a file or directory |
| `rm` | Remove - delete a file or directory |
| `cat` | Concatenate - display the contents of a file |
| `less` | View the contents of a file one screen at a time |
| `head` | Display the first few lines of a file |
| `tail` | Display the last few lines of a file |
| `echo` | Print text to the terminal |
| `grep` | Search for a pattern in files |
| `find` | Search for files and directories |
| `chmod` | Change file permissions |
| `chown` | Change file ownership |
| `history` | Show command history |
| `clear` | Clear the terminal screen |
| `exit` | Exit the terminal session |

## Excercise 1