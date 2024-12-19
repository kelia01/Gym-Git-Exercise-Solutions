# Gym-Git-Exercise-Solutions
 
 ## Bundle 1

 ### Exercise 1

 ```bash
 `git init` # initialising a git repository
Initialized empty Git repository in /Users/gymumutuzo/git-bundleOne/.git/
gymumutuzo@Umutuzos-iMac git-bundleOne % 
`git branch` #checking current branch
gymumutuzo@Umutuzos-iMac git-bundleOne % 
`git status` #checking the staged files
On branch main

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        readme.md

nothing added to commit but untracked files present (use "git add" to track)
gymumutuzo@Umutuzos-iMac git-bundleOne % 
`git branch -M master` #changing branch to master
gymumutuzo@Umutuzos-iMac git-bundleOne % 
`git branch -M main`
gymumutuzo@Umutuzos-iMac git-bundleOne % 
`git status`
On branch main

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        readme.md

nothing added to commit but untracked files present (use "git add" to track)
gymumutuzo@Umutuzos-iMac git-bundleOne % 
`git add readme.md` #staging a file
gymumutuzo@Umutuzos-iMac git-bundleOne % 
`git commit -m "This is for exercise 1"` #commiting a file with commit message
[main (root-commit) b1b457c] This is for exercise 1
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 readme.md
gymumutuzo@Umutuzos-iMac git-bundleOne % 
`git remote add originhttps://github.com/kelia01/git-bundleOne.git` #connect to the github repository
gymumutuzo@Umutuzos-iMac git-bundleOne % git push
fatal: The current branch main has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin main

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

gymumutuzo@Umutuzos-iMac git-bundleOne % 
`git push --set-upstream origin main` #pushing to your github repository
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 229 bytes | 229.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/kelia01/git-bundleOne.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.
gymumutuzo@Umutuzos-iMac git-bundleOne % 
`git checkout -b dev` #creating new branch dev
Switched to a new branch 'dev'
gymumutuzo@Umutuzos-iMac git-bundleOne % 
`git checkout -b test` #creating new branch test under dev
Switched to a new branch 'test'
gymumutuzo@Umutuzos-iMac git-bundleOne % 
`git checkout dev` #changing to branch dev
Switched to branch 'dev'
gymumutuzo@Umutuzos-iMac git-bundleOne % 
`git branch -D test` #deleting branch test locally
Deleted branch test (was b1b457c).
gymumutuzo@Umutuzos-iMac git-bundleOne % 
`git checkout -b test` 
Switched to a new branch 'test'
gymumutuzo@Umutuzos-iMac git-bundleOne % 
`git push origin dev` 
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote: 
remote: Create a pull request for 'dev' on GitHub by visiting:
remote:      https://github.com/kelia01/git-bundleOne/pull/new/dev
remote: 
To https://github.com/kelia01/git-bundleOne.git
 * [new branch]      dev -> dev
gymumutuzo@Umutuzos-iMac git-bundleOne % 
`git push origin test`
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote: 
remote: Create a pull request for 'test' on GitHub by visiting:
remote:      https://github.com/kelia01/git-bundleOne/pull/new/test
remote: 
To https://github.com/kelia01/git-bundleOne.git
 * [new branch]      test -> test
gymumutuzo@Umutuzos-iMac git-bundleOne % `git checkout dev`
Switched to branch 'dev'
gymumutuzo@Umutuzos-iMac git-bundleOne % 
`git push origin --delete test` #deleting branch test on the remote repository
To https://github.com/kelia01/git-bundleOne.git
 - [deleted]         test```
 
[Repository Name](https://github.com/kelia01/git-bundleOne.git)

 
## Bundle 2

### Exercise 1

``` bash
`git checkout -b ft/bundle-2` #created a new branch ft/bundle-2
 One> git add services.html
Switched to a new branch 'ft/bundle-2'
PS C:\Users\HP\git-bundleOne\git-bundleOne> 
`git add services.html` #staged file services.html
PS C:\Users\HP\git-bundleOne\git-bundleOne> 
`git commit -m "Add a new sevice.html file"` #commited the changes
[ft/bundle-2 1fba2a8] Add a new sevice.html file
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 services.html
 `git push -u origin ft/bundle-2` #push on remote repo 
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 254 bytes | 50.00 KiB/s, done.
Total 2 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/bundle-2' on GitHub by visiting:
remote:      https://github.com/kelia01/git-bundleOne/pull/new/ft/bundle-2
remote:
To https://github.com/kelia01/git-bundleOne.git  
 * [new branch]      ft/bundle-2 -> ft/bundle-2  
