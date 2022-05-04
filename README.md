# Git workshop

Instructions and commands for git workshop.

This repo includes [aliases.sh](aliases.sh) file with handy git aliases that are extremely useful when doing things presented in this workshop.

# Basics

```
git pull
git fetch

git status
git diff
git diff --cached

git reset
git reset --hard
git reset --soft HEAD~<number of commits>

git checkout content.txt
```

# Branches and commits

```
git checkout -b my-new-branch
git checkout master
git checkout -
git add --all
git commit -am "commit message"
```

# Stash

```
git stash
git stash pop
git stash apply
```

# Logging

```
git log
git log --oneline | head -n <number of commits>
git log --graph --all
git log --graph --oneline --all
```

# Rebasing

```
git rebase --onto <commit hash>
git rebase -i HEAD~<number of commits>
```

# Troubleshooting detached HEAD

1. Checkout other branch => loose all changes
2. Stash changes, checkout other branch, pop the stash => keep changes
3. Checkout new branch, commit, push => keep changes and commits
