## Git Commands Cheatsheet

### Terms

**Local Repo**: The folder on your computer with the (hidden) .git folder. This is where you will make changes to the files.

**Remote Repo**: The Github server that is accessed through the website.

**Staging**: Preparing files before commit, can be changed easily

**Commit**: Packaged files with message, hard to change contents (that's why check before committing)

### Basic Commands

`git init` - initialize the local git repo

`git config` - manage user account and authentication

`git remote add origin ` - creates a connection to the server based on the git file
> origin -> name of connection (usually named as origin)

> xxxxxxxxxxxx.git -> get link from github (green "Code" button) to establish connection

`git remove origin` - removes the connection "origin"

`git status` - sees the status of the files (staged or not)

`git add` - adds file to staging

`git rm --staged <file name>` - removes the file from staging

`git commit -m "test message"` - commits (packages) the updated files with message
> Note: remember to add message that describes the changes 

`git push origin master` - pushes commit to master branch (irreversible!)

`git pull origin master` - pulls files from master to get latest version of files
> Remember to pull when starting and before committing to prevent clashing errors

### Recommended Workflow
1. `git pull origin master` to get latest version
2. Make necessary changes 
3. git pull again to make sure it will not clash
4. `git add` the changed files
5. check then `git commit -m` with relevant message
6. if all is fine, `git push origin master` to push changes to master branch
7. updated files should be reflected on Github

If there are any commit errors or clashing files, make a backup and try to resolve it.
Try not to work on the same part of a file with another person if not the version of the file will be desynced

If there is any big issues with the remote repo, tell me (isaac) and i will try to fix or rollback if needed.

There are other tricks like using .gitignore files or separate branches it's optional and i'm lazy to explain so go google