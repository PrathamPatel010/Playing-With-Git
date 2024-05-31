Git is a widely used version control system that lets you manage and keep track of your source code history. It allows multiple people to work on the same project without interfering with each other's work. It stores file changes more efficiently and ensures file integrity.

GitHub, on the other hand, is a cloud-based hosting service that lets you manage Git repositories. It provides a central place where developers can store and share their code, collaborate on it, and track its changes.

The fundamental difference between Git and GitHub is that while Git is a version control system that lets you manage and keep track of your source code locally, GitHub is a hosting service for Git repositories. So they are not the same thing: Git is the tool, and GitHub is the service for projects that use Git.

---

`git init` : Powers your folder to be managed by git, and initializes an empty git repository.

It also creates .git folder that has all relevant logic to manage version of your project.

There are 3 area your file can be while using Git VCS: Working, Staging, Repository 

`Working Area` : There can be bunch of files that are not currently handled by git. It means changes that done or to be done in those files are not managed by git yet. A file which is in working area is not considered to be in staging area. 

When we do `git status` and we see bunch of `untracked files` , then these are actually called in the working area.

`Stage Area` : What all files are going to be part of next version that we will create. This area is the place where git knows what all changes will be done from the latest version to next version.

  

`Repository Area` : This area actually contains the details of all your previously registered version. And the files in this area, git already manages them and knows their version history.

`git add <filename>` : Moves file from working area to staging area.

`git rm <filename>` : Moves file back from staging area to working area.

`commit` : It is a particular version of the project. It captures the snapshot of the project’s staged changes and creates version out of it.

`git commit` : Registers staging changes to a commit.

`git log` : Lists down all the commits of the repository. To exit from git logs, just enter `q` .

`git restore <filename>` : It removes all file changes from the staging area to be committed. This can be useful, if we wrote some dirty piece of code and now we don’t want it. Instead deleting every change line-by-line, we can restore it or you can say restore last clear version of the file.

git restore --staged <filename> : To move back files from staged area to working area. So that we can restore the changes made by that file. Because we can’t restore the changes made in staged file, so first we have to move it to working area using this command. Then we can restore the changes.  

This will only works if it is in staging area.

One more Line

`Difference between git rm and git restore` :

→ If we want to move whole file back to untracked state, we can use git rm. We just want the changes to be moved in working area or staging area, we use git restore.

`git diff commit1 commit2` : Gives difference of all file changes between 2 commits.

`git commit -m “commit message”` : To quickly give commit message instead of opening it in vim editor.

`git remote` : Lists down all the remote connection names.

`Remote Connection` : It helps you to link 2 git repositories for downloading and uploading changes from each other.

`git remote add <name of connection> <link of connection>`  : Helps us to add new link to remote repo and give name to it.

`git remote rm <name of remote>` : Deletes a remote connection.

`git remote rename <oldname> <newname>` : Rename the connection. 

Note : Name of remote connection is always used to communication between repos.

`git add <filename1> <filename2>` : To move multiple files to staging area.
`git add .` : To move all files to staging area.
`git pull <remote-name> <branch-name>` : Download all the changes from the branch mentioned remote in your local repo.

# Recommended Practice to do
    - make changes
    - git add <file>
    - git commit -m "<message>"
    - git pull
    - git push

merge conflicts can occur if multiple people try to make changes to same file, then collaborate.