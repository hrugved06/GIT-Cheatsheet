# Basic GIT Command-line Guide

- Install Git VCS :- [ Click here!](https://git-scm.com/downloads) 

| Description | Commands |
| ----------- | ----------- |
| If you already have Git installed, you can get the latest development version via | `git clone https://github.com/git/git` |
| Git version check | `git --version` |
| Update Git to the latest version on Windows | `git update-git-for-windows` |
| Update Git to the latest version on Linux | `sudo apt-get update` > `sudo apt-get install git` |
| Update Git to the latest version on MacOS | `brew install git` > `brew updrage git`|

---

## First time Setup Configurations

| Description | Commands |
| ----------- | ----------- |
| Setting up Username | `git config --global user.name "Your Name"` |
| Setting up UserEmail | `git config --global user.email "Your Email"` |
| View all your Git settings | `git config --list --show-origin` |

---

## Git directory setup commands

| Description | Commands |
| ----------- | ----------- |
| Initializes a git repository | `git init` |
| Clone a remote repository to local system | `git clone <url>` |

---

## Git Basic Commands to interact with remote repository

| Description | Commands |
| ----------- | ----------- |
| Adds a specific untracked or modified file to the staging area | `git add <filename.extension>` |
| Adds all untracked or modified files to staging area  | `git add -A` or `git add .` |
|Shows status of the files in the directory (untracked/added/modified/deleted/etc.)|`git status`|
|Commits a specific modified or deleted file | `git commit <fileName.extension>`|
| Stages all (a) files automatically that have been modified and deleted | `git commit -a` |
|Stages a commit of with a custom message (m) | `git commit -m 'Message'` |
|Push local commits to the remote repository branch |`git push <alias> <branch>`|
|Push local commits to the remote server |`git push`|

---

With the help of above commands one can do interaction with a remote repository if a proper workflow if followed*.

e.g. Lets say you want to add some feature in your organization's website homepage, what you need to do is fork the repository to your GitHub account the by copying the remote URL `clone` it on your local machine, add the code required for your feature X and stage the changes in the staging area with `git add`, after adding all the changes `commit` the changes with a proper commit message and finally `push` commited changes with a alias on a remote repository branch. Then creating a pull request will ultimately merge the changes to the main repository. Tada! 

- Basic Workflow: 
1. `git clone https://github.com/OSSdeveloper/webExperiments.git`
2. `git add index.html`
3. `git commit -m 'Added feature X'`
4. `git push origin main`.


*Note:- This is an example of very basic workflow, based upon the requirements and changes you do the workflow will vary.

---