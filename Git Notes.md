# Git Notes
## Innit
* Initialises Git repo
```
$ git init 
```
## Clone
* Clone a repository into a new directory. After cloning, git automatically adds that remote repository under the name “origin”.
```
$ git clone <url>
```
---
## Status
* Get the list of files staged and those that haven't been yet
```
$ git status 
```
## Log
* Get history of local repo
```
$ git log
```
* See commits that haven't been pushed to origin
```
$ git log origin/master..master
```
## Add
* Add modified files to stage
```javascript   
$ git add . 
```
## Commit
* Add staged files to local repo
```
$ git commit
```
---
## Fetch
* Download objects and refs from another repository. It does not merge any code into actual branch.
```
$ git fetch
```
## Checkout
* Update the index and update files to match that "branch_name" state
```
$ git checkout "branch_name"
```
* Create a branch and checkout that branch
```
$ git checkout -b "branch_name"
```
* Checkout specific commit using SHA1 identifier. Moves HEAD pointer to that commit
```
$ git checkout <SHA1>
```
---
## Branch
* Create a new branch
```
$ git branch "branch_name"
```
* Delete local branch
```
$ git branch -d "branch_name"
```
---
## Remote
* Check which remotes you have configured
```
$ git remote
```
* Check which remotes URLs
```
$ git remote -v
```
* Add a remote
```
$ git remote add <shortname> <url>
```
* Inspecting a remote
```
$ git remote show <remote>
```
* Renaming a remote
```
$ git remote rename <remote_name> <remote_new_name>
```
* Deleting a remote
```
$ git remote remove <remote_to_remove>
```
## Push
* Sending your code to the remote repo.
```
$ git push <remote> <branch>
```

## Reset
* Reset branch to origin state (removing commits)
```
$ git fetch origin
$ git reset --hard origin/master
```