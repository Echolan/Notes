##CLI: Command Line Interface

- Windows: Git Bash
- Mac/Linux: Terminal

Commands: pwd, clear, ls, cd, mkdir, 
touch, cp, rm, mv, date, echo...

**pwd**(print working directory) can be used at any time to display the path to your working directory.

- CLI commands follow this recipe: **command flags arguments**
- **command** is the CLI command which does a specific task
- **flags** are options we give to the **command** to trigger certain behaviors, preceded by a -
- **arguments** can be what the **command** is going to modify, or other options for the command
- Depending on the **command**, there can be zero or more **flags** and **arguments**
- For example **pwd** is a **command** that requires no **flags** or **arguments**

##CLI Commands
- **pwd** displays the path to the current working directory
- **clear** will clear out the commands in your current CLI window
- **ls** lists files and folders in the current directory
- **ls - a** lists hidden and unhidden files and folders
- **ls -al** lists details for hidden and unhidden files and folders
- **cd** stands for "change directory"
- **cd** with no argument takes you to your home directory
- **cd ..** allows you to change directory to one level above your current directory
- **mkdir** stands for "make directory"
- **touch** creates an empty file
- **cp** stands for "copy"
- **cp** can also be used for copying the contents of directories, but you must use the **-r** flag.
- **rm** stands for "remove"
- You can also use **rm** to delete entire directories and their contents by using the **-r** flag. (*Be very careful when you do this, there is no was to undo an **rm***)
- **mv** stands for "move"

##Configure Username and Email
- git config --global user.name "Your Name Here"
- git config --global user.email "Your_email@example.com"
- git config --list

##Creating a GitHub Repository
Two methods of creating a GitHub repository:

1. Start a repository from scratch
2. "Fork" another user's repository

##Creating a Local Copy
- Open Git Bash

- Create a directory on your computer where you will store your copy of the repo:

    $ mkdir ~/test-repo

- Navigate to this new directory using the following command:

    $ cd ~/test-repo

- Initialize a local Git repository in this directory

    $ git init
- Point your local repository at the remove repository you just created on the GitHub server

    $ git remote add origin https://github.com/yourUserNameHere/test-repo.git

## Clone the Repo
$ git clone https://github.com/yourUserNameHere/repoNameHere.git

## Adding
- **git add .** adds all new files
- **git add -u** updates tracking for files that changed names or were deleted
- **git add -A** does both of the previous

You should do this before committing.

## Committing
- git commit -m "message"
- git commit -m "add"

## Pushing
- git push
- git push -u origin master

When encountering situation "failed to push some refs to git", you may try this

- git pull --rebase origin master

Then try to push again.

##Reference
Most of the notes are quoted from the course "The Data Scientist’s Toolbox", which is given by Professor Jeff Leek. Thanks for him.