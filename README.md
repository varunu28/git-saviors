# git-saviors
Commands which help me to navigate around git

#### Check the history log for git
```
git reflog
```

#### Set sublime(or your favorite text editor) as default text editor for editing commits
```
git config --global core.editor "subl -n -w"
```

#### Check the history log with timestamp
```
git reflog --date=iso
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

#### Messed Up and want to revert the commit
```
git reset --soft HEAD^ (If you want to keep the changes on local)
git reset --hard HEAD^ (Messed up big time & don't care about the changes)
```

#### Maven commands (Specific to checkstyle project)
```
mvn -Passembly -Dmaven.test.skip=true package
mvn verify
```
