
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

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (master)
$ git status
On branch master
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        CONSOLE_LOG.md

nothing added to commit but untracked files present (use "git add" to track)

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (master)
$ git add CONSOLE_LOG.md

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (master)
$ git commit -m "Concole_log.md added"
[master f8c18c5] Concole_log.md added
 1 file changed, 177 insertions(+)
 create mode 100644 CONSOLE_LOG.md

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (master)
$ git log
commit f8c18c5510be10b6bdab34f3105a73ef13923e75 (HEAD -> master)
Author: Ina Krasnokutska <inessa.krasnokutska@gmail.com>
Date:   Thu Mar 31 00:06:24 2022 +0300

    Concole_log.md added

commit 1b4a86c1259ff44b9518de6db6b925fb5fa89730
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

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (master)
$ ^[[200~git remote add origin https://github.com/InaKrasnokutska/sample_git_repo.git~bash: $'\E[200~git': command not found

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (master)
$ git remote add origin https://github.com/InaKrasnokutska/sample_git_repo.git

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (master)
$ git branch -M main

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (main)
$ git push -u origin main
Enumerating objects: 9, done.
Counting objects: 100% (9/9), done.
Delta compression using up to 8 threads
Compressing objects: 100% (5/5), done.
Writing objects: 100% (9/9), 1.76 KiB | 1.76 MiB/s, done.
Total 9 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/InaKrasnokutska/sample_git_repo.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        .gitignore

nothing added to commit but untracked files present (use "git add" to track)

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (main)
$ git add .gitignore

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (main)
$ git commit -m ".gitignore was added"
[main 32bcc40] .gitignore was added
 1 file changed, 24 insertions(+)
 create mode 100644 .gitignore

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (main)
$ git push
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 524 bytes | 262.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/InaKrasnokutska/sample_git_repo.git
   f8c18c5..32bcc40  main -> main

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (main)
$ git restore README.md

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (main)
$ git add README.md

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   README.md


Zver@Inka MINGW64 /d/work/Git/sample-git-repo (main)
$ git restore --staged README.md

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (main)
$ git restore README.md

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (main)
$ git log
commit 32bcc40a30a9b2bb10e8e80dd1cd0030e9c45bcd (HEAD -> main, origin/main)
Author: Ina Krasnokutska <inessa.krasnokutska@gmail.com>
Date:   Thu Mar 31 00:34:52 2022 +0300

    .gitignore was added

commit f8c18c5510be10b6bdab34f3105a73ef13923e75
Author: Ina Krasnokutska <inessa.krasnokutska@gmail.com>
Date:   Thu Mar 31 00:06:24 2022 +0300

    Concole_log.md added

commit 1b4a86c1259ff44b9518de6db6b925fb5fa89730
Author: Ina Krasnokutska <inessa.krasnokutska@gmail.com>
Date:   Wed Mar 30 23:57:16 2022 +0300

    Added 2 lines to README.md

commit 68b4a0b551cf4e6cf340a35cc7833191a0852e36
Author: Ina Krasnokutska <inessa.krasnokutska@gmail.com>
Date:   Wed Mar 30 23:52:34 2022 +0300

     On branch master

     Initial commit


Zver@Inka MINGW64 /d/work/Git/sample-git-repo (main)
$ git branch iss53

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (main)
$ git branch
  iss53
* main

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (main)
$ git log
commit 32bcc40a30a9b2bb10e8e80dd1cd0030e9c45bcd (HEAD -> main, origin/main, iss53)
Author: Ina Krasnokutska <inessa.krasnokutska@gmail.com>
Date:   Thu Mar 31 00:34:52 2022 +0300

    .gitignore was added

commit f8c18c5510be10b6bdab34f3105a73ef13923e75
Author: Ina Krasnokutska <inessa.krasnokutska@gmail.com>
Date:   Thu Mar 31 00:06:24 2022 +0300

    Concole_log.md added

commit 1b4a86c1259ff44b9518de6db6b925fb5fa89730
Author: Ina Krasnokutska <inessa.krasnokutska@gmail.com>
Date:   Wed Mar 30 23:57:16 2022 +0300

    Added 2 lines to README.md

commit 68b4a0b551cf4e6cf340a35cc7833191a0852e36
Author: Ina Krasnokutska <inessa.krasnokutska@gmail.com>
Date:   Wed Mar 30 23:52:34 2022 +0300

     On branch master

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (main)
$ git chechout iss53
git: 'chechout' is not a git command. See 'git --help'.

The most similar command is
        checkout

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (main)
$ git log
commit 32bcc40a30a9b2bb10e8e80dd1cd0030e9c45bcd (HEAD -> main, origin/main, iss53)
Author: Ina Krasnokutska <inessa.krasnokutska@gmail.com>
Date:   Thu Mar 31 00:34:52 2022 +0300

    .gitignore was added

commit f8c18c5510be10b6bdab34f3105a73ef13923e75
Author: Ina Krasnokutska <inessa.krasnokutska@gmail.com>
Date:   Thu Mar 31 00:06:24 2022 +0300

    Concole_log.md added

commit 1b4a86c1259ff44b9518de6db6b925fb5fa89730
Author: Ina Krasnokutska <inessa.krasnokutska@gmail.com>
Date:   Wed Mar 30 23:57:16 2022 +0300

    Added 2 lines to README.md

commit 68b4a0b551cf4e6cf340a35cc7833191a0852e36
Author: Ina Krasnokutska <inessa.krasnokutska@gmail.com>
Date:   Wed Mar 30 23:52:34 2022 +0300

     On branch master

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (main)
$ q
bash: q: command not found

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (main)
$ git chechout iss53
git: 'chechout' is not a git command. See 'git --help'.

The most similar command is
        checkout

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (main)
$ git checkout iss53
Switched to branch 'iss53'

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (iss53)
$ git log
commit 32bcc40a30a9b2bb10e8e80dd1cd0030e9c45bcd (HEAD -> iss53, origin/main, main)
Author: Ina Krasnokutska <inessa.krasnokutska@gmail.com>
Date:   Thu Mar 31 00:34:52 2022 +0300

    .gitignore was added

commit f8c18c5510be10b6bdab34f3105a73ef13923e75
Author: Ina Krasnokutska <inessa.krasnokutska@gmail.com>
Date:   Thu Mar 31 00:06:24 2022 +0300

    Concole_log.md added

commit 1b4a86c1259ff44b9518de6db6b925fb5fa89730
Author: Ina Krasnokutska <inessa.krasnokutska@gmail.com>
Date:   Wed Mar 30 23:57:16 2022 +0300

    Added 2 lines to README.md

commit 68b4a0b551cf4e6cf340a35cc7833191a0852e36
Author: Ina Krasnokutska <inessa.krasnokutska@gmail.com>
Date:   Wed Mar 30 23:52:34 2022 +0300

     On branch master
q
Zver@Inka MINGW64 /d/work/Git/sample-git-repo (iss53)
$ touch LICENCE.md

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (iss53)
$ git status
On branch iss53
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        LICENCE.md

nothing added to commit but untracked files present (use "git add" to track)

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (iss53)
$ git add LICENCE.md

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (iss53)
$ git commit -m "Added LICENCE.md"
[iss53 a823c54] Added LICENCE.md
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 LICENCE.md

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (iss53)
$ git status
On branch iss53
nothing to commit, working tree clean

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (iss53)
$ git log
commit a823c5403809cea8d2768cea4d8dbf0a34ccee19 (HEAD -> iss53)
Author: Ina Krasnokutska <inessa.krasnokutska@gmail.com>
Date:   Thu Mar 31 00:48:45 2022 +0300

    Added LICENCE.md

commit 32bcc40a30a9b2bb10e8e80dd1cd0030e9c45bcd (origin/main, main)
Author: Ina Krasnokutska <inessa.krasnokutska@gmail.com>
Date:   Thu Mar 31 00:34:52 2022 +0300

    .gitignore was added

commit f8c18c5510be10b6bdab34f3105a73ef13923e75
Author: Ina Krasnokutska <inessa.krasnokutska@gmail.com>
Date:   Thu Mar 31 00:06:24 2022 +0300

    Concole_log.md added

commit 1b4a86c1259ff44b9518de6db6b925fb5fa89730
Author: Ina Krasnokutska <inessa.krasnokutska@gmail.com>
Date:   Wed Mar 30 23:57:16 2022 +0300

    Added 2 lines to README.md

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (iss53)
$ ls
CONSOLE_LOG.md  LICENCE.md  README.md

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (iss53)
$ git checkout master
error: pathspec 'master' did not match any file(s) known to git

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (iss53)
$ git status
On branch iss53
nothing to commit, working tree clean

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (iss53)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (main)
$ ls
CONSOLE_LOG.md  README.md

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (main)
$ git checkout -b hotfix
Switched to a new branch 'hotfix'

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (hotfix)
$ git branch
* hotfix
  iss53
  main

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (hotfix)
$ git log
commit 32bcc40a30a9b2bb10e8e80dd1cd0030e9c45bcd (HEAD -> hotfix, origin/main, main)
Author: Ina Krasnokutska <inessa.krasnokutska@gmail.com>
Date:   Thu Mar 31 00:34:52 2022 +0300

    .gitignore was added

commit f8c18c5510be10b6bdab34f3105a73ef13923e75
Author: Ina Krasnokutska <inessa.krasnokutska@gmail.com>
Date:   Thu Mar 31 00:06:24 2022 +0300

    Concole_log.md added

commit 1b4a86c1259ff44b9518de6db6b925fb5fa89730
Author: Ina Krasnokutska <inessa.krasnokutska@gmail.com>
Date:   Wed Mar 30 23:57:16 2022 +0300

    Added 2 lines to README.md

commit 68b4a0b551cf4e6cf340a35cc7833191a0852e36
Author: Ina Krasnokutska <inessa.krasnokutska@gmail.com>
Date:   Wed Mar 30 23:52:34 2022 +0300

     On branch master

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (hotfix)
$ vi README.md

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (hotfix)
$ git status
On branch hotfix
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (hotfix)
$ git add README.md

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (hotfix)
$ git status
On branch hotfix
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   README.md


Zver@Inka MINGW64 /d/work/Git/sample-git-repo (hotfix)
$ git commit -m "Hotfix"
[hotfix 1da9ab7] Hotfix
 1 file changed, 3 insertions(+), 1 deletion(-)

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (hotfix)
$ git log
commit 1da9ab7c8553196368fd4d89125a6793da4c3515 (HEAD -> hotfix)
Author: Ina Krasnokutska <inessa.krasnokutska@gmail.com>
Date:   Thu Mar 31 00:52:54 2022 +0300

    Hotfix

commit 32bcc40a30a9b2bb10e8e80dd1cd0030e9c45bcd (origin/main, main)
Author: Ina Krasnokutska <inessa.krasnokutska@gmail.com>
Date:   Thu Mar 31 00:34:52 2022 +0300

    .gitignore was added

commit f8c18c5510be10b6bdab34f3105a73ef13923e75
Author: Ina Krasnokutska <inessa.krasnokutska@gmail.com>
Date:   Thu Mar 31 00:06:24 2022 +0300

    Concole_log.md added

commit 1b4a86c1259ff44b9518de6db6b925fb5fa89730
Author: Ina Krasnokutska <inessa.krasnokutska@gmail.com>
Date:   Wed Mar 30 23:57:16 2022 +0300

    Added 2 lines to README.md
q
Zver@Inka MINGW64 /d/work/Git/sample-git-repo (hotfix)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (main)
$ git merge hotfix
Updating 32bcc40..1da9ab7
Fast-forward
 README.md | 4 +++-
 1 file changed, 3 insertions(+), 1 deletion(-)

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (main)
$ git log
commit 1da9ab7c8553196368fd4d89125a6793da4c3515 (HEAD -> main, hotfix)
Author: Ina Krasnokutska <inessa.krasnokutska@gmail.com>
Date:   Thu Mar 31 00:52:54 2022 +0300

    Hotfix

commit 32bcc40a30a9b2bb10e8e80dd1cd0030e9c45bcd (origin/main)
Author: Ina Krasnokutska <inessa.krasnokutska@gmail.com>
Date:   Thu Mar 31 00:34:52 2022 +0300

    .gitignore was added

commit f8c18c5510be10b6bdab34f3105a73ef13923e75
Author: Ina Krasnokutska <inessa.krasnokutska@gmail.com>
Date:   Thu Mar 31 00:06:24 2022 +0300

    Concole_log.md added

commit 1b4a86c1259ff44b9518de6db6b925fb5fa89730
Author: Ina Krasnokutska <inessa.krasnokutska@gmail.com>
Date:   Wed Mar 30 23:57:16 2022 +0300

    Added 2 lines to README.md
q
Zver@Inka MINGW64 /d/work/Git/sample-git-repo (main)
$ git branch -d hotfix
Deleted branch hotfix (was 1da9ab7).

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (main)
$ git log
commit 1da9ab7c8553196368fd4d89125a6793da4c3515 (HEAD -> main)
Author: Ina Krasnokutska <inessa.krasnokutska@gmail.com>
Date:   Thu Mar 31 00:52:54 2022 +0300

    Hotfix

commit 32bcc40a30a9b2bb10e8e80dd1cd0030e9c45bcd (origin/main)
Author: Ina Krasnokutska <inessa.krasnokutska@gmail.com>
Date:   Thu Mar 31 00:34:52 2022 +0300

    .gitignore was added

commit f8c18c5510be10b6bdab34f3105a73ef13923e75
Author: Ina Krasnokutska <inessa.krasnokutska@gmail.com>
Date:   Thu Mar 31 00:06:24 2022 +0300

    Concole_log.md added

commit 1b4a86c1259ff44b9518de6db6b925fb5fa89730
Author: Ina Krasnokutska <inessa.krasnokutska@gmail.com>
Date:   Wed Mar 30 23:57:16 2022 +0300

    Added 2 lines to README.md
q
Zver@Inka MINGW64 /d/work/Git/sample-git-repo (main)
$ git branch
  iss53
* main

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (main)
$ git checkout iss53
Switched to branch 'iss53'

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (iss53)
$ echo "LICENSE" > LICENCE.md

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (iss53)
$ git status
On branch iss53
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   LICENCE.md

no changes added to commit (use "git add" and/or "git commit -a")

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (iss53)
$ git commit -a -m "Changed LICENCE.md"
warning: LF will be replaced by CRLF in LICENCE.md.
The file will have its original line endings in your working directory
[iss53 57d8438] Changed LICENCE.md
 1 file changed, 1 insertion(+)

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (iss53)
$ git status
On branch iss53
nothing to commit, working tree clean

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (iss53)
$ git log
commit 57d84389edb4c82a2742d66fa5901543597a47b2 (HEAD -> iss53)
Author: Ina Krasnokutska <inessa.krasnokutska@gmail.com>
Date:   Thu Mar 31 00:57:00 2022 +0300

    Changed LICENCE.md

commit a823c5403809cea8d2768cea4d8dbf0a34ccee19
Author: Ina Krasnokutska <inessa.krasnokutska@gmail.com>
Date:   Thu Mar 31 00:48:45 2022 +0300

    Added LICENCE.md

commit 32bcc40a30a9b2bb10e8e80dd1cd0030e9c45bcd (origin/main)
Author: Ina Krasnokutska <inessa.krasnokutska@gmail.com>
Date:   Thu Mar 31 00:34:52 2022 +0300

    .gitignore was added

commit f8c18c5510be10b6bdab34f3105a73ef13923e75
Author: Ina Krasnokutska <inessa.krasnokutska@gmail.com>
Date:   Thu Mar 31 00:06:24 2022 +0300

    Concole_log.md added
q
Zver@Inka MINGW64 /d/work/Git/sample-git-repo (iss53)
$ git checkout main
Switched to branch 'main'
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (main)
$ git merge iss53
Merge made by the 'ort' strategy.
 LICENCE.md | 1 +
 1 file changed, 1 insertion(+)
 create mode 100644 LICENCE.md

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (main)
$ git branch -d iss53
Deleted branch iss53 (was 57d8438).

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (main)
$ git branch
* main

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (main)
$ git checkout -b iss55
Switched to a new branch 'iss55'

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (iss55)
$ git branch
* iss55
  main

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (iss55)
$ ls
CONSOLE_LOG.md  LICENCE.md  README.md

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (iss55)
$ echo "ISS55" > LICENCE.md

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (iss55)
$ cat LICENCE.md
ISS55

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (iss55)
$ git status
On branch iss55
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   LICENCE.md

no changes added to commit (use "git add" and/or "git commit -a")

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (iss55)
$ git commit -a -m "changes in iss55"
warning: LF will be replaced by CRLF in LICENCE.md.
The file will have its original line endings in your working directory
[iss55 26f94b7] changes in iss55
 1 file changed, 1 insertion(+), 1 deletion(-)

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (iss55)
$ git checkout main
Switched to branch 'main'
Your branch is ahead of 'origin/main' by 4 commits.
  (use "git push" to publish your local commits)

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (main)
$ echo "MASTER" > LICENCE.md

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (main)
$ cat LICENCE.md
MASTER

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (main)
$ git commit -a -m "changes in master"
warning: LF will be replaced by CRLF in LICENCE.md.
The file will have its original line endings in your working directory
[main 36a30dc] changes in master
 1 file changed, 1 insertion(+), 1 deletion(-)

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (main)
$ git merge iss55
Auto-merging LICENCE.md
CONFLICT (content): Merge conflict in LICENCE.md
Automatic merge failed; fix conflicts and then commit the result.

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (main|MERGING)
$ git status
On branch main
Your branch is ahead of 'origin/main' by 5 commits.
  (use "git push" to publish your local commits)

You have unmerged paths.
  (fix conflicts and run "git commit")
  (use "git merge --abort" to abort the merge)

Unmerged paths:
  (use "git add <file>..." to mark resolution)
        both modified:   LICENCE.md

no changes added to commit (use "git add" and/or "git commit -a")

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (main|MERGING)
$ vi LICENCE.md

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (main|MERGING)
$ git status
On branch main
Your branch is ahead of 'origin/main' by 5 commits.
  (use "git push" to publish your local commits)

You have unmerged paths.
  (fix conflicts and run "git commit")
  (use "git merge --abort" to abort the merge)

Unmerged paths:
  (use "git add <file>..." to mark resolution)
        both modified:   LICENCE.md

no changes added to commit (use "git add" and/or "git commit -a")

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (main|MERGING)
$ git add LiCENCE.md

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (main|MERGING)
$ git status
On branch main
Your branch is ahead of 'origin/main' by 5 commits.
  (use "git push" to publish your local commits)

You have unmerged paths.
  (fix conflicts and run "git commit")
  (use "git merge --abort" to abort the merge)

Unmerged paths:
  (use "git add <file>..." to mark resolution)
        both modified:   LICENCE.md

no changes added to commit (use "git add" and/or "git commit -a")

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (main|MERGING)
$ git add LICENCE.md

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (main|MERGING)
$ git status
On branch main
Your branch is ahead of 'origin/main' by 5 commits.
  (use "git push" to publish your local commits)

All conflicts fixed but you are still merging.
  (use "git commit" to conclude merge)

Changes to be committed:
        modified:   LICENCE.md


Zver@Inka MINGW64 /d/work/Git/sample-git-repo (main|MERGING)
$ git commit -m "Merge iss55 into master"
[main 8983af0] Merge iss55 into master

Zver@Inka MINGW64 /d/work/Git/sample-git-repo (main)
$ git log
commit 8983af0ee3c42b586dc5d930799a7fb80460bd80 (HEAD -> main)
Merge: 36a30dc 26f94b7
Author: Ina Krasnokutska <inessa.krasnokutska@gmail.com>
Date:   Thu Mar 31 01:07:52 2022 +0300

    Merge iss55 into master

commit 36a30dcdfc49a33f8ab9740ec80938f8d1871259
Author: Ina Krasnokutska <inessa.krasnokutska@gmail.com>
Date:   Thu Mar 31 01:03:29 2022 +0300

    changes in master

commit 26f94b7836ebf88edb7a9ee1fdc608f20ce6a0f6 (iss55)
Author: Ina Krasnokutska <inessa.krasnokutska@gmail.com>
Date:   Thu Mar 31 01:02:20 2022 +0300

    changes in iss55

commit 600d87924c0e06a764d258d5b7fe2e7f63b49b1d
Merge: 1da9ab7 57d8438
Author: Ina Krasnokutska <inessa.krasnokutska@gmail.com>
Date:   Thu Mar 31 00:58:14 2022 +0300
