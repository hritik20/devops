ritik15@ritik15-Dell-15-DC15250:~/Documents/john savill devops$ ls
devops  DevOpsMC  git_demo
ritik15@ritik15-Dell-15-DC15250:~/Documents/john savill devops$ cd devops
ritik15@ritik15-Dell-15-DC15250:~/Documents/john savill devops/devops$ ls
git_commands.md  test.py
ritik15@ritik15-Dell-15-DC15250:~/Documents/john savill devops/devops$ cd ..
ritik15@ritik15-Dell-15-DC15250:~/Documents/john savill devops$ cd git_demo
ritik15@ritik15-Dell-15-DC15250:~/Documents/john savill devops/git_demo$ ls
devops
ritik15@ritik15-Dell-15-DC15250:~/Documents/john savill devops/git_demo$ cd devops
ritik15@ritik15-Dell-15-DC15250:~/Documents/john savill devops/git_demo/devops$ ls
ritik15@ritik15-Dell-15-DC15250:~/Documents/john savill devops/git_demo/devops$ git branch
* develop
  main
ritik15@ritik15-Dell-15-DC15250:~/Documents/john savill devops/git_demo/devops$ git log
commit 08a7cfd2cbb1f47dd2601cb1f7d723c550ddc237 (HEAD -> develop, origin/develop)
Author: ritik mishra <49184178+hritik20@users.noreply.github.com>
Date:   Sat May 16 16:17:23 2026 +0530

    Add message advocating for world peace

commit 7436f94ebd1ca1630f90b4d7f6807584f46a4db9
Author: Ritik <rishumishra231@gmail.com>
Date:   Sat May 16 16:14:41 2026 +0530

    file saved

commit 3d26deeea421026c861b66769eae4becf9955c54
Author: Ritik <rishumishra231@gmail.com>
Date:   Sat May 16 16:11:15 2026 +0530

    saved

commit d894ae4032369e6025f2a90f616744dbfc9c40d8
Author: Ritik <rishumishra231@gmail.com>
Date:   Sat May 16 16:05:01 2026 +0530

    saved

commit 79f721842b43e02b71687aad6c91030f654de8f5
Author: Ritik <rishumishra231@gmail.com>
Date:   Sat May 16 16:02:30 2026 +0530

    saved

commit b72259b3681e22e33a21f2b3bf6c1452eccad226 (origin/main, origin/HEAD, main)
Author: Ritik <rishumishra231@gmail.com>
Date:   Sat May 16 15:51:37 2026 +0530

    bkl.txt

commit 6fe6a6251e9443ec95c44139a9657a3af0a2372a
Author: Ritik <rishumishra231@gmail.com>
Date:   Sat May 16 15:49:48 2026 +0530

    bkl.txt

commit 19897d54c95dfc3bc5017066df30370b7a5425f6
Author: Ritik <rishumishra231@gmail.com>
Date:   Sat May 16 15:47:07 2026 +0530

    bkl.txt

commit 1ea6b34526c286e1a9d874617843ca70bcc95dc6
Author: Ritik <rishumishra231@gmail.com>
Date:   Sat May 16 14:32:29 2026 +0530

    bkl.txt

commit cfea18809b600013cf7581d1a4fa4ac652dd534e
Author: ritik mishra <49184178+hritik20@users.noreply.github.com>
Date:   Sat May 16 14:24:31 2026 +0530

    Create testing.py

commit 7b24945272c3335513937c25608da8a34c9982a0
Author: ritik mishra <49184178+hritik20@users.noreply.github.com>
Date:   Sat May 16 01:54:04 2026 +0530

    Initial commit

