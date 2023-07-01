# **Instructions for working with Git**

## *__What is Git__*
Git is a free and open source distributed version control system designed to handle everything from small to very large projects with speed and efficiency.

## *__What is GitHub__*
GitHub is a code hosting platform for version control and collaboration. It allows you and other users to work on projects together from anywhere.

## *__Remote repositories__*
A *remote repository* is the versions of your project that are stored on a remote server.
* Git clone

Clones the passed repository to your computer.

Format: Git clone <link to remote repository>
* Git pull

Gets the changes from the passed in remote repository and updates the working copy to match the remote repository.
Format: git pull [key][remote repository name]
* Git push

Downloads changes to the remote repository.

Format: git push [key] [remote repository name] [branch name]

## *__Preparing the repository__*
To create a new repository, we need to open a terminal, go to our project folder and run the git init command.

## *__Git Commands__*
* Git add

The git add command adds the contents of the working directory to the index (staging area) for later commit

* Git status

The git status command shows the status of files in the working directory and index

* Git commit

The git commit command takes all the data added to the index with git add and saves a snapshot of it in the internal database

* Git diff

The git diff command is used to calculate the difference between any two Git trees.

## *__Moving between saves__*
To move between commits, use the *git checkout* command. It is used in the repository folder as follows: *git checkout <commit number>*

## *__Changelog__*
In order to see all the changes made in the repository, the *git log* command is used. To do this, just run the *git log* command in the folder with the repository

## *__Branches in Git__*
Create a branch. To create a branch, use the *git branch* command. This is done as follows in the folder with the repository: *git branch <name of the new branch>*

![Branching in Git](/Branch.png)

* *Merging branches*

To add a branch to the current branch, use the *git merge* command.

* *Deleting branches*

To delete a branch, enter the command *git branch -d 'name branch'*