---
layout: post
title:  "Git Aliases"
categories: git
---

These are the Git Aliases I use to help me do the day to day.

Git add-alias
```

git config --global alias.add-alias '!f() { git config --global alias.$1 $2; }; f'

```

Standard Git Aliases
```
git st == git status
git co == git checkout
git cm == git commit
git df == git diff
```

Git alias
```
git alias == git config --global -l
```

Always will be adding to this page as a central point for my own reference :)
