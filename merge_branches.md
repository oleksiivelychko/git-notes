### Merge branches.

```
git fetch origin
```
💡 **origin** is a shorthand name for the remote repository that a project was originally cloned from.

```
git checkout develop-branch
git pull
```

_(Optional)_ Recreate local branch from remote:
```
git branch --delete --force develop-branch
git checkout -b develop-branch /origin/develop-branch
```

Merge `hotfix-branch` into `develop-branch`:
```
git merge origin/hotfix-branch --no-ff
```
💡 _no-fast-forward (optional)_ to preserve the history of commits into `develop-branch`.

If there are conflicts, fix them and:
```
git merge --continue
```
...or cancel the merging action:
```
git merge --abort
```

After that - push changes:
```
git push
```

_(Optional)_ Delete remote branch:
```
git push origin --delete origin/hotfix-branch
```