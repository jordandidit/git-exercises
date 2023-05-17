# git-exercises-BUNDLE 1 EXERCISE 2"



FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (dev)
$ git init
Reinitialized existing Git repository in C:/Users/FALCON/Downloads/the gym rwanda files/git/.git/

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (dev)
$ git status
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   .vscode/settings.json
        new file:   read me.md

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        about.html
        home.html
        team.html


FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (dev)
$ git add about.html

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (dev)
$ git add home.html

FALCON@Jordanpc MINGW64 ~/Downloads/the gym rwanda files/git (dev)
$ git add team.html

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
Counting objects: 100% (12/12), done.
Delta compression using up to 8 threads
Compressing objects: 100% (9/9), done.
Writing objects: 100% (11/11), 1.24 KiB | 127.00 KiB/s, done.
Total 11 (delta 3), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (3/3), done.
To https://github.com/jordandidit/git-exercises.git
   47fe311..538653c  dev -> dev
branch 'dev' set up to track 'origin/dev'.
