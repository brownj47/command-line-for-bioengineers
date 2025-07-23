# command-line-for-bioengineers

This repository hosts the content for my short course teaching command line literacy for bioengineers.

## Table of Contents
- [What is the Command Line?](#what-is-the-command-line)
- [Why Use the Command Line?](#why-use-the-command-line)
- [Terminal Commands Cheat Sheet](#terminal-commands-cheat-sheet)
- [Exercise 1](./exercise-1)

## What is the Command Line?
The command line interface or CLI refers to a text-based interface for interacting with an operating system. Operating systems include Mac, Windows, and Linux. You access the CLI through a "shell." Popular shell programs include bash, zsh (Mac), Powershell (Windows). 

Within a CLI, you interact with the operating system by sending text commands. An example command is shown below. 

```sh
echo "Hello, World!"
```
`echo <your message>` is the print statement of the command line. It prints the text you provide to the terminal. In this case, it will print "Hello, World!" to the terminal. 

## Why Use the Command Line?
The command line is a powerful tool for bioengineers and scientists for several reasons:
1. **Automation**: You can write scripts to automate repetitive tasks, saving time and reducing errors.
2. **Efficiency**: Once you know it well, many tasks can be performed faster via the command line than through a graphical user interface (GUI).
3. **Remote Access**: You can access and control remote servers or systems via the command line. This is particularly useful for running simulations or processing large datasets on high-performance computing clusters.
4. **Version Control**: Command line tools like Git allow for efficient version control of code and documents.      
5. **Data Processing**: Command line tools can handle large datasets and perform complex data manipulations efficiently.

A bioengineer might use the command line to:
1. Create an automated script that processes large biological datasets.
2. Run bioinformatics tools to analyze genetic or protein data.
3. Run simulations of biological systems on remote servers.
4. Manage source code for a project using Git.

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