[1]+  Stopped                 git log
ritik15@ritik15-Dell-15-DC15250:~/Documents/john savill devops/git_demo/devops$ function gitgraph {git log --online --graph --decorate --all}
bash: syntax error near unexpected token `{git'
ritik15@ritik15-Dell-15-DC15250:~/Documents/john savill devops/git_demo/devops$ git log --oneline --graph --all
* 08a7cfd (HEAD -> develop, origin/develop) Add message advocating for world peace
* 7436f94 file saved
* 3d26dee saved
* d894ae4 saved
* 79f7218 saved
* b72259b (origin/main, origin/HEAD, main) bkl.txt
* 6fe6a62 bkl.txt
* 19897d5 bkl.txt
* 1ea6b34 bkl.txt
* cfea188 Create testing.py
* 7b24945 Initial commit
ritik15@ritik15-Dell-15-DC15250:~/Documents/john savill devops/git_demo/devops$ git diff 6fe6a62..1ea6b34
diff --git a/bkl.txt b/bkl.txt
index 403788f..93f0588 100644
--- a/bkl.txt
+++ b/bkl.txt
@@ -1,2 +1,2 @@
-Ramayana 
-Mahabharata
\ No newline at end of file
+hello bkl gand marao
+thank you
\ No newline at end of file
ritik15@ritik15-Dell-15-DC15250:~/Documents/john savill devops/git_demo/devops$ git status
On branch develop
Your branch is up to date with 'origin/develop'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
	key-gen
	key-gen.pub

nothing added to commit but untracked files present (use "git add" to track)
ritik15@ritik15-Dell-15-DC15250:~/Documents/john savill devops/git_demo/devops$ git diff --cache
error: invalid option: --cache
usage: git diff [<options>] [<commit>] [--] [<path>...]
   or: git diff [<options>] --cached [--merge-base] [<commit>] [--] [<path>...]
   or: git diff [<options>] [--merge-base] <commit> [<commit>...] <commit> [--] [<path>...]
   or: git diff [<options>] <commit>...<commit> [--] [<path>...]
   or: git diff [<options>] <blob> <blob>
   or: git diff [<options>] --no-index [--] <path> <path>

common diff options:
  -z            output diff-raw with lines terminated with NUL.
  -p            output patch format.
  -u            synonym for -p.
  --patch-with-raw
                output both a patch and the diff-raw format.
  --stat        show diffstat instead of patch.
  --numstat     show numeric diffstat instead of patch.
  --patch-with-stat
                output a patch and prepend its diffstat.
  --name-only   show only names of changed files.
  --name-status show names and status of changed files.
  --full-index  show full object name on index lines.
  --abbrev=<n>  abbreviate object names in diff-tree header and diff-raw.
  -R            swap input file pairs.
:
























error: invalid option: --cache
usage: git diff [<options>] [<commit>] [--] [<path>...]
   or: git diff [<options>] --cached [--merge-base] [<commit>] [--] [<path>...]
   or: git diff [<options>] [--merge-base] <commit> [<commit>...] <commit> [--] [<path>...]
   or: git diff [<options>] <commit>...<commit> [--] [<path>...]
   or: git diff [<options>] <blob> <blob>
   or: git diff [<options>] --no-index [--] <path> <path>

common diff options:
  -z            output diff-raw with lines terminated with NUL.
  -p            output patch format.
  -u            synonym for -p.
  --patch-with-raw
                output both a patch and the diff-raw format.
  --stat        show diffstat instead of patch.
  --numstat     show numeric diffstat instead of patch.
  --patch-with-stat
                output a patch and prepend its diffstat.
  --name-only   show only names of changed files.
  --name-status show names and status of changed files.
  --full-index  show full object name on index lines.
  --abbrev=<n>  abbreviate object names in diff-tree header and diff-raw.
  -R            swap input file pairs.

[2]+  Stopped                 git diff --cache
ritik15@ritik15-Dell-15-DC15250:~/Documents/john savill devops/git_demo/devops$ git diff --cached
ritik15@ritik15-Dell-15-DC15250:~/Documents/john savill devops/git_demo/devops$ ls
bkl.txt  key-gen  key-gen.pub  pack.py  README.md  testing.py  War
ritik15@ritik15-Dell-15-DC15250:~/Documents/john savill devops/git_demo/devops$ git status
On branch develop
Your branch is up to date with 'origin/develop'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
	modified:   testing.py

Untracked files:
  (use "git add <file>..." to include in what will be committed)
	key-gen
	key-gen.pub

no changes added to commit (use "git add" and/or "git commit -a")
ritik15@ritik15-Dell-15-DC15250:~/Documents/john savill devops/git_demo/devops$ git status
On branch develop
Your branch is up to date with 'origin/develop'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
	modified:   pack.py
	modified:   testing.py

Untracked files:
  (use "git add <file>..." to include in what will be committed)
	key-gen
	key-gen.pub

no changes added to commit (use "git add" and/or "git commit -a")
ritik15@ritik15-Dell-15-DC15250:~/Documents/john savill devops/git_demo/devops$ git add testing.py
ritik15@ritik15-Dell-15-DC15250:~/Documents/john savill devops/git_demo/devops$ git diff --cached
diff --git a/testing.py b/testing.py
index cdecb62..090e4ff 100644
--- a/testing.py
+++ b/testing.py
@@ -1,4 +1,4 @@
-print("a")
+print("hello")
 
 a=99
 b=101
ritik15@ritik15-Dell-15-DC15250:~/Documents/john savill devops/git_demo/devops$ git add pack.py
ritik15@ritik15-Dell-15-DC15250:~/Documents/john savill devops/git_demo/devops$ git diff --cached
diff --git a/pack.py b/pack.py
index ce47b77..e75154b 100644
--- a/pack.py
+++ b/pack.py
@@ -1 +1 @@
-print("hello")
\ No newline at end of file
+print("hello world")
\ No newline at end of file
diff --git a/testing.py b/testing.py
index cdecb62..090e4ff 100644
--- a/testing.py
+++ b/testing.py
@@ -1,4 +1,4 @@
-print("a")
+print("hello")
 
 a=99
 b=101
ritik15@ritik15-Dell-15-DC15250:~/Documents/john savill devops/git_demo/devops$ git diff HEAD
diff --git a/pack.py b/pack.py
index ce47b77..e75154b 100644
--- a/pack.py
+++ b/pack.py
@@ -1 +1 @@
-print("hello")
\ No newline at end of file
+print("hello world")
\ No newline at end of file
diff --git a/testing.py b/testing.py
index cdecb62..090e4ff 100644
--- a/testing.py
+++ b/testing.py
@@ -1,4 +1,4 @@
-print("a")
+print("hello")
 
 a=99
 b=101
ritik15@ritik15-Dell-15-DC15250:~/Documents/john savill devops/git_demo/devops$ git rm pack.py
error: the following file has changes staged in the index:
    pack.py
(use --cached to keep the file, or -f to force removal)
ritik15@ritik15-Dell-15-DC15250:~/Documents/john savill devops/git_demo/devops$ git restore --staged pack.py
ritik15@ritik15-Dell-15-DC15250:~/Documents/john savill devops/git_demo/devops$ git status
On branch develop
Your branch is up to date with 'origin/develop'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
	modified:   testing.py

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
	modified:   pack.py

Untracked files:
  (use "git add <file>..." to include in what will be committed)
	key-gen
	key-gen.pub

ritik15@ritik15-Dell-15-DC15250:~/Documents/john savill devops/git_demo/devops$ git restore pack.py
ritik15@ritik15-Dell-15-DC15250:~/Documents/john savill devops/git_demo/devops$ git status
On branch develop
Your branch is up to date with 'origin/develop'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
	modified:   testing.py

Untracked files:
  (use "git add <file>..." to include in what will be committed)
	key-gen
	key-gen.pub

ritik15@ritik15-Dell-15-DC15250:~/Documents/john savill devops/git_demo/devops$ git restore --staged testing.py
ritik15@ritik15-Dell-15-DC15250:~/Documents/john savill devops/git_demo/devops$ git status
On branch develop
Your branch is up to date with 'origin/develop'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
	modified:   testing.py

Untracked files:
  (use "git add <file>..." to include in what will be committed)
	key-gen
	key-gen.pub

no changes added to commit (use "git add" and/or "git commit -a")
ritik15@ritik15-Dell-15-DC15250:~/Documents/john savill devops/git_demo/devops$ git restore testing.py
ritik15@ritik15-Dell-15-DC15250:~/Documents/john savill devops/git_demo/devops$ git status
On branch develop
Your branch is up to date with 'origin/develop'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
	key-gen
	key-gen.pub

nothing added to commit but untracked files present (use "git add" to track)
ritik15@ritik15-Dell-15-DC15250:~/Documents/john savill devops/git_demo/devops$ git status
On branch develop
Your branch is up to date with 'origin/develop'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
	key-gen
	key-gen.pub

nothing added to commit but untracked files present (use "git add" to track)
ritik15@ritik15-Dell-15-DC15250:~/Documents/john savill devops/git_demo/devops$ git branch
* develop
  main
ritik15@ritik15-Dell-15-DC15250:~/Documents/john savill devops/git_demo/devops$ git branch
* develop
  main
ritik15@ritik15-Dell-15-DC15250:~/Documents/john savill devops/git_demo/devops$ git status
On branch develop
Your branch is up to date with 'origin/develop'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
	modified:   testing.py

Untracked files:
  (use "git add <file>..." to include in what will be committed)
	key-gen
	key-gen.pub

no changes added to commit (use "git add" and/or "git commit -a")
ritik15@ritik15-Dell-15-DC15250:~/Documents/john savill devops/git_demo/devops$ git add testing.py
ritik15@ritik15-Dell-15-DC15250:~/Documents/john savill devops/git_demo/devops$ git status
On branch develop
Your branch is up to date with 'origin/develop'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
	modified:   testing.py

Untracked files:
  (use "git add <file>..." to include in what will be committed)
	key-gen
	key-gen.pub

ritik15@ritik15-Dell-15-DC15250:~/Documents/john savill devops/git_demo/devops$ git reset
Unstaged changes after reset:
M	testing.py
ritik15@ritik15-Dell-15-DC15250:~/Documents/john savill devops/git_demo/devops$ git status
On branch develop
Your branch is up to date with 'origin/develop'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
	modified:   testing.py

Untracked files:
  (use "git add <file>..." to include in what will be committed)
	key-gen
	key-gen.pub

no changes added to commit (use "git add" and/or "git commit -a")
ritik15@ritik15-Dell-15-DC15250:~/Documents/john savill devops/git_demo/devops$ git restore testing.py
ritik15@ritik15-Dell-15-DC15250:~/Documents/john savill devops/git_demo/devops$ git log --online --graph
fatal: unrecognized argument: --online
ritik15@ritik15-Dell-15-DC15250:~/Documents/john savill devops/git_demo/devops$ git log --oneline --graph --alfatal: unrecognized argument: --al
ritik15@ritik15-Dell-15-DC15250:~/Documents/john savill devops/git_demo/devops$ git log --oneline --graph --all
* 08a7cfd (HEAD -> develop, origin/develop) Add message advocating for world peace
* 7436f94 file saved
* 3d26dee saved
* d894ae4 saved
* 79f7218 saved
* b72259b (origin/main, origin/HEAD, main) bkl.txt
* 6fe6a62 bkl.txt
* 19897d5 bkl.txt
* 1ea6b34 bkl.txt
* cfea188 Create testing.py
* 7b24945 Initial commit
ritik15@ritik15-Dell-15-DC15250:~/Documents/john savill devops/git_demo/devops$ git branch
* develop
  main
ritik15@ritik15-Dell-15-DC15250:~/Documents/john savill devops/git_demo/devops$ git branch main
fatal: a branch named 'main' already exists
ritik15@ritik15-Dell-15-DC15250:~/Documents/john savill devops/git_demo/devops$ git branch -b main
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
    -v, --[no-]verbose    show hash and subject, give twice for upstream branch
    -q, --[no-]quiet      suppress informational messages
    -t, --[no-]track[=(direct|inherit)]
                          set branch tracking configuration
    -u, --[no-]set-upstream-to <upstream>
                          change the upstream info
    --[no-]unset-upstream unset the upstream info
    --[no-]color[=<when>] use colored output
    -r, --remotes         act on remote-tracking branches
    --contains <commit>   print only branches that contain the commit
    --no-contains <commit>
                          print only branches that don't contain the commit
    --[no-]abbrev[=<n>]   use <n> digits to display object names

Specific git-branch actions:
    -a, --all             list both remote-tracking and local branches
    -d, --[no-]delete     delete fully merged branch
    -D                    delete branch (even if not merged)
    -m, --[no-]move       move/rename a branch and its reflog
    -M                    move/rename a branch, even if target exists
    --[no-]omit-empty     do not output a newline after empty formatted refs
    -c, --[no-]copy       copy a branch and its reflog
    -C                    copy a branch, even if target exists
    -l, --[no-]list       list branch names
    --[no-]show-current   show current branch name
    --[no-]create-reflog  create the branch's reflog
    --[no-]edit-description
                          edit the description for the branch
    -f, --[no-]force      force creation, move/rename, deletion
    --merged <commit>     print only branches that are merged
    --no-merged <commit>  print only branches that are not merged
    --[no-]column[=<style>]
                          list branches in columns
    --[no-]sort <key>     field name to sort on
    --[no-]points-at <object>
                          print only branches of the object
    -i, --[no-]ignore-case
                          sorting and filtering are case insensitive
    --[no-]recurse-submodules
                          recurse through submodules
    --[no-]format <format>
                          format to use for the output

ritik15@ritik15-Dell-15-DC15250:~/Documents/john savill devops/git_demo/devops$ git branch -m main
fatal: a branch named 'main' already exists
ritik15@ritik15-Dell-15-DC15250:~/Documents/john savill devops/git_demo/devops$ git branch
* develop
  main
ritik15@ritik15-Dell-15-DC15250:~/Documents/john savill devops/git_demo/devops$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
ritik15@ritik15-Dell-15-DC15250:~/Documents/john savill devops/git_demo/devops$ git log --oneline --graph --all
* 08a7cfd (origin/develop, develop) Add message advocating for world peace
* 7436f94 file saved
* 3d26dee saved
* d894ae4 saved
* 79f7218 saved
* b72259b (HEAD -> main, origin/main, origin/HEAD) bkl.txt
* 6fe6a62 bkl.txt
* 19897d5 bkl.txt
* 1ea6b34 bkl.txt
* cfea188 Create testing.py
* 7b24945 Initial commit
ritik15@ritik15-Dell-15-DC15250:~/Documents/john savill devops/git_demo/devops$ git reset HEAD~1 --soft
ritik15@ritik15-Dell-15-DC15250:~/Documents/john savill devops/git_demo/devops$ git log --oneline --graph --all
* 08a7cfd (origin/develop, develop) Add message advocating for world peace
* 7436f94 file saved
* 3d26dee saved
* d894ae4 saved
* 79f7218 saved
* b72259b (origin/main, origin/HEAD) bkl.txt
* 6fe6a62 (HEAD -> main) bkl.txt
* 19897d5 bkl.txt
* 1ea6b34 bkl.txt
* cfea188 Create testing.py
* 7b24945 Initial commit
ritik15@ritik15-Dell-15-DC15250:~/Documents/john savill devops/git_demo/devops$ git diff b72259b..6fe6a62
diff --git a/bkl.txt b/bkl.txt
index 3cdf9c2..403788f 100644
--- a/bkl.txt
+++ b/bkl.txt
@@ -1,3 +1,2 @@
 Ramayana 
-Mahabharata
-are the Greatest mythology epic of india
\ No newline at end of file
+Mahabharata
\ No newline at end of file
ritik15@ritik15-Dell-15-DC15250:~/Documents/john savill devops/git_demo/devops$ git diff 6fe6a62..19897d5
diff --git a/bkl.txt b/bkl.txt
index 403788f..ebffe61 100644
--- a/bkl.txt
+++ b/bkl.txt
@@ -1,2 +1,3 @@
-Ramayana 
-Mahabharata
\ No newline at end of file
+hello bkl gand marao
+thank you
+chal be
\ No newline at end of file
ritik15@ritik15-Dell-15-DC15250:~/Documents/john savill devops/git_demo/devops$ git diff 19897d5..1ea6b34
diff --git a/bkl.txt b/bkl.txt
index ebffe61..93f0588 100644
--- a/bkl.txt
+++ b/bkl.txt
@@ -1,3 +1,2 @@
 hello bkl gand marao
-thank you
-chal be
\ No newline at end of file
+thank you
\ No newline at end of file
ritik15@ritik15-Dell-15-DC15250:~/Documents/john savill devops/git_demo/devops$ git reset HEAD~2 --soft
ritik15@ritik15-Dell-15-DC15250:~/Documents/john savill devops/git_demo/devops$ git reset HEAD~1 --soft
ritik15@ritik15-Dell-15-DC15250:~/Documents/john savill devops/git_demo/devops$ git branch
  develop
* main
ritik15@ritik15-Dell-15-DC15250:~/Documents/john savill devops/git_demo/devops$ git checkout develop
error: Your local changes to the following files would be overwritten by checkout:
	bkl.txt
Please commit your changes or stash them before you switch branches.
Aborting
ritik15@ritik15-Dell-15-DC15250:~/Documents/john savill devops/git_demo/devops$ git commit -m "backtooriginal"
[main 17ee03a] backtooriginal
 1 file changed, 3 insertions(+)
 create mode 100644 bkl.txt
ritik15@ritik15-Dell-15-DC15250:~/Documents/john savill devops/git_demo/devops$ git checkout develop
Switched to branch 'develop'
Your branch is up to date with 'origin/develop'.
ritik15@ritik15-Dell-15-DC15250:~/Documents/john savill devops/git_demo/devops$ git checkout main
Switched to branch 'main'
Your branch and 'origin/main' have diverged,
and have 1 and 4 different commits each, respectively.
  (use "git pull" if you want to integrate the remote branch with yours)
ritik15@ritik15-Dell-15-DC15250:~/Documents/john savill devops/git_demo/devops$ git checkout develop
Switched to branch 'develop'
Your branch is up to date with 'origin/develop'.
ritik15@ritik15-Dell-15-DC15250:~/Documents/john savill devops/git_demo/devops$ git reset HEAD~1 --soft
ritik15@ritik15-Dell-15-DC15250:~/Documents/john savill devops/git_demo/devops$ git commit -m "back"
[develop b16921b] back
 1 file changed, 1 insertion(+)
 create mode 100644 War
ritik15@ritik15-Dell-15-DC15250:~/Documents/john savill devops/git_demo/devops$ git branch
* develop
  main
ritik15@ritik15-Dell-15-DC15250:~/Documents/john savill devops/git_demo/devops$ git checkout main
Switched to branch 'main'
Your branch and 'origin/main' have diverged,
and have 1 and 4 different commits each, respectively.
  (use "git pull" if you want to integrate the remote branch with yours)
ritik15@ritik15-Dell-15-DC15250:~/Documents/john savill devops/git_demo/devops$ 

