Change repository URL:
```
git remote set-url origin https://git-repo/new-repository.git
```

Make a commit in the past:
```
git commit --date="10 day ago" -m "10 days ago changes" 
```

Reset repository to remote state:
```
git fetch origin && git reset --hard origin/main
```

Undo commit(-s):
```
git reset HEAD~1 && git push -f
```

Prettify git log output:
```
git log --pretty=oneline --abbrev-commit
```