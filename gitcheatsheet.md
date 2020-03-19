# Git Cheat Sheet: Chapter 2 Git Bassics #
## Create a Git Repository ##

###git 
used as the begginig of the command.
###git init 
it creates an empty subdirectory in format .git .
###git add *.c
add a file content to the repository index.
###git commit 
it record changes in the repository.
###git clone<url>
creates a copy of an existing Git repository.

## Recording changes to the repository ##

###git status
used to determine which files are in which state.
###git status README
order to begin tracking a new filE.
###git reset HEAD <file>
to remove files from stage
###git add CONTRIBUTING.md
used it to begin tracking new files, to stage files, and to do other things
###git status -s or git status --short
a way to see changes in a more compact way.
###git diff
to see what you’ve changed but not yet staged
###git diff --staged
to see what it has been staged and will go into your next commit.
###git diff --cached
to see what you’ve staged so far 
###git commit
record changes to the repository
###git commit -m
create a commit message inline.
###git rm 
Remove files from the working tree and from the index
###git rm --cached README
clear your cache easily
###git rm log/\*.log
remove the file of your directory
###git mv file_from file_to
Move or rename a file.

## Git Basics - Viewing the Commit History ##

###git log
show commit logs
###git log --stat
code review or to quickly browse
###git log -p -2
limit the number of log entries displayed
###git log --pretty=oneline
hanges the log output to formats other than the default
###git log --pretty=format:"%h %s" --graph
adds a nice little ASCII graph showing your branch and merge history
###git log -S function_name
shows only those commits that changed the number of occurrences of that string.

## Undoing Things ##

###git commit --amend
make the additional changes you forgot, stage them, and commit again

## Working with Remotes ##

###git remote
to see which remote servers you have configured
###git remote add <shortname> <url>
to add a new remote Git repository as a shortname you can reference easily
###git fetch pb
if you want to fetch all the information but that don’t yet have in your repository
###git fetch <remote>
to get data from your remote projects
###git push origin master
loned from a server to which you have write access and if nobody has pushed in the meantime

## Tagging ##

###git tag 
Create, list, delete or verify a tag object signed with GPG
###git tag -a
to specify a command
###git push
Update remote refs along with associated objects
###git push origin <tagname>
explicitly push tags to a shared server 
###git tag -d <tagname>
To delete a tag on a local repository

## Git Aliases ##

###git config
Set up an alias for each command
###git config --global alias.unstage 'reset HEAD --'
creating commands that you think should exist
###git config --global alias.visual '!gitk'
to demostrate by aliasing

##GIT BRANCHING##

###git branch <testing>
creates a new branch.
###git log --one line --decorate
show us where the branch pointers are pointing.
###git checkout <testing> 
switch an existing branch.
###git checkout master
switch back to the master branch.
###git log --oneline --decorate --graph --all
it will print out the history of your commits, where your branch pointers are and how your history has diverged.


###git checkout -b <iss53>
creates a new branch and switch it at the same time.
###git merge <hotfix
merges the branch back into your master branch to deploy to production.
###git branch -d <hotfix>
deletes the hotfix branch.
###git mergetool
graphical tool to solve problems.


###git branch
List, create, or delete branches.
###git branch -v 
to see the last commit on each branch.
###git branch --merged
to see which branchs are already merged.
###git branch --no-merged
 to see which branchs haven't yet merged.
###git branch -vv"
to see what tracking branches you have set up.
###git fetch --all; git branch -vv
If you want totally up to date ahead and behind numbers, you’ll need to fetch from all your remotes right before running this. 
###git push origin --delete <serverflix>
to delete a remote branch/pointer from the server. 
###git rebase master Reapply
commits on top of another base tigit rebase --onto maste take changes on client that aren't on server and replay them on your master branch.
###git rebase master server
rebase the server branch onto the master branch.
 
