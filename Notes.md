What is Git?
-git is a distributed version control system(DVCS).

What is GitHub?
-github is a cloud basedplatform that hosts Git repostories,allowing developers to store,manage,collabrate,and share code from anywhere in the world.

CLone repositary:
-creates a complete local copy of a github repo on ur comp.
Syntax
-git clone <repo_url>

Repositary Status:
-is a cmd helps u monitor the current state of ur repo.
Syntax
-git status

Add Files:
-there two ways to change file from untracked to the staging area those 2 options are,
Syntax
-git add.
-git add filename
from above to ways the stage changes.

Commit:
-this cmd is used to save the staged changes permanetly in ur local git repositary.each commit creates a snapshot of ur project,making it easy to track changes.
Syntax
-git commit -m "message" ,this creates snapshot

Push:
-used to upload local commits from a git repositary to a remote repositary,such as git hub.
Syntax
-git push 
-git push origin main

Pull:
-this cmd downloads the latest changes froom a remote repo and automatically merges them into ur current local branch.
Syntax
-git pull 
-git pull origin main

Fetch:
-this cmd is used to download the latest changes from a remote repo without merging them into ur current branch.
Syntax
-git fetch origin,downloads changes without merging.

Create Branch:
-A branch in git is an independent line of development.it allows developers to work on new features.
Syntax
-git branch new branch name
-git checkout -b new branch name
-git checkout new branch name and old branch name

PS D:\BCA\Git & GitHub Workshop> git branch      
* bug
  master
PS D:\BCA\Git & GitHub Workshop> git checkout -b feature
Switched to a new branch 'feature'
PS D:\BCA\Git & GitHub Workshop> 

Switch Branch:
Syntax
-git switch branchname
-git checkout branchname,are used to move between branches.

Merge Branch:
-git merge cmd combines changes from 1 branch into another.
Syntax
-git checkout main
-git merge branchname,resolves conflict if needed.

Checkout:
-cmd used to switch between the branches or move to a specific commit in a repo,and to create a new branch.
-git checkout <branch>
-git checkout <commit>,this switches branches or inspect commits.

Reset:
-used to move the current branch to a previous commit.
Syntax
-mixed reset: git reset <hashid>
-soft reset:git reset --soft <hashid>
-hard reset:git reset --hard <hashid>

Revert:
-cmd is used to undo changes.
Syntax
-git revert <commit>

Cherry-pick:
-git cherry-pick cmd used to a copy a specific commit from 1 branch and apply to another branch.
Syntax
-git cherry-pick <commit>

Stach
-git stach cmd temporarily saves uncommitted changes and restores the wirking directory to clean a state.
-to see changes, git stash apply

Cmds:
 git config --global user.name "name"
 git config --global user.email "email"
 git init
 git status
 
 <cms to run in terminal:>
 PS D:\BCA\Git & GitHub Workshop> git init
PS D:\BCA\Git & GitHub Workshop>  git config --global user.email "tanushmuddapur@gmail.com"
PS D:\BCA\Git & GitHub Workshop> git init                                                  
PS D:\BCA\Git & GitHub Workshop> git status
PS D:\BCA\Git & GitHub Workshop> git add cmd.py
PS D:\BCA\Git & GitHub Workshop> git status    
PS D:\BCA\Git & GitHub Workshop> git add.  
PS D:\BCA\Git & GitHub Workshop> git add .
PS D:\BCA\Git & GitHub Workshop> git status
PS D:\BCA\Git & GitHub Workshop> git commit -m "intial commit "
PS D:\BCA\Git & GitHub Workshop> git status                    
PS D:\BCA\Git & GitHub Workshop> git log   
commit 01bfd0adbf5e2fb269455e53a77a66bca01ed700 (HEAD -> master)
Author: Tanushmuddapur <tanushmuddapur@gmail.com>
Date:   Fri Jul 31 14:58:51 2026 +0530

    intial commit
