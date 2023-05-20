########BUNDLE 2 AND 3##########
includes
BUNDLE2
EXERCISE 1 & 2

BUNDLE3
EXCERCise 1&2


FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (dev)
$ git add index.html

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (dev)
$ git status
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   .vscode/settings.json
        new file:   about.html
        new file:   home.html
        new file:   read me.md
        new file:   team.html


FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (dev)
$ git stash list
stash@{0}: WIP on dev: 47fe311 init project

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (dev)
$ git stash pop stash@{0}
Auto-merging about.html
Auto-merging home.html
Auto-merging team.html
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   .vscode/settings.json
        new file:   about.html
        new file:   home.html
        new file:   read me.md
        new file:   team.html

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   about.html
        modified:   home.html

Dropped stash@{0} (b4dc2af7449f31c12240b9df220d9344feb1ba8e)

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (dev)
$ git status
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   .vscode/settings.json
        new file:   about.html
        new file:   home.html
        new file:   read me.md
        new file:   team.html

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   about.html
        modified:   home.html


FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (dev)
$ git status
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   .vscode/settings.json
        new file:   about.html
        new file:   home.html
        new file:   read me.md
        new file:   team.html

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   about.html
        modified:   home.html


FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (dev)
$ git stash list

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (dev)
$ git status
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   .vscode/settings.json
        new file:   about.html
        new file:   home.html
        new file:   read me.md
        new file:   team.html

