# learning-git-2
https://lankiewicz.github.io/learning-git-2/
{code}
JakubL@DESKTOP-HI6G1OG MINGW64 ~/Desktop
$ cd learning-git-2/

JakubL@DESKTOP-HI6G1OG MINGW64 ~/Desktop/learning-git-2 (master)
$ git tree
* bc37d52 (HEAD -> master, origin/master) sprawdzam cos tylko
* 6e84eb7 (tag: task-3-finished) add third verbs
* d4e7e41 add second verse
* c78bce0 add verse of song
* 519f158 Add style for new
* da0d2c4 Add basic html code
* ce5c8fd Init project

JakubL@DESKTOP-HI6G1OG MINGW64 ~/Desktop/learning-git-2 (master)
$ git branch task-4

JakubL@DESKTOP-HI6G1OG MINGW64 ~/Desktop/learning-git-2 (master)
$ touch .gitignore

JakubL@DESKTOP-HI6G1OG MINGW64 ~/Desktop/learning-git-2 (master)
$ git status
On branch master
Your branch is up to date with 'origin/master'.

Changes not staged for commit:
  (use "git add/rm <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

        modified:   index.html
        modified:   sass/.sass-cache/65f74e16b2d19f69e38998f1a705ae460074b101/style.scssc
        modified:   sass/style.css
        modified:   sass/style.css.map
        modified:   sass/style.scss
        deleted:    style.css

Untracked files:
  (use "git add <file>..." to include in what will be committed)

        .gitignore

no changes added to commit (use "git add" and/or "git commit -a")

JakubL@DESKTOP-HI6G1OG MINGW64 ~/Desktop/learning-git-2 (master)
$ echo ".sass-cache" > .gitignore

JakubL@DESKTOP-HI6G1OG MINGW64 ~/Desktop/learning-git-2 (master)
$ git status
On branch master
Your branch is up to date with 'origin/master'.

Changes not staged for commit:
  (use "git add/rm <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

        modified:   index.html
        modified:   sass/.sass-cache/65f74e16b2d19f69e38998f1a705ae460074b101/style.scssc
        modified:   sass/style.css
        modified:   sass/style.css.map
        modified:   sass/style.scss
        deleted:    style.css

Untracked files:
  (use "git add <file>..." to include in what will be committed)

        .gitignore

no changes added to commit (use "git add" and/or "git commit -a")

JakubL@DESKTOP-HI6G1OG MINGW64 ~/Desktop/learning-git-2 (master)
$ touch .sass-cache

JakubL@DESKTOP-HI6G1OG MINGW64 ~/Desktop/learning-git-2 (master)
$ git status
On branch master
Your branch is up to date with 'origin/master'.

Changes not staged for commit:
  (use "git add/rm <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

        modified:   index.html
        modified:   sass/.sass-cache/65f74e16b2d19f69e38998f1a705ae460074b101/style.scssc
        modified:   sass/style.css
        modified:   sass/style.css.map
        modified:   sass/style.scss
        deleted:    style.css

Untracked files:
  (use "git add <file>..." to include in what will be committed)

        .gitignore

no changes added to commit (use "git add" and/or "git commit -a")

JakubL@DESKTOP-HI6G1OG MINGW64 ~/Desktop/learning-git-2 (master)
$ echo ".sass-cache" > .gitignore

JakubL@DESKTOP-HI6G1OG MINGW64 ~/Desktop/learning-git-2 (master)
$ git status
On branch master
Your branch is up to date with 'origin/master'.

Changes not staged for commit:
  (use "git add/rm <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

        modified:   index.html
        modified:   sass/.sass-cache/65f74e16b2d19f69e38998f1a705ae460074b101/style.scssc
        modified:   sass/style.css
        modified:   sass/style.css.map
        modified:   sass/style.scss
        deleted:    style.css

Untracked files:
  (use "git add <file>..." to include in what will be committed)

        .gitignore

no changes added to commit (use "git add" and/or "git commit -a")

JakubL@DESKTOP-HI6G1OG MINGW64 ~/Desktop/learning-git-2 (master)
$ git branch Kuba

JakubL@DESKTOP-HI6G1OG MINGW64 ~/Desktop/learning-git-2 (master)
$ git branch Ania

JakubL@DESKTOP-HI6G1OG MINGW64 ~/Desktop/learning-git-2 (master)
$ git checkout Kuba
Switched to branch 'Kuba'
M       index.html
M       sass/.sass-cache/65f74e16b2d19f69e38998f1a705ae460074b101/style.scssc
M       sass/style.css
M       sass/style.css.map
M       sass/style.scss
D       style.css

JakubL@DESKTOP-HI6G1OG MINGW64 ~/Desktop/learning-git-2 (Kuba)
$ git add . && git commit - m "remove h1 and add style for section"
warning: LF will be replaced by CRLF in .gitignore.
The file will have its original line endings in your working directory.
error: pathspec '-' did not match any file(s) known to git.
error: pathspec 'm' did not match any file(s) known to git.
error: pathspec 'remove h1 and add style for section' did not match any file(s) known to git.

JakubL@DESKTOP-HI6G1OG MINGW64 ~/Desktop/learning-git-2 (Kuba)
$ git tree
* bc37d52 (HEAD -> Kuba, origin/master, task-4, master, Ania) sprawdzam cos tylko
* 6e84eb7 (tag: task-3-finished) add third verbs
* d4e7e41 add second verse
* c78bce0 add verse of song
* 519f158 Add style for new
* da0d2c4 Add basic html code
* ce5c8fd Init project

JakubL@DESKTOP-HI6G1OG MINGW64 ~/Desktop/learning-git-2 (Kuba)
$ git add . && git commit -m "remove h1"
[Kuba 4fe7e3d] remove h1
 7 files changed, 31 insertions(+), 14 deletions(-)
 create mode 100644 .gitignore
 rewrite sass/.sass-cache/65f74e16b2d19f69e38998f1a705ae460074b101/style.scssc (84%)
 rewrite style.css (100%)

JakubL@DESKTOP-HI6G1OG MINGW64 ~/Desktop/learning-git-2 (Kuba)
$ git tree
* 4fe7e3d (HEAD -> Kuba) remove h1
* bc37d52 (origin/master, task-4, master, Ania) sprawdzam cos tylko
* 6e84eb7 (tag: task-3-finished) add third verbs
* d4e7e41 add second verse
* c78bce0 add verse of song
* 519f158 Add style for new
* da0d2c4 Add basic html code
* ce5c8fd Init project

JakubL@DESKTOP-HI6G1OG MINGW64 ~/Desktop/learning-git-2 (Kuba)
$ git checkout Ania
Switched to branch 'Ania'

JakubL@DESKTOP-HI6G1OG MINGW64 ~/Desktop/learning-git-2 (Ania)
$ git add . && git commit -m "same hchange"
[Ania 39b49de] same hchange
 3 files changed, 3 insertions(+), 5 deletions(-)
 create mode 100644 .sass-cache

JakubL@DESKTOP-HI6G1OG MINGW64 ~/Desktop/learning-git-2 (Ania)
$ git tree
* 39b49de (HEAD -> Ania) same hchange
* bc37d52 (origin/master, task-4, master) sprawdzam cos tylko
* 6e84eb7 (tag: task-3-finished) add third verbs
* d4e7e41 add second verse
* c78bce0 add verse of song
* 519f158 Add style for new
* da0d2c4 Add basic html code
* ce5c8fd Init project

JakubL@DESKTOP-HI6G1OG MINGW64 ~/Desktop/learning-git-2 (Ania)
$ git checkout master
Switched to branch 'master'
Your branch is up to date with 'origin/master'.

JakubL@DESKTOP-HI6G1OG MINGW64 ~/Desktop/learning-git-2 (master)
$ git tree --all
* 39b49de (Ania) same hchange
| * 4fe7e3d (Kuba) remove h1
|/
* bc37d52 (HEAD -> master, origin/master, task-4) sprawdzam cos tylko
* 6e84eb7 (tag: task-3-finished) add third verbs
* d4e7e41 add second verse
* c78bce0 add verse of song
* 519f158 Add style for new
* da0d2c4 Add basic html code
* ce5c8fd Init project

JakubL@DESKTOP-HI6G1OG MINGW64 ~/Desktop/learning-git-2 (master)
$ git merge Kuba
Updating bc37d52..4fe7e3d
Fast-forward
 .gitignore                                         |   1 +
 index.html                                         |   3 ++-
 .../style.scssc                                    | Bin 1926 -> 2165 bytes
 sass/style.css                                     |   7 ++----
 sass/style.css.map                                 |   2 +-
 sass/style.scss                                    |   5 ++--
 style.css                                          |  27 ++++++++++++++++++---
 7 files changed, 31 insertions(+), 14 deletions(-)
 create mode 100644 .gitignore

JakubL@DESKTOP-HI6G1OG MINGW64 ~/Desktop/learning-git-2 (master)
$ git tree --all
* 39b49de (Ania) same hchange
| * 4fe7e3d (HEAD -> master, Kuba) remove h1
|/
* bc37d52 (origin/master, task-4) sprawdzam cos tylko
* 6e84eb7 (tag: task-3-finished) add third verbs
* d4e7e41 add second verse
* c78bce0 add verse of song
* 519f158 Add style for new
* da0d2c4 Add basic html code
* ce5c8fd Init project

JakubL@DESKTOP-HI6G1OG MINGW64 ~/Desktop/learning-git-2 (master)
$ git merge Ania
Auto-merging sass/style.css
CONFLICT (content): Merge conflict in sass/style.css
Automatic merge failed; fix conflicts and then commit the result.

JakubL@DESKTOP-HI6G1OG MINGW64 ~/Desktop/learning-git-2 (master|MERGING)
$ git merge Kuba
error: Merging is not possible because you have unmerged files.
hint: Fix them up in the work tree, and then use 'git add/rm <file>'
hint: as appropriate to mark resolution and make a commit.
fatal: Exiting because of an unresolved conflict.

JakubL@DESKTOP-HI6G1OG MINGW64 ~/Desktop/learning-git-2 (master|MERGING)
$ git add .

JakubL@DESKTOP-HI6G1OG MINGW64 ~/Desktop/learning-git-2 (master|MERGING)
$ git commit
[master 96547b5] Merge branch 'Ania'

JakubL@DESKTOP-HI6G1OG MINGW64 ~/Desktop/learning-git-2 (master)
$ git tree --all
*   96547b5 (HEAD -> master) Merge branch 'Ania'
|\
| * 39b49de (Ania) same hchange
* | 4fe7e3d (Kuba) remove h1
|/
* bc37d52 (origin/master, task-4) sprawdzam cos tylko
* 6e84eb7 (tag: task-3-finished) add third verbs
* d4e7e41 add second verse
* c78bce0 add verse of song
* 519f158 Add style for new
* da0d2c4 Add basic html code
* ce5c8fd Init project

JakubL@DESKTOP-HI6G1OG MINGW64 ~/Desktop/learning-git-2 (master)
$ git merge Kuba
Already up to date.

JakubL@DESKTOP-HI6G1OG MINGW64 ~/Desktop/learning-git-2 (master)
$ git tree --all
*   96547b5 (HEAD -> master) Merge branch 'Ania'
|\
| * 39b49de (Ania) same hchange
* | 4fe7e3d (Kuba) remove h1
|/
* bc37d52 (origin/master, task-4) sprawdzam cos tylko
* 6e84eb7 (tag: task-3-finished) add third verbs
* d4e7e41 add second verse
* c78bce0 add verse of song
* 519f158 Add style for new
* da0d2c4 Add basic html code
* ce5c8fd Init project

JakubL@DESKTOP-HI6G1OG MINGW64 ~/Desktop/learning-git-2 (master)
$ git merge task-4
Already up to date.

JakubL@DESKTOP-HI6G1OG MINGW64 ~/Desktop/learning-git-2 (master)
$ git tree --all
*   96547b5 (HEAD -> master) Merge branch 'Ania'
|\
| * 39b49de (Ania) same hchange
* | 4fe7e3d (Kuba) remove h1
|/
* bc37d52 (origin/master, task-4) sprawdzam cos tylko
* 6e84eb7 (tag: task-3-finished) add third verbs
* d4e7e41 add second verse
* c78bce0 add verse of song
* 519f158 Add style for new
* da0d2c4 Add basic html code
* ce5c8fd Init project

JakubL@DESKTOP-HI6G1OG MINGW64 ~/Desktop/learning-git-2 (master)
$ git merge task-4
Already up to date.

JakubL@DESKTOP-HI6G1OG MINGW64 ~/Desktop/learning-git-2 (master)
$ git tree
*   96547b5 (HEAD -> master) Merge branch 'Ania'
|\
| * 39b49de (Ania) same hchange
* | 4fe7e3d (Kuba) remove h1
|/
* bc37d52 (origin/master, task-4) sprawdzam cos tylko
* 6e84eb7 (tag: task-3-finished) add third verbs
* d4e7e41 add second verse
* c78bce0 add verse of song
* 519f158 Add style for new
* da0d2c4 Add basic html code
* ce5c8fd Init project

JakubL@DESKTOP-HI6G1OG MINGW64 ~/Desktop/learning-git-2 (master)
{code}
