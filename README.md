
1. "git init" --> powers your folder to be managed by git, and initialises a new empty repo. 
It also creates a .git folder that has all the relevant logic to manage versions of your project.

2. "Working Area" -> there can be a bunch of files that are not currently handled by git
IT means that changes done or to be done in those files are not managed by git. A file which is in working 
area is considered to be not in staging area. When we er do "git status"
and we see abunch if 'untracked files' than these are actually called to be in the working area.

3. "Staging Area" -> what all files are going to be part of the next version that we will create.
This staging area is the place where git knows what changes will be done from the last version to the next version.

4. "Repository Area" --> this area actually contains the details of all your previous registered versions 
and the files in this area, git already manages them and knows their version history.

5. 'git add <file>'--> moves file from working area to staging area
'git rm --cached <file>'--> moves file from staging to working area

6. 'commit' --> commit is a particular version of the project. It captures a snapshot of the project's staged changed and creates a version out of it.

7. 'git commit' --> applies commit
** use git commit -m "comment" -> if you dont want to open vim/nano editor and want to directly commit


8. "git log" --> lists down all the commits of the Repository. if you waant
to get out of the git log press q


9. "git restore <file>" --> it removes all the changes 

10. ** after commiting the changes you make in the repo, you have to use git add <file> in order to move the changes from working to staging area and 
now when you use git restore <file> it wont delete anything

11. "git restore --staged <file>" --> it removes file changes from the staging area to thw wworking area.
this only works if changes are in staging area

**diff bw git rm and git restore --> if you want to play bw working and staging area than you use restore but we use rm if want to remove the whole file in untracked files meaning 


11. "git remote add <name of remote> <link of the relevant>" -->  this command helps us to add a new link to the remote repo 
and give a name to it

12. "git remote rm <name of remote>" --> this command deletes a remote connection

13. "git remote rename <oldname> <rename> --> this command renames the remote connection

** the name of the remote connection is used to establish communication between repos


14. "git add <file1> <file2> <file3> --> this command will add multiple file changes together to the staging area

15. "git add ." --> this command add all files from working repo to the staging area

16. "git pull <remote name> <branch name>" --> downloads latest changes from the branch of the remote repo in your local repo

### RECOMMENDED PRACTICE TO DO
- make changes
- git add <file>
- git commit
- git pull
- git push

beacuse if you have some changes in working/staging directory and you use git pull it will show error, so you have to first commit your changes and than pull