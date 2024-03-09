git clone
ls
mkdir repp
touch a1.txt
cd repp
git init
touch f1.txtnew file
vl f1.txt ro write the changes
gid add f1.txt - to track the file
git commit -m"f1 file is created"
git log -to check the commit
git remote add origin"url"
git remote -v -to check if i created a remote rep or not
git push -u origin 
 2
git branch 
git branch a1
git checkout a1
git branch -d "branch name u want to delete"
git merge






# demoo-file
lets try
Git Commands
============

## Translated Versions
- [Versão em português](READMEpt.md)
- [Versión en español](READMEes.md)
- [Türkçe versiyon](READMEtr.md)
- [বাংলা সংস্করণ](READMEbn.md)
- [हिन्दी अनुवाद](READMEhi.md)
- [العربية](READMEar.md)

___

_A list of my commonly used Git commands_

*If you are interested in my Git aliases, have a look at my `.bash_profile`, found here: https://github.com/joshnh/bash_profile/blob/master/.bash_profile*

--

### Getting & Creating Projects

| Command | Description |
| ------- | ----------- |
| `git init` | Initialize a local Git repository |
| `git clone ssh://git@github.com/[username]/[repository-name].git` | Create a local copy of a remote repository |

### Basic Snapshotting

| Command | Description |
| ------- | ----------- |
| `git status` | Check status |
| `git add [file-name.txt]` | Add a file to the staging area |
| `git add -A` | Add all new and changed files to the staging area |
| `git commit -m "[commit message]"` | Commit changes |
| `git rm -r [file-name.txt]` | Remove a file (or folder) |

### Branching & Merging

| Command | Description |
| ------- | ----------- |
| `git branch` | List branches (the asterisk denotes the current branch) |
| `git branch -a` | List all branches (local and remote) |
| `git branch [branch name]` | Create a new branch |
| `git branch -d [branch name]` | Delete a branch |
| `git push origin --delete [branch name]` | Delete a remote branch |
| `git checkout -b [branch name]` | Create a new branch and switch to it |
| `git checkout -b [branch name] origin/[branch name]` | Clone a remote branch and switch to it |
| `git branch -m [old branch name] [new branch name]` | Rename a local branch |
| `git checkout [branch name]` | Switch to a branch |
| `git checkout -` | Switch to the branch last checked out |
| `git checkout -- [file-name.txt]` | Discard changes to a file |
| `git merge [branch name]` | Merge a branch into the active branch |
| `git merge [source branch] [target branch]` | Merge a branch into a target branch |
| `git stash` | Stash changes in a dirty working directory |
| `git stash clear` | Remove all stashed entries |

### Sharing & Updating Projects

| Command | Description |
| ------- | ----------- |
| `git push origin [branch name]` | Push a branch to your remote repository |
| `git push -u origin [branch name]` | Push changes to remote repository (and remember the branch) |
| `git push` | Push changes to remote repository (remembered branch) |
| `git push origin --delete [branch name]` | Delete a remote branch |
| `git pull` | Update local repository to the newest commit |
| `git pull origin [branch name]` | Pull changes from remote repository |
| `git remote add origin ssh://git@github.com/[username]/[repository-name].git` | Add a remote repository |
| `git remote set-url origin ssh://git@github.com/[username]/[repository-name].git` | Set a repository's origin branch to SSH |

### Inspection & Comparison

| Command | Description |
| ------- | ----------- |
| `git log` | View changes |
| `git log --summary` | View changes (detailed) |
| `git log --oneline` | View changes (briefly) |
| `git diff [source branch] [target branch]` | Preview changes before merging |






To initialize a new Git repository in a directory, create a new file, add it to the staging area, and commit 
the changes with an appropriate commit message, follow these steps:
1. Open your terminal and navigate to the directory where you want to create the Gitrepository.
2. Initialize a new Git repository in that directory:
$ git init
3. Create a new file in the directory. For example, let's create a file named "my_file.txt."You can 
use any text editor or command-line tools to create the file.
4. Add the newly created file to the staging area. Replace "my_file.txt" with the actualname of
your file:
$ git add my_file.txt
This command stages the file for the upcoming commit.
5. Commit the changes with an appropriate commit message. Replace "Your commitmessage
here" with a meaningful description of your changes:
$ git commit -m "Your commit message here"
Your commit message should briefly describe the purpose or nature of the changes you made.For
example:
$ git commit -m "Add a new file called my_file.txt"
After these steps, your changes will be committed to the Git repository with the provi

2-To create a new branch named "feature-branch," switch to the "master" branch, and mergethe
"feature-branch" into "master" in Git, follow these steps:
1. Make sure you are in the "master" branch by switching to it:
$ git checkout master
2. Create a new branch named "feature-branch" and switch to it:
$ git checkout -b feature-branch
This command will create a new branch called "feature-branch" and switch to it.
3. Make your changes in the "feature-branch" by adding, modifying, or deleting files asneeded.
4. Stage and commit your changes in the "feature-branch":
$ git add .
$ git commit -m "Your commit message for feature-branch"
Replace "Your commit message for feature-branch" with a descriptive commit message forthe
changes you made in the "feature-branch."
5. Switch back to the "master" branch:
$ git checkout master
6. Merge the "feature-branch" into the "master" branch:
$ git merge feature-branch
This command will incorporate the changes from the "feature-branch" into the "master"branch.
Project Management with Git BCS358C
Department of Computer Science and Engineering, Sir MVIT Page | 16
Now, your changes from the "feature-branch" have been merged into the "master" branch.Your
project's history will reflect the changes made in both bran

3-To create a new branch named "feature-branch," switch to the "master" branch, and mergethe
"feature-branch" into "master" in Git, follow these steps:
1. Make sure you are in the "master" branch by switching to it:
$ git checkout master
2. Create a new branch named "feature-branch" and switch to it:
$ git checkout -b feature-branch
This command will create a new branch called "feature-branch" and switch to it.
3. Make your changes in the "feature-branch" by adding, modifying, or deleting files asneeded.
4. Stage and commit your changes in the "feature-branch":
$ git add .
$ git commit -m "Your commit message for feature-branch"
Replace "Your commit message for feature-branch" with a descriptive commit message forthe
changes you made in the "feature-branch."
5. Switch back to the "master" branch:
$ git checkout master
6. Merge the "feature-branch" into the "master" branch:
$ git merge feature-branch
This command will incorporate the changes from the "feature-branch" into the "master"branch.
Project Management with Git BCS358C
Department of Computer Science and Engineering, Sir MVIT Page | 16
Now, your changes from the "feature-branch" have been merged into the "master" branch.Your
project's history will reflect the changes made in both bran
