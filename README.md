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

12. Diff between gir rm and git restore ->
Ans:- if you want to move the whole file back to the untracked  state, then we do 'git rm', otherwise if we just want the changes to be moved in working area or staging area then we use 'git restore'.

13.'git diff commit1 commit2' -> gives the difference of all file changes between two commits.

14. 'git commit -m "<your commit message>" -> if we want to avoid opening of some editor for commit message we can directly send commit message by using this command.

15. 'git remote' -> List down all the remote connection names.

16 Remote connection -> It helps you to link two git repositories for uploading and downloading changes from each otherwise.

17. 'git remote add <name of remote> <link of the remote>' -> this commands helps ush to add a new link to the remote repo and give a name to it.

18. 'git remote rm <name of remote>' -> this command deletes a remote connection.

19.'git remote rename <oldname> <newname'-> this command renames the remote connection.

NOTE:- The name of the remote connection is always used to establish communication between the repos.

20. 'git add <file1> <file2> <file3>' -> this command will add multiple file changes together in the staging area.

21. 'git add . ' -> It adds all file to statging area.

22. 'git pull <remote name> <branch name>' -> downloads latest changes from the branch of the mentioned remote in your local repo.

#### Recommended practice to do.

-make changes
-git add <file>
-git commit
-git pull
-git push

.
.
23.Merge confilicts are a very common scnerio.

merge conflicts can occur if multiple people try to make changes to thr same file and collaborate.