PS D:\BCA\Git & GitHub Workshop> git remote add origin https://github.com/Tanushmuddapur/Git-GitHub-Workshop.git
PS D:\BCA\Git & GitHub Workshop> git push -u origin main
error: src refspec main does not match any
error: failed to push some refs to 'https://github.com/Tanushmuddapur/Git-GitHub-Workshop.git'
PS D:\BCA\Git & GitHub Workshop> git push -u origin main
error: src refspec main does not match any
error: failed to push some refs to 'https://github.com/Tanushmuddapur/Git-GitHub-Workshop.git'
PS D:\BCA\Git & GitHub Workshop> git push -u origin main
error: src refspec main does not match any
error: failed to push some refs to 'https://github.com/Tanushmuddapur/Git-GitHub-Workshop.git'
PS D:\BCA\Git & GitHub Workshop> git branch
>> 
* master
PS D:\BCA\Git & GitHub Workshop> git push -u origin main
error: src refspec main does not match any
error: failed to push some refs to 'https://github.com/Tanushmuddapur/Git-GitHub-Workshop.git'
PS D:\BCA\Git & GitHub Workshop> git push -u origin main
error: src refspec main does not match any
error: failed to push some refs to 'https://github.com/Tanushmuddapur/Git-GitHub-Workshop.git'
PS D:\BCA\Git & GitHub Workshop> git push -u origin master
info: please complete authentication in your browser...
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 12 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (4/4), 1.32 KiB | 1.32 MiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/Tanushmuddapur/Git-GitHub-Workshop.git
 * [new branch]      master -> master
branch 'master' set up to track 'origin/master'.
PS D:\BCA\Git & GitHub Workshop> git status               
On branch master
Your branch is up to date with 'origin/master'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   Notes.md
        modified:   cmd.py
        modified:   std.txt

no changes added to commit (use "git add" and/or "git commit -a")
PS D:\BCA\Git & GitHub Workshop> git add .
PS D:\BCA\Git & GitHub Workshop> git status
On branch master
Your branch is up to date with 'origin/master'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   Notes.md
        modified:   cmd.py
        modified:   std.txt

PS D:\BCA\Git & GitHub Workshop> git commit -m "feat:new line added"
[master 7c7e110] feat:new line added
 3 files changed, 7 insertions(+), 1 deletion(-)
PS D:\BCA\Git & GitHub Workshop> git push
Enumerating objects: 9, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 12 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (5/5), 419 bytes | 419.00 KiB/s, done.
Total 5 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/Tanushmuddapur/Git-GitHub-Workshop.git
   01bfd0a..7c7e110  master -> master
PS D:\BCA\Git & GitHub Workshop> git branch
* master
PS D:\BCA\Git & GitHub Workshop> git branch bug
PS D:\BCA\Git & GitHub Workshop> git branch    
  bug
* master
PS D:\BCA\Git & GitHub Workshop> git checkout branch
error: pathspec 'branch' did not match any file(s) known to git
PS D:\BCA\Git & GitHub Workshop> git branch         
  bug
* master
PS D:\BCA\Git & GitHub Workshop> git checkout bug
PS D:\BCA\Git & GitHub Workshop> git branch      
* bug
  master
PS D:\BCA\Git & GitHub Workshop> git checkout -b feature
PS D:\BCA\Git & GitHub Workshop> git checkout bug2      
error: pathspec 'bug2' did not match any file(s) known to git
PS D:\BCA\Git & GitHub Workshop> git checkout main
error: pathspec 'main' did not match any file(s) known to git
PS D:\BCA\Git & GitHub Workshop> git checkout master
PS D:\BCA\Git & GitHub Workshop> git checkout bug2  
PS D:\BCA\Git & GitHub Workshop> git branch bug2        
PS D:\BCA\Git & GitHub Workshop> git branch bug2 bug
PS D:\BCA\Git & GitHub Workshop> git branch             
  bug
* bug2
  feature
  master
PS D:\BCA\Git & GitHub Workshop> git push --set -upstream origin bug2
PS D:\BCA\Git & GitHub Workshop> git push -u origin bug
PS D:\BCA\Git & GitHub Workshop> git push -u origin feature
PS D:\BCA\Git & GitHub Workshop> git branch bug2
PS D:\BCA\Git & GitHub Workshop> git branch bug2 bug
PS D:\BCA\Git & GitHub Workshop> git branch         
PS D:\BCA\Git & GitHub Workshop> git push -u origin bug2   