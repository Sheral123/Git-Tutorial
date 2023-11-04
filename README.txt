
"git init" --> powers your folder to be managed by git, and initialises a new empty repo. 
It also creates a .git folder that has all the relevant logic to manage versions of your project.

"Working Area" -> there can be a bunch of files that are not currently handled by git
IT means that changes done or to be done in those files are not managed by git. A file which is in working 
area is considered to be not in staging area. When we er do "git status"
and we see abunch if 'untracked files' than these are actually called to be in the working area.

"Staging Area" -> what all files are going to be part of the next version that we will create.
This staging area is the place where git knows what changes will be done from the last version to the next version.

"Repository Area" --> this area actually contains the details of all your previous registered versions 
and the files in this area, git already manages them and knows their version history.

'git add <file>'--> moves file from working area to staging area
'git rm --cached <file>'--> moves file from staging to working area

'commit' --> commit is a particular version of the project. It captures a snapshot of the project's staged changed and creates a version out of it.

'git commit' --> applies commit
** use git commit -m "comment" -> if you dont want to open vim/nano editor and want to directly commit


git log --> lists down all the commits of the Repository. if you waant
to get out of the git log press q

git restore <file> --> it removes all the changes 

** after commiting the changes you make in the repo, you have to use git add <file> in order to move the changes from working to staging area and 
now when you use git restore <file> it wont delete anything


git restore --staged <file> --> it removes file changes from the staging area to thw wworking area.
this only works if changes are in staging area

diff bw git rm and git restore --> if you want to play bw working and staging area than you use restore but we use rm if want to remove the whole file in untracked files meaning 












