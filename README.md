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

One> 
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