# GIT: tips and tricks

🧙‍♂️In this repository I am going to add all the tips and tricks for using GIT like a wizard.

## List of common commands

### clone

```
git clone <LINK> 
```

or 

```
git clone <LINK> .
```

or 


```
git clone <LINK> <folder_name>
```

### commit + push

```
git add .
git commit -m "<Message>"
git push
```

### pull

```
git pull
```

### fetch

```
git fetch
```

### checkout

```
git checkout <branch_name>
```

To force it

```
git checkout <branch_name> -f
```

### add remote

```
git remote add origin <LINK>
```



## List of super commands

### Change remote url link


```
git remote set-url origin <LINK>

git remote -v
```

### Merge + Squash

Squash is a nice feature that allows to do a commit collapsing all the history commits in one commit. It is useful when developer do WIP commits.

```
git checkout <branch_name>
git merge --squash <branch_name>
git commit
```

### Create a branch without history

```
git checkout --orphan <name_you_choose_for_orphan_branch>
git commit
```

### Force checkout

All the chances will be replaced by the checkout. 


```
git checkout <branch_name> -f
```

### Disable TLS/SSL verification for a single git command

```
git -c http.sslVerify=false clone <LINK>
```

### Disable SSL verification for a specific repository

```
git config http.sslVerify false
```

Global: 

```
git config --global http.sslVerify false
```

### Merge unrelated histories

```
git pull --allow-unrelated-histories
```

### Compare branches

```
git diff master..staging
```
