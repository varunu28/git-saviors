# git-saviors
Commands which help me to navigate around git

#### Check the history log for git
```
git reflog
```

#### Undo a rebase/squash 
```
git reset --hard HEAD@{N}

Replace N with the log number as shown in reflog
```

#### Shows a clear description of all the commits in a git repository
```
git log --pretty=oneline
```

#### Rebase to master and get the forked repo in sync from local
```
git pull --rebase main master
git push -f
```
