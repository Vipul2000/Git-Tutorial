1. 'git init' -> Powers your folders to be managed by git and initialises a new empty repository. It also create a .git folder that has all the relevant logic to manage versions of your projects.


2.'Working area' -> There can be a bunch of files that are not currently handled by git. it means that changes done or to be done in those files are not managed by git yet. A file which is in working area is considered to be not in the staging area. when we do 'git status' and we see bunch of 'untracked files' then these are actually called to be in the working area.


3. 'Staging area' -> what all files are going to be part of the next version that we will create. This staging area is the place where git knows what changes will be done from the last version to the next version.


4. 'repository area' -> This area actually contains the details of all your previous registered version. and the files in this area, git already manages them and knows their version history.


5. 'git add <file>' -> moves file from working area to staging area.

6. 'git rm --cached <file>' -> moves file back from staging area to woking area.

7. 'commit' -> commit is the particular version of the project. It captures a snapshots of  the project's staged changes and creates a version out of it.

8. 'git commit' -> registers staging changes to a commit.

9. 'git log' -> list down all the possible commits of repository. if you want to exit out of 'git log' prompt press 'q'.

10. 'git restore <files>' -> It removes all files changes from the staging area to be committed. this can be useful, if we did some dirty piece of code and no more want it. Instead of deleting every change line by line we can restore it or you can say restore last clean version of the file.

11. 'git restore --staged <file>' -> It removes file from changes from staging area to working area. This only works if changes are in your staging area.