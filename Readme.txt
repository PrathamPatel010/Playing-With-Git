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