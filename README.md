# my_git is a collection of my combos 

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
