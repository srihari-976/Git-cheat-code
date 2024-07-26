
# Git Course

This guide provides an overview of common Git commands and their usage.

## Git Basics

### Checking the Git Version
```sh
git --version
```

### Checking the Status of Your Repository
```sh
git status
```

### Initializing a Git Repository
To initialize a repository with the default branch named `master`:
```sh
git init
```
To initialize a repository with a branch named `main`:
```sh
git init -b main
```

### Staging and Committing Changes
To add a specific file to the staging area:
```sh
git add git.txt
```

To add all files to the staging area:
```sh
git add .
```

To commit the staged files with a message:
```sh
git commit -m "My first commit"
```

To commit all changes (including unstaged) with a message:
```sh
git commit -a -m "My first commit"
```

### Viewing Commit History
```sh
git log
```

### Viewing Changes
To see what changes have been made but not yet staged:
```sh
git diff
```

To see changes in the staged area:
```sh
git diff --staged
```

### Removing Files
To remove a file from the repository but keep it in the working directory:
```sh
git rm --cached git.txt
```

## Branching and Merging

### Creating and Managing Branches
To create a new branch named `main`:
```sh
git branch - main
```

To see all branches:
```sh
git branch -a
```

To switch to a specific branch:
```sh
git switch main
```

To create and switch to a new branch named `master`:
```sh
git switch -c master
```

To switch to the previous branch:
```sh
git switch -
```

To delete a branch named `master`:
```sh
git branch -d master
```

### Merging Branches
To merge changes from the `master` branch into the `main` branch:
```sh
git switch main
git merge master
```

## Working with Remote Repositories

### Setting Up SSH
To generate an SSH key:
```sh
ssh-keygen -o
```

### Connecting to a Remote Repository
To add a remote repository:
```sh
git remote add origin <repository_url>
```

### Pushing Changes
To push changes from the local repository to the remote repository:
```sh
git push -u origin main
```

To push changes forcefully:
```sh
git push -f origin main
```

## Tags

### Listing Tags
To find out the number of tags for the project:
```sh
git tag -l
```

### Creating and Pushing Tags
To create a new tag:
```sh
git tag -a v1.0 -m "1st tag"
```

To push a tag to the remote repository:
```sh
git push origin v1.0
```

### Viewing a Tag
To see a particular tag:
```sh
git show v1.0
```

## Other Commands

### Creating a README.md File
To create a README.md file:
```sh
echo "# git - course" >> README.md
```
