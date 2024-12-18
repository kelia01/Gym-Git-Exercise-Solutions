# Gym-Git-Exercise-Solutions
 
 ## Bundle 1

 ### Exercise 1

 ```bash
 `git init`
Initialized empty Git repository in /Users/gymumutuzo/git-bundleOne/.git/
gymumutuzo@Umutuzos-iMac git-bundleOne % `git branch`
gymumutuzo@Umutuzos-iMac git-bundleOne % `git status`
On branch main

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        readme.md

nothing added to commit but untracked files present (use "git add" to track)
gymumutuzo@Umutuzos-iMac git-bundleOne % `git branch -M master`
gymumutuzo@Umutuzos-iMac git-bundleOne % `git branch -M main`
gymumutuzo@Umutuzos-iMac git-bundleOne % `git status`
On branch main

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        readme.md

nothing added to commit but untracked files present (use "git add" to track)
gymumutuzo@Umutuzos-iMac git-bundleOne % `git add readme.md`
gymumutuzo@Umutuzos-iMac git-bundleOne % `git commit -m "This is for exercise 1"`
[main (root-commit) b1b457c] This is for exercise 1
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 readme.md
gymumutuzo@Umutuzos-iMac git-bundleOne % git remote add origin https://github.com/kelia01/git-bundleOne.git
gymumutuzo@Umutuzos-iMac git-bundleOne % git push
fatal: The current branch main has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin main

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

gymumutuzo@Umutuzos-iMac git-bundleOne % `git push --set-upstream origin main`
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 229 bytes | 229.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/kelia01/git-bundleOne.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.
gymumutuzo@Umutuzos-iMac git-bundleOne % `git checkout -b dev`
Switched to a new branch 'dev'
gymumutuzo@Umutuzos-iMac git-bundleOne % `git checkout -b test`
Switched to a new branch 'test'
gymumutuzo@Umutuzos-iMac git-bundleOne % `git checkout dev`
Switched to branch 'dev'
gymumutuzo@Umutuzos-iMac git-bundleOne % `git branch -D test`
Deleted branch test (was b1b457c).
gymumutuzo@Umutuzos-iMac git-bundleOne % `git checkout -b test` 
Switched to a new branch 'test'
gymumutuzo@Umutuzos-iMac git-bundleOne % `git push origin dev`
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote: 
remote: Create a pull request for 'dev' on GitHub by visiting:
remote:      https://github.com/kelia01/git-bundleOne/pull/new/dev
remote: 
To https://github.com/kelia01/git-bundleOne.git
 * [new branch]      dev -> dev
gymumutuzo@Umutuzos-iMac git-bundleOne % `git push origin test`
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote: 
remote: Create a pull request for 'test' on GitHub by visiting:
remote:      https://github.com/kelia01/git-bundleOne/pull/new/test
remote: 
To https://github.com/kelia01/git-bundleOne.git
 * [new branch]      test -> test
gymumutuzo@Umutuzos-iMac git-bundleOne % `git checkout dev`
Switched to branch 'dev'
gymumutuzo@Umutuzos-iMac git-bundleOne % `git push origin --delete test`
To https://github.com/kelia01/git-bundleOne.git
 - [deleted]         test```
 
  ## Bundle 1

 ### Exercise 2 

