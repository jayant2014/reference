# GIT Reference

This reference sheet is for the free Udemy course https://www.udemy.com/course/getting-started-with-git 

## GIT Create

Create a GIT repository or clone an existing repository

### Clone an existing repository

```
$ git clone <repo URL>
```

### Create a new local repository

```
$ git init
```

## GIT Local Changes

Change files locally and commit

### View changed files in your local directory

```
$ git status
```

### Changes to tracked files

```
$ git diff
```

### Add changes for next commit

```
$ git add <filename>
```

### Add all current changes for next commit

```
$ git add .
```

### Changes to tracked files added

```
$ git diff --staged
```

### Commit all previously added local changes

```
$ git commit -a
```

### Commit previously staged changes

```
$ git commit
```

### Commit previously modified changes with comment

```
$ git commit -m "Committing changes"
```

## GIT Branches and Tags

List branches and tags of a repository

### List all existing branches

```
$ git branch -av
```

### Switch HEAD branch

```
$ git checkout <branch>
```

### Create a new branch based on your current HEAD

```
$ git branch <new-branch>
```

### Delete a local branch

```
$ git branch -d <branch>
```

### Mark the current commit with a tag

```
$ git tag <tag-name>
```

### Checkout a tag

```
$ git checkout <tag-name>
```

## GIT Update and Publish

Update the remote repository

### Show information about a remote branch

```
$ git remote show <remote>
```

### Download all changes from remote repository

```
$ git fetch <remote>
```

### Checkout remote repository

```
$ git checkout <remote>
```

### Download all changes from remote repository and merge to HEAD

```
$ git pull <remote> <branch>
```

### Publish local changes to remote

```
$ git push <remote> <branch>
```

### Delete a branch from remote

```
$ git branch -dr <remote/branch>
```

## GIT Merge and Rebase

Merge and rebase branches

### Merge a branch into current HEAD

```
$ git merge <branch>
```

### Rebase current HEAD onto branch

```
$ git rebase <HEAD>
```

### Abort a rebase

```
$ git rebase --abort
```

### Continue rebase after resolving conflicts manually

```
$ git rebase --continue
```

### Resolve conflicts

```
$ git merge <branch>
After auto merge, the conflict files need to be resolved manually.
Then add the resolved file and commit
$ git add <resolved-file>
$ git commit
```

## GIT Undo

Discard local changes in your workspace

### Discard all local changes

```
$ git reset -hard HEAD
```

### Discard local changes to a specific file

```
$ git reset -hard HEAD <filename>
```

### Reset your HEAD to a previous commit and discard all after that

```
$ git reset -hard <commit>
```

### Preserve all changes as unstaged

```
$ git reset <commit>
```

## GIT History

Check the history of commits

### Show all commits in chronological order

```
$ git log
```

### Show change history for a file

```
$ git log -p <filename>
```

### Total change history of a file like who, what and when

```
$ git blame <filename>
```
