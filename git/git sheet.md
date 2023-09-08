# git sheet

[Basic git commands](https://confluence.atlassian.com/bitbucketserver/basic-git-commands-776639767.html)

## Basic changes

- `git status` - show status
- `git status` - show
- `git add <file>` - add files to branch
- `git add *` - add all files to branch
- `git commit -m "Comment"` - commit changes to branch
- `git commit -a` - commit all tracked changes to branch
- `git push origin main` - push changes to _main_ branch of remote repo
- `git pull` - pull changes from remote repo
- `git clone <path to repo>` - clone a repo
- `git clone username@host:<path to repo>` - clone a remote repo

## Branches

- `git branch` - display all branches and select the one you are operating in
- `git checkout <name>` - go to the branch
- `git checkout -b <name>` - create a branch and go to it
- `git branch -d <name>` - delete the branch
- `git push origin <name>` - send a specific branch to remote repo
- `git push -all origin` - send all branches to remote repo

## Local repositories

- `git init` - new local repo

## Configuring Git

`git config`:

- `--global` - makes changes to your user configuration
- `--local` (or no flag specified) - makes changes to the local repo

### Options

- `git config --global user.name "username"` - add your username
- `git config --global user.email email@example.com` - add your e-mail address
- `git config --global core.autocrlf input` - leaves line endings as they are, commits unix-style line endings
    - this sounds cryptic but it's important to leave unix-style line endings
- GPG signing:
    - `git config --global user.signingkey <GPG key>` - your GPG key for signing commits
    - `git config --global commit.gpgsign` - automatically sign all commits