[git-bundleOne](https://github.com/kelia01/git-bundleOne.git)

 gymumutuzo@Umutuzos-iMac git-bundleOne % 
 `git stash list` # show a list of all your stashes 
stash@{0}: WIP on dev: 2584dba Add exercise 2 trial
stash@{1}: WIP on dev: 2584dba Add exercise 2 trial
gymumutuzo@Umutuzos-iMac git-bundleOne % 
`git stash clear` #deletes all stashes in your repository
gymumutuzo@Umutuzos-iMa`c git-bundleOne % git stash list 
gymumutuzo@Umutuzos-iMac git-bundleOne % 
`git add home.html` #stages the file
gymumutuzo@Umutuzos-iMac git-bundleOne % 
`git stash push` #stash home.html
Saved working directory and index state WIP on dev: 2584dba Add exercise 2 trial
gymumutuzo@Umutuzos-iMac git-bundleOne % git stash list   
stash@{0}: WIP on dev: 2584dba Add exercise 2 trial
gymumutuzo@Umutuzos-iMac git-bundleOne % 
`git stash pop` #removes the most recent stash
On branch dev
Changes not staged for commit:
  (use "git add/rm <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        deleted:    about.html
        modified:   home.html
        modified:   readme.md
        deleted:    team.html

no changes added to commit (use "git add" and/or "git commit -a")
Dropped refs/stash@{0} (c066a7d16fd76f790504833b3c515839737ed1ce)
gymumutuzo@Umutuzos-iMac git-bundleOne % git stash list 
gymumutuzo@Umutuzos-iMac git-bundleOne % git stash clear
gymumutuzo@Umutuzos-iMac git-bundleOne % 
`git add home.html`
gymumutuzo@Umutuzos-iMac git-bundleOne % 
`git stash push home.html`
Saved working directory and index state WIP on dev: 2584dba Add exercise 2 trial
gymumutuzo@Umutuzos-iMac git-bundleOne % git stash list
stash@{0}: WIP on dev: 2584dba Add exercise 2 trial
gymumutuzo@Umutuzos-iMac git-bundleOne % 
`git add about.html`
gymumutuzo@Umutuzos-iMac git-bundleOne % 
`git stash push about.html`
Saved working directory and index state WIP on dev: 2584dba Add exercise 2 trial
gymumutuzo@Umutuzos-iMac git-bundleOne % git stash list           
stash@{0}: WIP on dev: 2584dba Add exercise 2 trial
stash@{1}: WIP on dev: 2584dba Add exercise 2 trial
gymumutuzo@Umutuzos-iMac git-bundleOne % 
`git add team.html`        
gymumutuzo@Umutuzos-iMac git-bundleOne % 
`git stash push team.html `
Saved working directory and index state WIP on dev: 2584dba Add exercise 2 trial
gymumutuzo@Umutuzos-iMac git-bundleOne % git stash list
stash@{0}: WIP on dev: 2584dba Add exercise 2 trial
stash@{1}: WIP on dev: 2584dba Add exercise 2 trial
stash@{2}: WIP on dev: 2584dba Add exercise 2 trial
gymumutuzo@Umutuzos-iMac git-bundleOne % 
`git stash pop stash@{1}` #applies stash@{1} and removes it from the stash list.
On branch dev
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   about.html
        modified:   readme.md

no changes added to commit (use "git add" and/or "git commit -a")
Dropped stash@{1} (afb411ec7f502bcd389f00013b7aedbb3dec50fd)
gymumutuzo@Umutuzos-iMac git-bundleOne % git stash list         
stash@{0}: WIP on dev: 2584dba Add exercise 2 trial
stash@{1}: WIP on dev: 2584dba Add exercise 2 trial
gymumutuzo@Umutuzos-iMac git-bundleOne % 
`git stash pop stash@{1} `
On branch dev
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   about.html
        modified:   home.html
        modified:   readme.md

no changes added to commit (use "git add" and/or "git commit -a")
Dropped stash@{1} (4c0f3a89602c07094d0c01780fbb2fe7cff9cc28)
git add about.html home.html 
gymumutuzo@Umutuzos-iMac git-bundleOne % 
`git commit -m "stash and pop first two files"` #commiting the staged files
[dev 94e1209] stash and pop first two files
 2 files changed, 13 insertions(+), 3 deletions(-)
gymumutuzo@Umutuzos-iMac git-bundleOne % 
`git pull origin main`
From https://github.com/kelia01/git-bundleOne
 * branch            main       -> FETCH_HEAD
Already up to date.
gymumutuzo@Umutuzos-iMac git-bundleOne % git push    
fatal: The current branch dev has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin dev

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

gymumutuzo@Umutuzos-iMac git-bundleOne % 
`git push --set-upstream origin dev` #pushing to the remote repository
Enumerating objects: 9, done.
Counting objects: 100% (9/9), done.
Delta compression using up to 8 threads
Compressing objects: 100% (8/8), done.
Writing objects: 100% (8/8), 1.00 KiB | 1.00 MiB/s, done.
Total 8 (delta 3), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (3/3), done.
To https://github.com/kelia01/git-bundleOne.git
   b1b457c..94e1209  dev -> dev
branch 'dev' set up to track 'origin/dev'.
gymumutuzo@Umutuzos-iMac git-bundleOne % git stash list
stash@{0}: WIP on dev: 2584dba Add exercise 2 trial
gymumutuzo@Umutuzos-iMac git-bundleOne % 
`git stash pop stash@{0}`
On branch dev
Your branch is up to date with 'origin/dev'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   readme.md
        modified:   team.html

no changes added to commit (use "git add" and/or "git commit -a")
Dropped stash@{0} (423fb54affc212114518b27cd73b442a44c698e4)
gymumutuzo@Umutuzos-iMac git-bundleOne % git stash list         
gymumutuzo@Umutuzos-iMac git-bundleOne % 
`git reset --hard` #resetting the current changes
HEAD is now at 94e1209 stash and pop first two files
gymumutuzo@Umutuzos-iMac git-bundleOne % 
`git status`  # Checking the status of the git currently
On branch dev
Your branch is up to date with 'origin/dev'.
nothing to commit, working tree clean 
