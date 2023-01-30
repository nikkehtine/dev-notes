[Basic git commands](https://confluence.atlassian.com/bitbucketserver/basic-git-commands-776639767.html)

## Basic changes
* `git status` - show status 
* `git add <file>` - add files to branch
* `git add *` - add all files to branch
* `git commit -m "Comment"` - commit changes to branch
* `git commit -a` - commit all tracked changes to branch
* `git push origin master` - push changes to *master* branch of remote repo
* `git pull` - pull changes from remote repo
* `git clone /path/to/repo` - clone a repo
* `git clone username@host:/path/to/repo` - clone a remote repo

## Branches
* `git branch` - display all branches and select the one you are operating in
* `git checkout <name>` - go to the branch
* `git checkout -b <name>` - create a branch and go to it
* `git branch -d <name>` - delete the branch
* `git push origin <name>` - send the branch to a remote repository
* `git push -all origin` - send all branches to the remote repository

## Local repositories
* `git init` - new local repo

## Configuring Git
* `git config --global user.name "username"` - add your username
* `git config --global user.email email@example.com` - add your e-mail address