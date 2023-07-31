# Carl Tallon Git Commands
All the git commands you'd ever need &amp; their explanation

# git checkout = switch branches
therefore this creates branch and switches to it
```
git checkout -b branchname
```

# git merge targetbranchname
combines two branches 
```
  git merge targetbranchname
```


# git rebase
adds branch commit to end of other branch, makes commits linear
```
git rebase main (when in other branch)
```

# git checkout

You can use HASH name or commit name to checkout commit (detaches head)
```
git checkout c4
```

You can also reference a hash name and look at commits around it 
```
git checkout C4^
```
look at commit in past before this one

```
git checkout HEAD~4
```
look at commit four behind head

# git rebase / reset
git revert - remote
git reset - local

## In use 
```
git rebase -i C5
```
brings up UI to move commits around and omit commits 

# git tag 
```
git tag text C1
```
add tag to commit to show important milestones

# git pull 
``` 
git pull --rebase
``` 
pull from repo but in new branch (rebase)

# If you work on a large team, you generally can't push directly onto the main branch. The solution is to create your own branch locally, make your changes, then push that change to the remote using a pull request. Therefore do :

``` 
git branch feature
git checkout feature
git branch -f main c1
git push 
```
