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