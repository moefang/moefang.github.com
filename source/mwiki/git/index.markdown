---
layout: page
title: "How to Use Git"
date: 2012-09-13 23:16
sidebar: false
comments: false
sharing: true
footer: false
---
### Basic Commonds
Update source and push it to remote
``` sh
git add .
git commit -m 'First commit.'
git push origin remote
```
View branch
``` sh
git branch
```
### Use ssh alias
View file .git/config
``` sh
vim .git/config
``` 
We should modify the **[remote "origin"]** and set `url = ssh://alias/(username)/(gitname)`
We can test
``` sh
ssh -T git@alias
```