Changes not staged for commit:
  (use "git add/rm <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   about.html
        modified:   home.html
        deleted:    team.html


FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (dev)
$ git add home.html

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (dev)
$ git add about.htm;
fatal: pathspec 'about.htm' did not match any files

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (dev)
$ git add about.html

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (dev)
$ git commit -m "the home and about page"
[dev 9090968] the home and about page
 5 files changed, 40 insertions(+)
 create mode 100644 .vscode/settings.json
 create mode 100644 about.html
 create mode 100644 home.html
 create mode 100644 read me.md
 create mode 100644 team.html

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (dev)
$ git drop team.html
git: 'drop' is not a git command. See 'git --help'.

The most similar command is
        grep

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (dev)
$ git rm team.html
rm 'team.html'

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (dev)
$ git commit -m "about and home page"
[dev 89f5778] about and home page
 1 file changed, 12 deletions(-)
 delete mode 100644 team.html

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (dev)
$ git status
On branch dev
nothing to commit, working tree clean

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (dev)
$ git add about.html

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (dev)
$ git add home.html

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (dev)
$ git status
On branch dev
nothing to commit, working tree clean

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (dev)
$ git add home.html

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (dev)
$ git add about.html

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (dev)
$ git rm index.html
rm 'index.html'

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (dev)
$ git commit -m "about and home page"
[dev 538653c] about and home page
 1 file changed, 13 deletions(-)
 delete mode 100644 index.html

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (dev)
$ git pusj
git: 'pusj' is not a git command. See 'git --help'.

The most similar command is
        push

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (dev)
$ git push
fatal: The current branch dev has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin dev

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (dev)
$ git push --set-upstream origin dev
Enumerating objects: 12, done.
remote: Resolving deltas: 100% (3/3), done.
To https://github.com/jordandidit/git-exercises.git
   47fe311..538653c  dev -> dev
branch 'dev' set up to track 'origin/dev'.

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (dev)   
$ git reset --hard
HEAD is now at 538653c about and home page

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (dev)
$ git status
On branch dev
Your branch is behind 'origin/dev' by 1 commit, and can be fast-forwarded.
  (use "git pull" to update your local branch)

nothing to commit, working tree clean

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (dev)   
$ git checkout -b ft/bundle2
Switched to a new branch 'ft/bundle2'

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (ft/bundle2)
$ git status
On branch ft/bundle2
nothing to commit, working tree clean

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (ft/bundle2)
$ git add service.html
fatal: pathspec 'service.html' did not match any files

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (ft/bundle2)
$ git add services.html

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (ft/bundle2)
$ git stash
Saved working directory and index state WIP on ft/bundle2: 538653c about and home page

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (ft/bundle2)
$ git stash pop
On branch ft/bundle2
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   services.html

Dropped refs/stash@{0} (aa509451c516af5992065bd82d6d8b0c1aa03c10)

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (ft/bundle2)
$ git add services.html

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (ft/bundle2)
$ git status
On branch ft/bundle2
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   services.html


FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (ft/bundle2)
$ git commit -m "services page"
[ft/bundle2 28805f3] services page
 1 file changed, 12 insertions(+)
 create mode 100644 services.html

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (ft/bundle2)
$ git status
On branch ft/bundle2
nothing to commit, working tree clean

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (ft/bundle2)
$ git push
fatal: The current branch ft/bundle2 has no upstream branch.
To push the current branch and set the remote as upstream, use       

    git push --set-upstream origin ft/bundle2

To have this happen automatically for branches without a tracking    
upstream, see 'push.autoSetupRemote' in 'git help config'.


FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (ft/bundle2)
$ git push --set-upstream origin ft/bundle2
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 477 bytes | 43.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object. 
remote: 
remote: Create a pull request for 'ft/bundle2' on GitHub by visiting 
remote:      https://github.com/jordandidit/git-exercises/pull/new/ft/bundle2
remote:
To https://github.com/jordandidit/git-exercises.git
 * [new branch]      ft/bundle2 -> ft/bundle2
branch 'ft/bundle2' set up to track 'origin/ft/bundle2'.

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (ft/bundle2)
$ git checkout main
Switched to branch 'main'
Your branch is behind 'origin/main' by 4 commits, and can be fast-forwarded.
  (use "git pull" to update your local branch)

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (main)  
$ git pull
Updating 47fe311..e0e52c1
Fast-forward
 README.md | 162 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 1 file changed, 162 insertions(+)
 create mode 100644 README.md

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (main)  
$ git checkout -b ft/service-redesign
Switched to a new branch 'ft/service-redesign'

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (ft/service-redesign)
$ git status
On branch ft/service-redesign
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   readme.md

no changes added to commit (use "git add" and/or "git commit -a")    

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (ft/service-redesign)
$ git add --all

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (ft/service-redesign)
$ git status
On branch ft/service-redesign
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   readme.md
        new file:   services.html


FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (ft/service-redesign)
$ git commit -m "added the service list"
[ft/service-redesign 72565f9] added the service list
 2 files changed, 178 insertions(+)
 create mode 100644 services.html

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (ft/service-redesign)
$ git push
fatal: The current branch ft/service-redesign has no upstream branch.
To push the current branch and set the remote as upstream, use       

    git push --set-upstream origin ft/service-redesign

To have this happen automatically for branches without a tracking    
upstream, see 'push.autoSetupRemote' in 'git help config'.


FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (ft/service-redesign)
$ git push --set-upstream origin ft/service-redesign
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 516 bytes | 129.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object. 
remote: 
remote: Create a pull request for 'ft/service-redesign' on GitHub by visiting:
remote:      https://github.com/jordandidit/git-exercises/pull/new/ft/service-redesign
remote:
To https://github.com/jordandidit/git-exercises.git
 * [new branch]      ft/service-redesign -> ft/service-redesign      
branch 'ft/service-redesign' set up to track 'origin/ft/service-redesign'.

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (ft/service-redesign)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (main)  
$ git commit -m "add old services"
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

Untracked files:
  (use "git add <file>..." to include in what will be committed)     
        services.html

no changes added to commit (use "git add" and/or "git commit -a")    

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (main)  
$ git add --all

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (main)  
$ git stash
Saved working directory and index state WIP on main: e0e52c1 Update README.md

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (main)  
$ git stash pop
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   services.html

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

Dropped refs/stash@{0} (f417d1fc5a6d8a0857b7686c946c0badf47ad1cb)

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (main)  
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   services.html

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md


FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (main)  
$ git add --all

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (main)  
$ git commit -m "add old services"
[main 8180ff1] add old services
 1 file changed, 17 insertions(+)
 create mode 100644 services.html

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (main)  
$ git status
On branch main
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")    

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (main)  
$ git push
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 522 bytes | 130.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object. 
To https://github.com/jordandidit/git-exercises.git
   e0e52c1..8180ff1  main -> main

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (main)  
$ git checkout ft/service-redesign
Switched to branch 'ft/service-redesign'
M       README.md
Your branch is up to date with 'origin/ft/service-redesign'.

  
  
  #####################BUNDLE 3 BEGIN####################################
  ###########excercise1&2################################################
  
  
  FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (ft/contact-page|CHERRY-PICKING)
$ git push
Enumerating objects: 10, done.
Counting objects: 100% (10/10), done.
Delta compression using up to 8 threads
Compressing objects: 100% (7/7), done.
Writing objects: 100% (7/7), 783 bytes | 261.00 KiB/s, done.
Total 7 (delta 5), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (5/5), completed with 3 local objects.
To https://github.com/jordandidit/git-exercises.git
   3a811e1..f2ee344  ft/contact-page -> ft/contact-page

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (ft/contact-page|CHERRY-PICKING)
$ git log
commit f2ee344755b801fd6f77d76ace75ba6ed73b6cd8 (HEAD -> ft/contact-page, origin/ft/contact-page)
Author: jordandidit <jordygashagaza@gmail.com>
Date:   Fri May 19 00:10:20 2023 +0200

    new team page created

commit fd43fa3eedb1478f352943ebf1b1f2df47f727c7
Author: jordandidit <jordygashagaza@gmail.com>
Date:   Fri May 19 00:10:20 2023 +0200

    new team page created


FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (ft/contact-page|CHERRY-PICKING)
$ git cherry-pick f2ee344755b801fd6f77d76ace75ba6ed73b6cd8
The previous cherry-pick is now empty, possibly due to conflict resolution.
If you wish to commit it anyway, use:

    git commit --allow-empty

Otherwise, please use 'git cherry-pick --skip'
On branch ft/contact-page
Your branch is up to date with 'origin/ft/contact-page'.

You are currently cherry-picking commit f2ee344.
  (all conflicts fixed: run "git cherry-pick --continue")
  (use "git cherry-pick --skip" to skip this patch)
  (use "git cherry-pick --abort" to cancel the cherry-pick operation)

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (ft/contact-page|CHERRY-PICKING)
$ git add services.html

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (ft/contact-page|CHERRY-PICKING)
$ git add team.html

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (ft/contact-page|CHERRY-PICKING)
$ git commit
The previous cherry-pick is now empty, possibly due to conflict resolution.
If you wish to commit it anyway, use:

    git commit --allow-empty

Otherwise, please use 'git cherry-pick --skip'
On branch ft/contact-page
Your branch is up to date with 'origin/ft/contact-page'.

You are currently cherry-picking commit f2ee344.
  (all conflicts fixed: run "git cherry-pick --continue")
  (use "git cherry-pick --skip" to skip this patch)
  (use "git cherry-pick --abort" to cancel the cherry-pick operation)

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (ft/contact-page|CHERRY-PICKING)
$ git checkout ft/contact-page
Already on 'ft/contact-page'
warning: cancelling a cherry picking in progress
M       README.md
Your branch is up to date with 'origin/ft/contact-page'.

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (ft/contact-page)
$ git add team.html

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (ft/contact-page)
$ git cherry-pick f2ee344755b801fd6f77d76ace75ba6ed73b6cd8
The previous cherry-pick is now empty, possibly due to conflict resolution.
If you wish to commit it anyway, use:

    git commit --allow-empty

Otherwise, please use 'git cherry-pick --skip'
On branch ft/contact-page
Your branch is up to date with 'origin/ft/contact-page'.

You are currently cherry-picking commit f2ee344.
  (all conflicts fixed: run "git cherry-pick --continue")
  (use "git cherry-pick --skip" to skip this patch)
  (use "git cherry-pick --abort" to cancel the cherry-pick operation)

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (ft/contact-page|CHERRY-PICKING)
$ git checkout ft/contact-page
Already on 'ft/contact-page'
warning: cancelling a cherry picking in progress
M       README.md
Your branch is up to date with 'origin/ft/contact-page'.

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (ft/contact-page)
$ git commit -a
On branch ft/contact-page
Your branch is up to date with 'origin/ft/contact-page'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (ft/contact-page)
$ git add services.html

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (ft/contact-page)
$ git add team.html

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (ft/contact-page)
$ git commit -a
On branch ft/contact-page
Your branch is up to date with 'origin/ft/contact-page'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (ft/contact-page)
$ git cherry-pick f2ee344755b801fd6f77d76ace75ba6ed73b6cd8
The previous cherry-pick is now empty, possibly due to conflict resolution.
If you wish to commit it anyway, use:

    git commit --allow-empty

Otherwise, please use 'git cherry-pick --skip'
On branch ft/contact-page
Your branch is up to date with 'origin/ft/contact-page'.

You are currently cherry-picking commit f2ee344.
  (all conflicts fixed: run "git cherry-pick --continue")
  (use "git cherry-pick --skip" to skip this patch)
  (use "git cherry-pick --abort" to cancel the cherry-pick operation)

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
        modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")    

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (ft/contact-page|CHERRY-PICKING)
$ git cherry-pick --skip

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (ft/contact-page)
$ git status
On branch ft/contact-page
Your branch is up to date with 'origin/ft/contact-page'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")    

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (ft/contact-page)
$ git status
On branch ft/contact-page
Your branch is up to date with 'origin/ft/contact-page'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")    

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (ft/contact-page)
$ git add --all

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (ft/contact-page)
$ git add --all

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (ft/contact-page)
$ git commit "add contact page"
error: pathspec 'add contact page' did not match any file(s) known to git

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (ft/contact-page)
$ git commit -m "add contact page"
[ft/contact-page f79347d] add contact page
 1 file changed, 15 insertions(+)
 create mode 100644 contact.html

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (ft/contact-page)
$ git push
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 480 bytes | 480.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object. 
To https://github.com/jordandidit/git-exercises.git
   f2ee344..f79347d  ft/contact-page -> ft/contact-page

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (ft/contact-page)
$ git checkout -b ft/faq-page
Switched to a new branch 'ft/faq-page'

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (ft/faq-page)
$ git add --all

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (ft/faq-page)
$ git add --all

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (ft/faq-page)
$ git commit -m " add faq page"
[ft/faq-page f986578]  add faq page
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 faq.html

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (ft/faq-page)
$ git push --set-upstream origin ft/faq-page
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 260 bytes | 260.00 KiB/s, done.
Total 2 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object. 
remote: 
remote: Create a pull request for 'ft/faq-page' on GitHub by visiting:
remote:      https://github.com/jordandidit/git-exercises/pull/new/ft/faq-page
remote:
To https://github.com/jordandidit/git-exercises.git
 * [new branch]      ft/faq-page -> ft/faq-page
branch 'ft/faq-page' set up to track 'origin/ft/faq-page'.

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (ft/faq-page)
$ git log
commit f986578fe2e009932a4110a7b3a56a8e78dc258e (HEAD -> ft/faq-page,
 origin/ft/faq-page)
Author: jordandidit <jordygashagaza@gmail.com>
Date:   Sat May 20 15:41:10 2023 +0200

     add faq page

commit f79347d7841ce69bebe15e2696545aa320eb6fd5 (origin/ft/contact-page, ft/contact-page)
Author: jordandidit <jordygashagaza@gmail.com>
Date:   Sat May 20 15:35:33 2023 +0200


FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (ft/faq-page)
$ git push
Everything up-to-date

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (ft/faq-page)
$ git checkout -b ft/home-page-redesign
Switched to a new branch 'ft/home-page-redesign'

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (ft/home-page-redesign)      
$ git checkout main
Switched to branch 'main'
M       README.md
Your branch is behind 'origin/main' by 3 commits, and can be fast-forwarded.
  (use "git pull" to update your local branch)

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (main)
$ git status
On branch main
Your branch is behind 'origin/main' by 3 commits, and can be fast-forwarded.
  (use "git pull" to update your local branch)

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        contact.html
        faq.html
        home.html
        team.html

no changes added to commit (use "git add" and/or "git commit -a")

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (main)
$ git add --all

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (main)
$ git status
On branch main
Your branch is behind 'origin/main' by 3 commits, and can be fast-forwarded.
  (use "git pull" to update your local branch)

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   contact.html
        new file:   faq.html
        new file:   home.html
        new file:   team.html

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md


FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (main)
$ git commit -m "add homepage contents"
[main 1482eb9] add homepage contents
 4 files changed, 54 insertions(+)
 create mode 100644 contact.html
 create mode 100644 faq.html
 create mode 100644 home.html
 create mode 100644 team.html

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (main)
$ git status
On branch main
Your branch and 'origin/main' have diverged, 
and have 1 and 3 different commits each, respectively.
  (use "git pull" to merge the remote branch into yours)

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (main)
$ git log
commit 1482eb9f3f6af2d9d3e7a9131d4ad6da3cdf0a23 (HEAD -> main)
Author: jordandidit <jordygashagaza@gmail.com>
Date:   Sat May 20 15:49:34 2023 +0200       

    add homepage contents

commit 8180ff1784d3b0ec15d12663450b165a8b8cbf14
Author: jordandidit <jordygashagaza@gmail.com>

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (main)
$ git rebase main
error: cannot rebase: You have unstaged changes.
error: Please commit or stash them.

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (main)
$ git commit
On branch main
Your branch and 'origin/main' have diverged, 
and have 1 and 3 different commits each, respectively.
  (use "git pull" to merge the remote branch into yours)

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (main)
$ git commit -a
On branch main
Your branch and 'origin/main' have diverged, 
and have 1 and 3 different commits each, respectively.
  (use "git pull" to merge the remote branch into yours)

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (main)
$ git push
To https://github.com/jordandidit/git-exercises.git
 ! [rejected]        main -> main (non-fast-forward)
error: failed to push some refs to 'https://github.com/jordandidit/git-exercises.git'     
hint: Updates were rejected because the tip of your current branch is behind
hint: its remote counterpart. Integrate the remote changes (e.g.
hint: 'git pull ...') before pushing again.  
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (main)
$ git checkout ft/home-page-redesign
Switched to branch 'ft/home-page-redesign'
M       README.md

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (ft/home-page-redesign)      
$ git log
commit f986578fe2e009932a4110a7b3a56a8e78dc258e (HEAD -> ft/home-page-redesign, origin/ft/faq-page, ft/faq-page)
Author: jordandidit <jordygashagaza@gmail.com>
Date:   Sat May 20 15:41:10 2023 +0200       

     add faq page

commit f79347d7841ce69bebe15e2696545aa320eb6fd5 (origin/ft/contact-page, ft/contact-page) 
Author: jordandidit <jordygashagaza@gmail.com

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (ft/home-page-redesign)      
$ git rebase main
error: cannot rebase: You have unstaged changes.
error: Please commit or stash them.

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (ft/home-page-redesign)      
$ git stash main
fatal: subcommand wasn't specified; 'push' can't be assumed due to unexpected token 'main'

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (ft/home-page-redesign)      
$ git rebase main
error: cannot rebase: You have unstaged changes.
error: Please commit or stash them.

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (ft/home-page-redesign)      
$ git add home.html

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (ft/home-page-redesign)      
$ git commit -m "home html"
[ft/home-page-redesign 7ebec43] home html
 1 file changed, 17 insertions(+)
 create mode 100644 home.html

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (ft/home-page-redesign)      
$ git rebase main
error: cannot rebase: You have unstaged changes.
error: Please commit or stash them.

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (ft/home-page-redesign)      
$ git add home.html

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (ft/home-page-redesign)      
$ git commit -m "added menus on home"
On branch ft/home-page-redesign
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (ft/home-page-redesign)      
$ git push
fatal: The current branch ft/home-page-redesign has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/home-page-redesign

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (ft/home-page-redesign)      
$ git push --set-upstream origin ft/home-page-redesign
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads      
Compressing objects: 100% (3/3), done.       
Writing objects: 100% (3/3), 501 bytes | 501.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote: 
remote: Create a pull request for 'ft/home-page-redesign' on GitHub by visiting:
remote:      https://github.com/jordandidit/git-exercises/pull/new/ft/home-page-redesign  
remote:
To https://github.com/jordandidit/git-exercises.git
 * [new branch]      ft/home-page-redesign -> ft/home-page-redesign
branch 'ft/home-page-redesign' set up to track 'origin/ft/home-page-redesign'.

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (ft/home-page-redesign)      
$  git checkout ft/home-page-redesign
Already on 'ft/home-page-redesign'
M       README.md
Your branch is up to date with 'origin/ft/home-page-redesign'.

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (ft/home-page-redesign)      
$ git push --set-upstream origin ft/home-page
-redesign
Everything up-to-date
branch 'ft/home-page-redesign' set up to track 'origin/ft/home-page-redesign'.

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (ft/home-page-redesign)      
$ git checkout -b ft/merge
Switched to a new branch 'ft/merge'

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (ft/merge)
$ git status
On branch ft/merge
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (ft/merge)
$ git status
On branch ft/merge
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")
Auto-merging home.html
CONFLICT (add/add): Merge conflict in home.html
Automatic merge failed; fix conflicts and then commit the result.

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (ft/merge|MERGING)
$

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (ft/merge|MERGING)
$ git checkout ft/home-page-redesign
error: you need to resolve your current index first
home.html: needs merge

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (ft/merge|MERGING)
$ git checkout ft/home-page-redesign
Switched to branch 'ft/home-page-redesign'
M       README.md
Your branch is behind 'origin/ft/home-page-redesign' by 1 commit, and can be fast-forwarded.
  (use "git pull" to update your local branch)

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (ft/home-page-redesign)
$ git log
commit 7ebec433ea1c7f2c667a77a1390468cec98ecd76 (HEAD -> ft/home-page
commit 7ebec433ea1c7f2c667a77a1390468cec98ecd76 (HEAD -> ft/home-page-redesign)
Author: jordandidit <jordygashagaza@gmail.com>
Date:   Sat May 20 15:54:33 2023 +0200

    home html

commit f986578fe2e009932a4110a7b3a56a8e78dc258e (origin/ft/faq-page, ft/faq-page)
Author: jordandidit <jordygashagaza@gmail.com>
Date:   Sat May 20 15:41:10 2023 +0200


FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (ft/home-page-redesign)
$
