# Git Commands

## Git Introduction

### What is Git?
Git is a distributed version control system that helps you track your code changes.
When doing a group project, every developer gets their local repository with full commit history. The commit history makes Git fast, as now a network connection is not needed to create commits or perform diffs between commits

### It is used for:
- Tracking code changes
- Tracking who made changes
- Coding collaboration

### What does Git do?
- Manage projects with Repositories
- Clone a project to work on a local copy
- Control and track changes with Staging and Committing
- Branch and Merge to allow for work on different parts and versions of a project
- Pull the latest version of the project to a local copy
- Push local updates to the main project

### What is GitHub?
- GitHub is different from Git.
- GitHub is a popular distributed version control platform to help developers collaborate with each other remotely.
- Developers can share their codes using GitHub.
- You cannot use GitHub without Git but you can use Git without GitHub.

## Different Commands in Git

### Git Basics
```
git init <directory>
```
Create empty Git repo in specified directory. Run with no arguments to initialize the current directory as a git repository

--------------------------------------------------------------------------------------------------------------------------------------------------------

```
git clone <repo>
```
Clone repo located at ```repo``` into local machine. Original repo can be located on the local filesystem or on a remote machine via HTTP or SSH.

-------------------------------------------------------------------------------------------------------------------------------------------------------

```
git config user.name <name>
```
Define author name to be used for all commits in current repo. Devs commonly use --global flag to set config options for current user.

-------------------------------------------------------------------------------------------------------------------------------------------------------

```
git add <directory>
```
Stage all changes in ```directory``` for the next commit. Replace ```directory``` with a ```file``` to change a specific file.

-------------------------------------------------------------------------------------------------------------------------------------------------------

```
git commit -m "<message>"
```
Commit the staged snapshot, but instead of launching a text editor, use ```message``` as the commit message.

-------------------------------------------------------------------------------------------------------------------------------------------------------

```
git status
```
List which files are staged, unstaged, and untracked.

-------------------------------------------------------------------------------------------------------------------------------------------------------

```
git log
```
Display the entire commit history using the default format. For customization see additional options.

-------------------------------------------------------------------------------------------------------------------------------------------------------

```
git diff
```
Show unstaged changes between your index and working directory.

-------------------------------------------------------------------------------------------------------------------------------------------------------

### Undoing Changes
```
git revert <commit>
```
Create new commit that undoes all of the changes made in ```commit```, then apply it to the current branch.

-------------------------------------------------------------------------------------------------------------------------------------------------------

```
git reset <file>
```
Remove ```file``` from the staging area, but leave the working directory unchanged. This unstages a file without overwriting any changes.

-------------------------------------------------------------------------------------------------------------------------------------------------------

```
git clean -n
```
Shows which files would be removed from working directory. Use the -f flag in place of the -n flag to execute the clean

-------------------------------------------------------------------------------------------------------------------------------------------------------

