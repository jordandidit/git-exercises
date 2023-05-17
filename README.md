#######EXERCISE 1###########3
# git-exercises

in the first excercise 
we are tasked to create and initialise git
rename main branch from 'master' to 'main'
make changes like adding files
stage changes and committing them
connect the github repo
push changes to github
create a new branch dev
from dev create another branch test 
go back to dev and delete test

#here are my git codes to execute the above

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (master)
$ git init
Initialized empty Git repository in C:/Users/FALCON/Downloads/the gym rwanda files/git/.git/

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (master)
$ git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        .vscode/
        index.html

nothing added to commit but untracked files present (use "git add" to track)

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (master)
$ git add index.html

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (master)
$ git branch -M main

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (main)
$ git add readme.md

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (main)
$ git commit -m "init project"
[main (root-commit) 47fe311] init project
 2 files changed, 13 insertions(+)
 create mode 100644 index.html
 create mode 100644 readme.md

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (main)
$ git remote add origin https://github.com/jordandidit/git-exercises.git

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (main)
$ git push
fatal: The current branch main has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin main

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (main)
$ git push --set-upstream origin main
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (4/4), 420 bytes | 420.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/jordandidit/git-exercises.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (main)
$ git checkout -b dev
Switched to a new branch 'dev'

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (dev)
$ git status
On branch dev
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        .vscode/
        read me.md

nothing added to commit but untracked files present (use "git add" to track)

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (dev)
$ git push origin dev
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (4/4), 420 bytes | 420.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0
remote: 
remote: Create a pull request for 'dev' on GitHub by visiting:
remote:      https://github.com/jordandidit/git-exercises/pull/new/dev
remote:
To https://github.com/jordandidit/git-exercises.git
 * [new branch]      dev -> dev

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (dev)
$ git checkout -b test
Switched to a new branch 'test'

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (test)
$ git push origin test
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote: 
remote: Create a pull request for 'test' on GitHub by visiting:
remote:      https://github.com/jordandidit/git-exercises/pull/new/test
remote:
To https://github.com/jordandidit/git-exercises.git
 * [new branch]      test -> test

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (test)
$ git checkout dev
Switched to branch 'dev'

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (dev)
$ git branch -D test
Deleted branch test (was 47fe311).

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (dev)
$ git push origin --delete test
To https://github.com/jordandidit/git-exercises.git
 - [deleted]         test

