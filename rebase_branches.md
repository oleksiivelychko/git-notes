### Rebase branches.

Merge `hotfix-branch` into `develop-branch`:
```
git pull --rebase origin develop-branch
git push --force
```

If there are conflicts, fix them and:
```
git rebase --continue
```
...or cancel the rebasing action:
```
git rebase --abort
```