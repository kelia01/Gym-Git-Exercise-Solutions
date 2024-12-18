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
 
[Repository Name](https://github.com/kelia01/git-bundleOne.git)

 
