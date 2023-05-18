########BUNDLE 2##########33
EXERCISE 1 & 2



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
