1. `git init` -> Powers your folder to be managed by git, and initialises a new repository. It is also creates a .git flder that has all the relevant logic to manage versions of your project.

2.  `Working Area` -> there can be a bunch of files that are not currenttly handled by git. It means that changes done or o be done in those files are not managed by git yet. A file which is in wirking area is considered to be not in the staging area. When we do `git status` and we see abuunch of `untracked files` then these are actually called to be in working area.

3.  `Staging area` -> What all files are going to be part of the next version taht we will create. this staging area is the place where git knows what changes will be done from the last vesion to the next version.

4.  `Repository Area` -> This area actually contains the details of all you previous registered version. And the files in this area, git already manages them and knows their version. And the files in this area, git already manages them and knows their version history.

5.  `git add <file>` -> moves file from working area to staging area

6.  `git rm --cached <file>` -> moves file back from staging area to working area

7.  `commit` -> Commit is a particular version of the project. It captures a snapshot of the project's staged changes and creates a version out of it.

8.  `git commit` -> registers staging changes to a commit.

9.  `git log` -> list downs all the commits of the repository. If you want to exit out of git log prompt press `q`.

10.  `git restore <file>` -> it removes all files changes from the staging area to be committed. this can be useful, if we did some dirty piece of code and now no more want it. Instead of deleting every change line by line, we can restore it or you can say restore last clean version of the file.

11.  `git restore --staged <file>` -> it removes file from changes from staging area to working area.this only works if changes are in your staging area.

12. Diff between git rm and it restore
ans: if you want to move the whole file back to the untracked state, then we do git rm, otherwise if we jest want to changes to be moved in working area or stagin area then we git reatore.