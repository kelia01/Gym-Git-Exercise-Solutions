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
 - [deleted]         test
 ```
 
[git-bundleOne](https://github.com/kelia01/git-bundleOne.git)

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
branch 'ft/bundle-2' set up to track 'origin/ft/bundle-2'.
```

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

## Bundle 3

### Exercise 1

``` bash
`git checkout -b ft/team-page`
Switched to a new branch 'ft/team-page'
PS C:\Users\HP\git-bundleOne\git-bundleOne> 

`git add teaam.html`
PS C:\Users\HP\git-bundleOne\git-bundleOne> 

`git commit -m "Add a new teaam.html file"`
[ft/team-page 2240d78] Add a new teaam.html file
 1 file changed, 11 insertions(+)
 create mode 100644 teaam.html
PS C:\Users\HP\git-bundleOne\git-bundleOne> 

`git push -u origin ft/team-page`
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.    
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 482 bytes | 241.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/team-page' 
on GitHub by visiting:
remote:      https://github.com/kelia01/git-bundleOne/pull/new/ft/team-page
remote:
To https://github.com/kelia01/git-bundleOne.git
 * [new branch]      ft/team-page -> ft/team-pagebranch 'ft/team-page' set up to track 'origin/ft/team-page'.

 `git checkout main`
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
PS C:\Users\HP\git-bundleOne\git-bundleOne> 

`git checkout -b ft/contact-page`
Switched to a new branch 'ft/contact-page'
PS C:\Users\HP\git-bundleOne\git-bundleOne> 

`git checkout ft/team-page`
Switched to branch 'ft/team-page'
Your branch is up to date with 'origin/ft/team-page'.
PS C:\Users\HP\git-bundleOne\git-bundleOne> 

`git log` #logs the commit history
Author: Kelia Iradukunda <iradukundakelia@gmail.cHEAD -> ft/team-page, origin/ft/team-page)Date:   Thu Dec 19 13:56:10 2024 +0200           om>
    Add a new teaam.html file

commit 74715110a97c56e6a164f1c84d0969ca5a51abbd (origin/main, origin/HEAD, main, ft/contact-page) 
Merge: 6a65f2d 31611a6                           origin/main, origin/HEAD, main, ft/contact-page)
Author: Kelia Iradukunda <iradukundakelia@gmail.com>                                              om>
Date:   Thu Dec 19 13:17:44 2024 +0200

PS C:\Users\HP\git-bundleOne\git-bundleOne> 

`git checkout ft/contact-page`
Switched to branch 'ft/contact-page'
PS C:\Users\HP\git-bundleOne\git-bundleOne> 

`git cherry-pick 2240d78f7c627b672b1d38098a00af074c07fc45` #uses the commit hash and applies the commit from one branch to teh specified branch
[ft/contact-page 07fb06e] Add a new teaam.html file
 Date: Thu Dec 19 13:56:10 2024 +0200
 1 file changed, 11 insertions(+)
 create mode 100644 teaam.html

`git checkout -b ft/team-page`
Switched to a new branch 'ft/team-page'
PS C:\Users\HP\git-bundleOne\git-bundleOne> 

`git add teaam.html`
PS C:\Users\HP\git-bundleOne\git-bundleOne> 

`git commit -m "Add a new teaam.html file"`
[ft/team-page 2240d78] Add a new teaam.html file
 1 file changed, 11 insertions(+)
 create mode 100644 teaam.html
PS C:\Users\HP\git-bundleOne\git-bundleOne> 

`git push -u origin ft/team-page`
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.    
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 482 bytes | 241.00 KPS C:\Users\HP\git-bundleOne\git-bundleOne> git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
PS C:\Users\HP\git-bundleOne\git-bundleOne> 

`git checkout -b ft/contact-page`
Switched to a new branch 'ft/contact-page'
PS C:\Users\HP\git-bundleOne\git-bundleOne> 

`git checkout ft/team-page`
Switched to branch 'ft/team-page'
Your branch is up to date with 'origin/ft/team-page'.
PS C:\Users\HP\git-bundleOne\git-bundleOne> git log
Author: Kelia Iradukunda <iradukundakelia@gmail.cHEAD -> ft/team-page, oDate:   Thu Dec 19 13:56:10 2024 +0200           om>
    Add a new teaam.html file

commit 74715110a97c56e6a164f1c84d0969ca5a51abbd (origin/main, origin/HEAD, main, ft/contact-page) 
Merge: 6a65f2d 31611a6                           origin/main, origin/HEA

PS C:\Users\HP\git-bundleOne\git-bundleOne> 

`git commit -m  "Add a new contact.html"`
[ft/contact-page eff1545] Add a new contact.html
 1 file changed, 11 insertions(+)              
 create mode 100644 contact.html
PS C:\Users\HP\git-bundleOne\git-bundleOne> 

`git status`
On branch ft/contact-page
nothing to commit, working tree clean       
PS C:\Users\HP\git-bundleOne\git-bundleOne> 

`git push -u origin ft/contact-page`
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 4 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 815 bytes | 271.00 KiB/s, done.
remote: Resolving deltas: 100% (3/3), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/contact-page' on GitHub by visiting:
remote:
ft/contact-page'.
PS C:\Users\HP\git-bundleOne\git-bundleOne> git status
-page'.

nothing to commit, working tree clean
PS C:\Users\HP\git-bundleOne\git-bundleOne> 

`git checkout -b ft/faq-page`
Switched to a new branch 'ft/faq-page'
PS C:\Users\HP\git-bundleOne\git-bundleOne> 

`git add faq.html`
PS C:\Users\HP\git-bundleOne\git-bundleOne> 

`git commit -m "Add a new faq.html file"`
[ft/faq-page 9bbf3fb] Add a new faq.html file    
 1 file changed, 11 insertions(+)
 create mode 100644 faq.html
PS C:\Users\HP\git-bundleOne\git-bundleOne> 

`git push -u origin ft/faq-page`
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 466 bytes | 233.00 Kd 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/faq-page' on GitHub by visiting:
remote:      https://github.com/kelia01/git-bundleOne/pull/new/ft/faq-page        
remote:
To https://github.com/kelia01/git-bundleOne.git
 * [new branch]      ft/faq-page -> ft/faq-page
branch 'ft/faq-page' set up to track 'origin/ft/faq-page'.
PS C:\Users\HP\git-bundleOne\git-bundleOne> 

`git checkout ft/team-page`
Switched to branch 'ft/team-page'
Your branch is up to date with 'origin/ft/team-page'.
git status
On branch ft/team-page

nothing to commit, working tree clean
PS C:\Users\HP\git-bundleOne\git-bundleOne> 

`git log -1` #brings back the last recent commit 
commit 2240d78f7c627b672b1d38098a00af074c07fc45 (HEAD -> ft/team-page, origin/ft/team-page)
Author: Kelia Iradukunda <iradukundakelia@gmail.com>
Date:   Thu Dec 19 13:56:10 2024 +0200

    Add a new teaam.html file
PS C:\Users\HP\git-bundleOne\git-bundleOne> 

`git revert 2240d78f7c627b672b1d38098a00af074c07fc45` # undoes changes introduced by a specific commit by creating a new commit 
[ft/team-page 7d5c1cf] Revert "Add a new teaam.html file"
 1 file changed, 11 deletions(-)
 delete mode 100644 teaam.html
PS C:\Users\HP\git-bundleOne\git-bundleOne> 

`git push origin ft/team-page`    
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 267 bytes | 267.00 KiB/s, done.
Total 2 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/kelia01/git-bundleOne.git
   2240d78..7d5c1cf  ft/team-page -> ft/team-page