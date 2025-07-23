# Exercise 1
In this exercise, you will learn how to navigate the command line, create and manage directories and files, and use basic commands. This will help you become familiar with the command line interface and prepare you for more advanced exercises in this course.

## Table of Contents
- [Learning Objectives](#learning-objectives)
- [Prerequisites](#prerequisites)
- [Getting Started](#getting-started)
- [Orienting Yourself in the Command Line](#orienting-yourself-in-the-command-line)
- [Computer File System Structure](#computer-file-system-structure)
- [Creating and Managing Directories and Files](#creating-and-managing-directories-and-files)
    - [Creating Directories](#creating-directories)
    - [Creating Files](#creating-files)
    - [Viewing File Contents](#viewing-file-contents)
    - [Deleting Files and Directories](#deleting-files-and-directories)
- [Summary](#summary)

## Learning Objectives
By the end of this exercise, you will be able to:
1. Navigate the command line interface.
2. Create and manage directories and files.
3. Use basic commands like `pwd`, `ls`, `cd`, `mkdir`, `touch`, `cat`, `echo`, and `rm`.
4. Understand the file system structure of your computer.
5. Delete files and directories using the command line.

## Prerequisites
Before starting this exercise, make sure you have the following tools installed:
- [Git](https://git-scm.com/downloads) (includes Git Bash for Windows users)
    -  Windows users can download Git for Windows, which includes [Git Bash](https://git-scm.com/downloads/win), a terminal emulator that provides a Unix-like command line experience. This will create a more consistent experience across platforms during this excercise.
    - Mac users should install [Homebrew](https://brew.sh/). Homebrew is a package manager for macOS that allows you to easily install and manage software packages like python and even [Visual Studio Code](https://formulae.brew.sh/cask/visual-studio-code). 
- [Visual Studio Code](https://code.visualstudio.com/download) (or any text editor of your choice)

## Getting Started

Note: Throughout this excercise please type the commands rather than copy-pasting them, as this will help you learn the commands better.

1. To get started with the command line, you will need to open a terminal or command prompt.
    - Mac: open the Terminal application (found in Applications > Utilities).
    - Windows: open Git Bash (if you installed Git) or Command Prompt (cmd).
2. Your terminal should now be open and ready for you to type commands. You will see a prompt that looks something like this:
    ```
    username@hostname:~$
    ```
    This indicates that you are in your home directory.

![Terminal Prompt Screenshot](TODO: Insert screenshot of terminal prompt here.)

## Orienting Yourself in the Command Line
Whenever I start using the command line, I like to start by asking the following questions:
1. "Where am I?" 
```sh
pwd
```
`pwd` which stands for "Print Working Directory." will cause the command line to print the full path to the directory (a fancy way to say folder) you are in.

2. "What's in here?" 
```sh
ls
```

The `ls` command, which stands for "List," will list all the files and subdirectories in your current directory.

## Computer File System Structure
The file system of your computer is organized in a hierarchical structure, similar to a tree. At the top of this hierarchy is the root directory, which contains all other directories and files.
On Linux and Mac, the root directory is represented by a forward slash `/`, while on Windows it is represented by a drive letter followed by a colon and a backslash (e.g., `C:\`). 

![File Tree Structure by By Peter Flass - Own work, CC BY-SA 4.0, https://commons.wikimedia.org/w/index.php?curid=129131805](https://upload.wikimedia.org/wikipedia/commons/2/2c/File_Hierarchy.png)


1. Navigate to the root directory of your computer using `cd`:
```sh
cd /
```
2. Use the `ls` command to list the contents of the root directory:
```sh
ls
```
You will most likely see directories like `home`, `usr`, `bin`, etc. The root directory is the top-level directory of your file system, and you will not often need to navigate here directly. Your personal files are usually stored in a subdirectory of the root directory, such as `/home/yourusername` on Linux or Mac, or `C:\Users\yourusername` on Windows. 

3. Navigate back to your home directory using `cd`:
```sh
cd ~
```
Alternatively you could use `cd /home/yourusername` (replace `yourusername` with your actual username).

## Creating and Managing Directories and Files
Now that you know how to navigate the file system, let's practice creating and managing directories and files.
1. Open your terminal or Git Bash.
2. Use the `pwd` command to confirm you are in your home directory.
3. Use the `ls` command to list the contents of your home directory. You should see directories like `Documents`, `Downloads`, `Desktop`, etc.
4. Use the `cd` command to navigate to your Desktop directory:
```sh
cd Desktop
```
5. Use the `mkdir` command to create a new directory called `bioengineer`:
```sh
mkdir bioengineer
```
6. Use the `ls` command to confirm that the `bioengineer` directory was created successfully. You should see `bioengineer` listed in the output.
7. Navigate into the `bioengineer` directory using the `cd` command:
```sh
cd bioengineer
```
8. Inside the `bioengineer` directory, create a new file called `bio.txt` using the `touch` command:
```sh
touch bio.txt
```
9. Create a second file called `bioengineer.txt` using the `touch` command:
```sh
touch bioengineer.txt
```
10. Use the `ls` command to confirm that the `bio.txt` and `bioengineer.txt` files were created successfully. You should see both files listed in the output.
11. You can also use the `ls -l` command to see more details about the files, such as their size and modification date:
```sh
ls -l
```
12. Confirm the files were created by looking in the `bioengineer` directory in your finder or file explorer.
13. Use the `cat` command to display the contents of the `bio.txt` file:
```sh
cat bio.txt
```
Note: Since it is currently empty, you will not see any output.
14. Now, use the `echo` command to add some text to the `bio.txt` file:
```sh
echo "Welcome MAB Class of 2026!" > bio.txt
```
This command will write the text "Welcome MAB Class of 2026!" into the `bio.txt` file.
15. Use the `cat` command again to display the contents of the `bio.txt` file:
```sh
cat bio.txt
```
You should see the text "Welcome MAB Class of 2026!" displayed in the terminal.

16. Use the `rm` command to delete the `bio.txt` file:
```sh
rm bio.txt
```
17. Use the `ls` command again to confirm that the file has been deleted successfully.
You should no longer see `bio.txt` listed in the output.    
18. Navigate back out of the `bioengineer` directory using:
```sh
cd ..
```
19. Try running the `rm` command to remove the `bioengineer` directory:
```sh
rm bioengineer
```
You will get an error message saying that the directory is not empty. This is because the directory contains the `bioengineer.txt` file.
20. To remove the directory, you need to use the `rm -r` command, which stands for "remove recursively." This command will delete the directory and all of its contents. Be careful with this command, as it will permanently delete everything in the directory without confirmation:
```sh
rm -r bioengineer
```
21. Use the `ls` command again to confirm that the `bioengineer` directory has been deleted successfully. You should no longer see `bioengineer` listed in the output.
You can also confirm the directory was deleted by looking in your finder or file explorer.
You should not see the `bioengineer` directory anymore.

## Summary
In this excercise, you learned how to navigate the file system using the command line, create and manage directories and files, and use basic commands like `pwd`, `ls`, `cd`, `mkdir`, `touch`, `cat`, `echo`, and `rm`. You also learned how to delete files and directories using the `rm` command. These skills are essential for working with the command line and will be useful for future excercises in this course.