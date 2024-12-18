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
gymumutuzo@Umutuzos-iMac git-bundleOne % git branch -M master
gymumutuzo@Umutuzos-iMac git-bundleOne % git branch -M main
gymumutuzo@Umutuzos-iMac git-bundleOne % git status
On branch main

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        readme.md

nothing added to commit but untracked files present (use "git add" to track)
gymumutuzo@Umutuzos-iMac git-bundleOne % git add readme.md
gymumutuzo@Umutuzos-iMac git-bundleOne % git commit -m "This is for exercise 1"
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

gymumutuzo@Umutuzos-iMac git-bundleOne % git push --set-upstream origin main
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 229 bytes | 229.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/kelia01/git-bundleOne.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.
gymumutuzo@Umutuzos-iMac git-bundleOne % git branch -b dev
error: unknown switch `b'
usage: git branch [<options>] [-r | -a] [--merged] [--no-merged]
   or: git branch [<options>] [-f] [--recurse-submodules] <branch-name> [<start-point>]
   or: git branch [<options>] [-l] [<pattern>...]
   or: git branch [<options>] [-r] (-d | -D) <branch-name>...
   or: git branch [<options>] (-m | -M) [<old-branch>] <new-branch>
   or: git branch [<options>] (-c | -C) [<old-branch>] <new-branch>
   or: git branch [<options>] [-r | -a] [--points-at]
   or: git branch [<options>] [-r | -a] [--format]

Generic options
    -v, --verbose         show hash and subject, give twice for upstream branch
    -q, --quiet           suppress informational messages
    -t, --track[=(direct|inherit)]
                          set branch tracking configuration
    -u, --set-upstream-to <upstream>
                          change the upstream info
    --unset-upstream      unset the upstream info
    --color[=<when>]      use colored output
    -r, --remotes         act on remote-tracking branches
    --contains <commit>   print only branches that contain the commit
    --no-contains <commit>
                          print only branches that don't contain the commit
    --abbrev[=<n>]        use <n> digits to display object names

Specific git-branch actions:
    -a, --all             list both remote-tracking and local branches
    -d, --delete          delete fully merged branch
    -D                    delete branch (even if not merged)
    -m, --move            move/rename a branch and its reflog
    -M                    move/rename a branch, even if target exists
    -c, --copy            copy a branch and its reflog
    -C                    copy a branch, even if target exists
    -l, --list            list branch names
    --show-current        show current branch name
    --create-reflog       create the branch's reflog
    --edit-description    edit the description for the branch
    -f, --force           force creation, move/rename, deletion
    --merged <commit>     print only branches that are merged
    --no-merged <commit>  print only branches that are not merged
    --column[=<style>]    list branches in columns
    --sort <key>          field name to sort on
    --points-at <object>  print only branches of the object
    -i, --ignore-case     sorting and filtering are case insensitive
    --recurse-submodules  recurse through submodules
    --format <format>     format to use for the output

gymumutuzo@Umutuzos-iMac git-bundleOne % git checkout -b dev
Switched to a new branch 'dev'
gymumutuzo@Umutuzos-iMac git-bundleOne % git checkout -b test 
Switched to a new branch 'test'
gymumutuzo@Umutuzos-iMac git-bundleOne % git checkout dev
Switched to branch 'dev'
gymumutuzo@Umutuzos-iMac git-bundleOne % git -D test
unknown option: -D
usage: git [-v | --version] [-h | --help] [-C <path>] [-c <name>=<value>]
           [--exec-path[=<path>]] [--html-path] [--man-path] [--info-path]
           [-p | --paginate | -P | --no-pager] [--no-replace-objects] [--bare]
           [--git-dir=<path>] [--work-tree=<path>] [--namespace=<name>]
           [--super-prefix=<path>] [--config-env=<name>=<envvar>]
           <command> [<args>]
gymumutuzo@Umutuzos-iMac git-bundleOne % git branch -D test
Deleted branch test (was b1b457c).
gymumutuzo@Umutuzos-iMac git-bundleOne % git checkout -b test 
Switched to a new branch 'test'
gymumutuzo@Umutuzos-iMac git-bundleOne % git push origin dev
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote: 
remote: Create a pull request for 'dev' on GitHub by visiting:
remote:      https://github.com/kelia01/git-bundleOne/pull/new/dev
remote: 
To https://github.com/kelia01/git-bundleOne.git
 * [new branch]      dev -> dev
gymumutuzo@Umutuzos-iMac git-bundleOne % git push origin test
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote: 
remote: Create a pull request for 'test' on GitHub by visiting:
remote:      https://github.com/kelia01/git-bundleOne/pull/new/test
remote: 
To https://github.com/kelia01/git-bundleOne.git
 * [new branch]      test -> test
gymumutuzo@Umutuzos-iMac git-bundleOne % git checkout dev
Switched to branch 'dev'
gymumutuzo@Umutuzos-iMac git-bundleOne % git push origin --delete test
To https://github.com/kelia01/git-bundleOne.git
 - [deleted]         test```
 

 
