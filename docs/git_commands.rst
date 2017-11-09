Popular Git commands and how they are used.
--------------------------------------------

* git config --global user.name "Sam Smith"

 git config --global user.email sam@example.com : It configures the author name and email to be used with the commits.

* git init: Initializes a git repository locally.

* git clone username@host/path_to_repo : Creates a copy of the remote repository to your local machine.
* git add * : adds all the unstaged files to the staging area.
* git add <filename> : adds  a specific unstaged file to the staging area.
* git commit -m "Commit message": commits changes to the head of the local repository instead of the remote.
* git commit -a :adds all the files that are in the staging area and all any file changed since then.
* git push origin master : pushes the changes made to the remote repository.
* git status: list all the files you have made changes to.
* git remote add origin <server> : adds the a link to the remote repository to be able to make changes to it.
* git remote -v : list all the currently configured remote repositories.
* git checkout -b <branchname> : creates a branch and switches to it.
* git checkout <branchname> : switches in between branches.
* git branch : lists all the branches in your repository and tells you the branch you are currently working on.
* git branch -a: List all remote or local branches
* git branch -d <branchname> : deletes the feature branch.
* git push origin <branchname> : pushes your branch to remote repository.
* git push --all origin : Pushes all your local branches to the remote repository.
* git push origin : <branchname> : Deletes a branch in your remote repository.
* git pull :  fetch and merge changes in your remote repository to your working repository.
* git merge <branchname> : To merge work in another branch to your working branch.
* git rm : Removes files from your index and your working directory so they will not be tracked.
* git diff: Generates patch files or statistics of differences between paths or files in your git repository, or your index or your working directory.
* git archive : Creates a tar or zip file including the contents of a single tree from your repository.
* git gc: Garbage collector for your repository. Optimizes your repository.
* git fsck: Does an integrity check of the Git file system, identifying corrupted objects.
* git prune : Removes objects that are no longer pointed to by any object in any reachable branch.

**Updates from remote repository**

* git diff : Views all the merge conflict.
* git diff --base <filename> : view the conflicts against a base file.
* git diff <sourcebranch> <targetbranch> : previews changes before merging.
* git add <filename> : After resolving the merge conflicts mark the file.
* git tag 1.0.0 <commitID> : You can use a a tag to mark a significant change like a release.
* git push --tags origin : Pushes all the local tags to the remote repository.
* git log : It lists all the commits.

**undoing local changes**

* git checkout -- <filename> : replaces the changes in your local tree to the local content in the head.
* git fetch origin, git reset --hard origin/master : Instead, to drop all your local changes and commits, fetch the latest history from the server and point your local master branch at it, do this.
* git reset --hard HEAD : Resets your index and working directory to the state of your last commit.
* git grep "folder" : searches the working directory.