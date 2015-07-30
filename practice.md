# Practical Training

First time git setup: https://git-scm.com/book/en/v2/Getting-Started-First-Time-Git-Setup

## Init new project

```
git init
git add files...
```

## Status

```
git status -s = svn status
```

## Commit

```
git commit -m "Something"
```

## Remotes

```
git remote add origin URL
git push origin master
```

## Git diff

```
$ git diff --staged # sometimes you see: --cached; diff between what you added to the staged area and last commit (HEAD)
$ git diff HEAD # diff with the last commit (HEAD) and your (unstaged) code
$ git diff # diff between the staged files and the unstaged files (not usually what you want).
$ git diff --cached origin/master # What would I push?
```

See: http://images.abizern.org.s3.amazonaws.com/365git/March10/GitDiffSimple.png 

## Log and previous commits

git log
git log -p (patch)
git log --stat
git log --graph
git log --since=yesterday

## Internals

Create empty repo. Create and commit one file. Three objects. Why?
- Inspect objects with "git cat-file -p <SHA1>"

```
git reflog
```
