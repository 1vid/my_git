# Collection of my git combos 
![Alt Text](https://github.com/1vid/my_git/blob/master/samurai.gif)

### Force "git pull" to overwrite local files


First, run a fetch to update branch or [--all] origin/<branch> refs to latest:

```
git fetch [--all]
```

Backup your current branch:
```
git branch backup-<branch> 
```
Then, you have two options:
```
git reset --hard origin/master
```
OR If you are on some other branch:
```
git reset --hard origin/<branch_name>
```
### Update last commit on remote repo

```
git add <file> or .
git commit --amend
git push -f
```
### Set push to different repo

set
```
git remote set-url --push origin git@github.com:<username>/<repository_name>.git
```

check
```
git remote -v
```
### Remove all changes inserts into tree after pull

hide changes
```
git stash
```

[clean](https://git-scm.com/docs/git-clean/2.23.0)
```
git clean -df
```

### Set and checkout branch locally from remote repo

```
git checkout -b <local branch> origin/<remote branch>
```

in my opinion local and remote branches should nemaed same way
