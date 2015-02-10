# Git Reference

* [http://git-scm.com/](Notes from git-scm.com)

## Intro

File Status Lifecycle:
* untracked
* unmodifed - not shown
* modified
* staged

## Config
* git config --global alias.st 'status'
* git config --global alias.ci 'commit'
* git config --global alias.unstage 'reset HEAD --'
* git config --global alias.last 'log -1 HEAD'
* git config --global alias.lg "log --color --graph --pretty=format:'%Cred%h%Creset -%C(yellow)%d%Creset %s %Cgreen(%cr)%C(bold blue)<%an>%Creset' --abbrev-commit"

## Start a project

### Set default pull and push
Run:

* git config branch.master.remote origin
* git config branch.master.merge refs/heads/master

to create in `.git/config`

```
[branch "master"]
        remote = origin
        merge = refs/heads/master
```

## 2.3 Viewing the Commit History

* git log -p -2
* git log -U1 --word-diff
* git log --pretty=oneline
* git log --oneline
* git log --pretty=format:"%h %an : %s" --graph

Filtering:
* git log --grep <commit message>
* git log --author <authorname>
* git log --after=2014-01-01

* gitk

## 2.4 Git Basics - Undoing Things

Change Your Last Commit
* git commit --amend

Anything that is committed in Git can almost always be recovered.

Remove unstaged file. Cannot be recovered:
* git checkout -- <file>


## 2.5 Git Basics - Working with Remotes

* git remote -v
* git remote add [shortname] [url]
* git remote rename pb paul
* git remote rm paul
* git fetch [shortname]
* git fetch origin
* git push [remote-name] [branch-name]

## 2.6 Git Basics - Tagging
lightweight and annotated

* git tag
* git tag -a v1.4 -m 'my version 1.4' (create annotated tag)
* git show v1.4
* git tag v1.4-lw
* git show v1.4-lw
* git tag -a v1.2 -m 'version 1.2' 9fceb02 (tag previous commit)
* git push origin v1.5 (explicitly push tags)
* git push origin --tags

move tag:
* git tag -a v2.56 8bad64f6e9 -f


# What is a Branch

* git branch testing (creates a new pointer at the current commit)
* git log --oneline --graph --decorate
* git log --oneline --all --graph --decorate
* git checkout -b iss53
* git branch -m old_branch_name new_branch_name
* git branch -d hotfix
* git branch --no-merged


## 3.5 Git Branching - Remote Branches

* git push (remote) (branch)
* git push origin serverfix
* git push origin serverfix:anotherremotebranchname
* git fetch origin
* git checkout -b serverfix origin/serverfix