branch 'ft/bundle-2' set up to track 'origin/ft/bundle-2'.```

## Bundle 2

### Exercise 2
``` bash
$ `git checkout main` #checking out branch main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

HP@DESKTOP-R0HLVRA MINGW64 ~/git-bundleOne/git-bundleOne (main)

$ `git pull origin main` #pulling the latest changes
From https://github.com/kelia01/git-bundleOne
 * branch            main       -> FETCH_HEAD
Already up to date.

HP@DESKTOP-R0HLVRA MINGW64 ~/git-bundleOne/git-bundleOne (main)

$ `git checkout -b ft/service-redesign` #creating a new branch
Switched to a new branch 'ft/service-redesign'
PS C:\Users\HP\git-bundleOne\git-bundleOne> 

`git add services.html `      
PS C:\Users\HP\git-bundleOne\git-bundleOne> 

`git status`
On branch ft/service-redesign
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   services.html

PS C:\Users\HP\git-bundleOne\git-bundleOne> 

`git commit -m "Add a paragraph to service.html"`
[ft/service-redesign 31611a6] Add a paragraph to service.html
 1 file changed, 13 insertions(+)
 create mode 100644 services.html
PS C:\Users\HP\git-bundleOne\git-bundleOne> 

`git push -u origin ft/service-redesign`
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.    
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done. 
Writing objects: 100% (3/3), 500 bytes | 38.00 KiB/s, done.  
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.    
remote: 
remote: Create a pull request for 'ft/service-redesign' on GitHub by visiting:
remote:      https://github.com/kelia01/git-bundleOne/pull/new/ft/service-redesign
remote:
To https://github.com/kelia01/git-bundleOne.git
 * [new branch]      ft/service-redesign -> ft/service-redesign
branch 'ft/service-redesign' set up to track 'origin/ft/service-redesign'.

`git checkout main`
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
PS C:\Users\HP\git-bundleOne\git-bundleOne> 

`git add services.html`
PS C:\Users\HP\git-bundleOne\git-bundleOne> 

`git commit -m "Correct a paragraph in service.html"`
[main 6a65f2d] Correct a paragraph in service.html
 1 file changed, 13 insertions(+)
 create mode 100644 services.html
PS C:\Users\HP\git-bundleOne\git-bundleOne> 

`git push -u origin main`     
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 506 bytes | 253.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.    
To https://github.com/kelia01/git-bundleOne.git
   5c43eb4..6a65f2d  main -> main
branch 'main' set up to track 'origin/main'.

`git checkout ft/service-redesign `
Switched to branch 'ft/service-redesign'
Your branch is up to date with 'origin/ft/service-redesign'.
PS C:\Users\HP\git-bundleOne\git-bundleOne> 

`git diff main -- services.html` #check the differences between the files on the two branches
diff --git a/services.html b/services.html
index 91c98e8..368b723 100644
--- a/services.html
+++ b/services.html
@@ -6,7 +6,7 @@
     <title>Welcome | Services</title>
 <body>
     <h1>Our services are excellent,
-        it is unlikely that you will find them elsewhere.
+        it is unlikely that you will them elsewhere.
     </h1>
 </body>
 </html>

 `git checkout main` #switched to main to merge it with ft/service-redesign
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
Your branch is up to date with 'origin/main'.
Auto-merging services.html
CONFLICT (add/add): Merge conflict in services.html
Automatic merge failed; fix conflicts and then commit the result.
PS C:\Users\HP\git-bundleOne\git-bundleOne> 

`git merge ft/service-redesign` #merged ft/service-redesign to main
Merge branch 'ft/service-redesign'
PS C:\Users\HP\git-bundleOne\git-bundleOne> 

`git add services.html`     #after resolving a conflict caused by the change in the same files at the same line of code, staged the file again
PS C:\Users\HP\git-bundleOne\git-bundleOne> 

`git commit` #commited with no message as merge provides its own
[main 7471511] Merge branch 'ft/service-redesign'
PS C:\Users\HP\git-bundleOne\git-bundleOne> 

`git push -u origin main` #pushe my changes
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.    
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done. 
Writing objects: 100% (3/3), 379 bytes | 75.00 KiB/s, done.  
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.   
To https://github.com/kelia01/git-bundleOne.git
   6a65f2d..7471511  main -> main
branch 'main' set up to track 'origin/main'.
```
 
[git-bundleTwo](https://github.com/kelia01/git-bundleOne.git)