```
git filter-branch --force --index-filter 'git rm --cached --ignore-unmatch "FILE_TO_BE_REMOVED"' --prune-empty --tag-name-filter cat -- --all
git for-each-ref --format='delete %(refname)' refs/original | git update-ref --stdin
git reflog expire --expire=now --all
git gc --prune=now
```
