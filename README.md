# Git-best-practices
Git best practices for devloppers

### Get changes from origin 
How to see the changes that were pulled on a `git pull`
```sh
$ git fetch
[...]
From github.com:blah
   00f82fa..38e4017  master     -> origin/master
```

```sh
$ git log HEAD..origin
commit 38e4017bc89a6eb41252465cbde68f7d897377cb
Author: Werner Robitza
Date:   Tue Jul 12 10:56:49 2011 -0700

    Edited Gemfile via GitHub
```

```sh
$ git merge origin
```
### Show changes in a commit

```sh
$ git show <COMMIT>
```

### Check if pull needed in Git

To bring your remote refs up to date

```sh
$ git remote update
```
Check if the branch you are tracking is ahead

```sh
$ git status -uno
```
