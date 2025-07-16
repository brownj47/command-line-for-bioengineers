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
2. **Efficiency**: Once you know it well, many tasks can be performed faster via the command line than through a graphical user interface (GUI).
3. **Remote Access**: You can access and control remote servers or systems via the command line.
4. **Version Control**: Command line tools like Git allow for efficient version control of code and documents.      
5. **Data Processing**: Command line tools can handle large datasets and perform complex data manipulations efficiently.

You might use the command line to:
create an automated script that processes large biological datasets, run bioinformatics tools, run simulations of biological systems on remote servers, or manage source code for a project with git.

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


## Basic Navigation
To navigate the file system using the command line, you can use the following commands:
- `pwd`: Print the current working directory.
- `ls`: List the files and directories in the current directory.
- `cd <directory>`: Change to the specified directory. For example, `cd Documents` will move you into the Documents directory.
- `cd ..`: Move up one directory level.
- `cd ~`: Move to your home directory.

## Excercise 1

Note: please type the commands rather than copy-pasting them, as this will help you learn the commands better.

Whenever I start using the command line, I like to start by asking the following questions:
1. "Where am I?"
    To answer this question, you can use the `pwd` command, which stands for "Print Working Directory." This command will show you the current directory you are in.
2. "What's in here?"
    To answer this question, you can use the `ls` command, which stands for "List." This command will list all the files and directories in your current directory.

The root of your computer is represented by a forward slash `/`. You can use `cd /` to navigate to the root directory of your computer. You will most likely see directories like `home`, `usr`, `bin`, etc. 

This is the top-level directory of your file system, and you will not often need to navigate here directly. Your personal files are usually stored in a subdirectory of the root directory, such as `/home/yourusername` on Linux or Mac, or `C:\Users\yourusername` on Windows. 

To navigate to your home directory, you can use the command `cd ~` or `cd /home/yourusername` (replace `yourusername` with your actual username).

Next, use `cd` to change to your Desktop directory. You can do this by typing `cd Desktop` or `cd /Users/yourusername/Desktop` (replace `yourusername` with your actual username).

Next, use `mkdir` to create a new directory called `bioengineer` in your Desktop directory. You can do this by typing `mkdir bioengineer`.

Open this folder in your finder or file explorer so that you can see what it looks like. 
Once you are back on the command line, use ls to confirm that the `bioengineer` directory was created successfully. Navigate into the `bioengineer` directory using `cd bioengineer`.

Inside the `bioengineer` directory, create a new file called `bio.txt` using the `touch` command. You can do this by typing `touch bio.txt`.
Create a second file called `bioengineer.txt` using the `touch` command. You can do this by typing `touch bioengineer.txt`.

Now, use the `ls` command to confirm that the `bio.txt` and `bioengineer.txt` files were created successfully.
You should see `bio.txt` and `bioengineer.txt` listed in the output of the `ls` command.
You can also use the `ls -l` command to see more details about the files, such as their size and modification date.
Also confirm the files were created by looking in the `bioengineer` directory in your finder or file explorer.

Next, use the `cat` command to display the contents of the `bio.txt` file. Since it is currently empty, you will not see any output.
Now, use the `echo` command to add some text to the `bio.txt` file. You can do this by typing `echo "Hello, Bioengineer!" > bio.txt`. This command will write the text "Hello, Bioengineer!" into the `bio.txt` file.
Now, use the `cat` command again to display the contents of the `bio.txt` file. You should see the text "Hello, Bioengineer!" displayed in the terminal.

Use the `rm` command to delete the `bio.txt` file. You can do this by typing `rm bio.txt`. Use the `ls` command again to confirm that the file has been deleted successfully.

Then navigate back out of the `bioengineer` directory using `cd ..`. try running removing the `bioengineer` directory using the `rm` command. You will get an error message saying that the directory is not empty. This is because the directory contains the `bioengineer.txt` file.
To remove the directory, you need to use the `rm -r` command, which stands
for "remove recursively." This command will delete the directory and all of its contents. You can do this by typing `rm -r bioengineer`.
Use the `ls` command again to confirm that the `bioengineer` directory has been deleted successfully.