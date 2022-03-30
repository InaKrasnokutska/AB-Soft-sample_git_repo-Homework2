
Zver@Inka MINGW64 /d/work/Git
$ mkdir sample-git-repo

Zver@Inka MINGW64 /d/work/Git
$ cd sample-git-repo/

Zver@Inka MINGW64 /d/work/Git/sample-git-repo
$ touch README.md

Zver@Inka MINGW64 /d/work/Git/sample-git-repo
$ git init
Initialized empty Git repository in D:/work/Git/sample-git-repo/.git/

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (master)
$ ls -la
total 4
drwxr-xr-x 1 Zver 197121 0 Mar 30 23:50 ./
drwxr-xr-x 1 Zver 197121 0 Mar 30 23:49 ../
drwxr-xr-x 1 Zver 197121 0 Mar 30 23:50 .git/
-rw-r--r-- 1 Zver 197121 0 Mar 30 23:50 README.md

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (master)
$ git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        README.md

nothing added to commit but untracked files present (use "git add" to track)

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (master)
$ git add README.md

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (master)
$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   README.md


Zver@Inka MINGW64 /d/work/Git/sample-git-repo (master)
$ git commit
[master (root-commit) 68b4a0b]  On branch master
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 README.md

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (master)
$ git status

On branch master
nothing to commit, working tree clean

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (master)
$

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (master)
$ git status
On branch master
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (master)
$ git diff
diff --git a/README.md b/README.md
index e69de29..02fa806 100644
--- a/README.md
+++ b/README.md
@@ -0,0 +1 @@
+# Sample Git Repo
\ No newline at end of file

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (master)
$ git commit -a -m "Added line to README.md"
[master e239db4] Added line to README.md
 1 file changed, 1 insertion(+)

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (master)
$ git log
commit e239db4ccf6b6b9b9c773160068db3566ec48309 (HEAD -> master)
Author: Ina Krasnokutska <inessa.krasnokutska@gmail.com>
Date:   Wed Mar 30 23:57:16 2022 +0300

    Added line to README.md

commit 68b4a0b551cf4e6cf340a35cc7833191a0852e36
Author: Ina Krasnokutska <inessa.krasnokutska@gmail.com>
Date:   Wed Mar 30 23:52:34 2022 +0300

     On branch master

     Initial commit

     Changes to be committed:
            new file:   README.md

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (master)
$ git status
On branch master
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (master)
$ git add README.md
g
Zver@Inka MINGW64 /d/work/Git/sample-git-repo (master)
$ git status
On branch master
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   README.md


Zver@Inka MINGW64 /d/work/Git/sample-git-repo (master)
$ git commit --amend
[master c9a2257] Added line to README.md
 Date: Wed Mar 30 23:57:16 2022 +0300
 1 file changed, 3 insertions(+)

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (master)
$ git log
commit c9a22573449230d0227353b13d7710988cab67aa (HEAD -> master)
Author: Ina Krasnokutska <inessa.krasnokutska@gmail.com>
Date:   Wed Mar 30 23:57:16 2022 +0300

    Added line to README.md

commit 68b4a0b551cf4e6cf340a35cc7833191a0852e36
Author: Ina Krasnokutska <inessa.krasnokutska@gmail.com>
Date:   Wed Mar 30 23:52:34 2022 +0300

     On branch master

     Initial commit

     Changes to be committed:
            new file:   README.md

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (master)
$ git commit --amend
[master 1b4a86c] Added 2 lines to README.md
 Date: Wed Mar 30 23:57:16 2022 +0300
 1 file changed, 3 insertions(+)

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (master)
$ git log
commit 1b4a86c1259ff44b9518de6db6b925fb5fa89730 (HEAD -> master)
Author: Ina Krasnokutska <inessa.krasnokutska@gmail.com>
Date:   Wed Mar 30 23:57:16 2022 +0300

    Added 2 lines to README.md

commit 68b4a0b551cf4e6cf340a35cc7833191a0852e36
Author: Ina Krasnokutska <inessa.krasnokutska@gmail.com>
Date:   Wed Mar 30 23:52:34 2022 +0300

     On branch master

     Initial commit

     Changes to be committed:
            new file:   README.md
