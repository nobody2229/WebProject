**در این پروژه ابتدا در لوکال سیستم پوشه ای به نام WebProject ساختم سپس به عنوان پوشه ریشه قرار دادم و سه فایل index.html,style.css,script.js
رو در ان پوشه ایجاد کردم و شاخه ای به نام feature/update-title که با استفاده از ان عنوان را تغییر داردم و پوشه main رو اپدیت کردم و بعد شاخه را پاک 
کردم. دستورات conflict,revertmerge همگی در لوکال اجرا و سپس همه را به گیت هاب پوش کردم
در گیت هاب پروژه Web project tasks را تعریف و ایسو به نام افزودن فوتر ایجاد کردم شاخه جدیدی به نام feature/add-footer ساختم و 
سپس پروژه را در نرم افزار گیت دسکتاپ بروز رسانی کردم فایل ایندکس در شاخه فوتر را بروزرسانی و فوتر را اضافه سپس به گیت هاب پوش و در گیت هاب دستور پول و مرج
بابت کلون هم امکان اوردن پروژه از گیت هاب به گیت هاب دسکتاب وجود دارد برای راحتی کار و پوش و پول کردن ان
**جزییات پروژه در لوکال به شرح ذیل می باشد**




C:\Users\CD CITY\WebProject>git init
Initialized empty Git repository in C:/Users/CD CITY/WebProject/.git/

C:\Users\CD CITY\WebProject>git status
On branch main

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        index.html
        script.js
        style.css

nothing added to commit but untracked files present (use "git add" to track)

C:\Users\CD CITY\WebProject>git add index.html script.js style.css

C:\Users\CD CITY\WebProject>git commit -m "avalin commit ba filhaye CSS,HTML,JS"
[main (root-commit) 3994a2d] avalin commit ba filhaye CSS,HTML,JS
 3 files changed, 22 insertions(+)
 create mode 100644 index.html
 create mode 100644 script.js
 create mode 100644 style.css

C:\Users\CD CITY\WebProject>git branch
* main

C:\Users\CD CITY\WebProject>git branch feature/update-title

C:\Users\CD CITY\WebProject>git checkout feature/update-title
Switched to branch 'feature/update-title'

C:\Users\CD CITY\WebProject>git branch
* feature/update-title
  main

C:\Users\CD CITY\WebProject>git status
On branch feature/update-title
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   index.html

no changes added to commit (use "git add" and/or "git commit -a")

C:\Users\CD CITY\WebProject>git add index.html

C:\Users\CD CITY\WebProject>git commit -m "onvan dar inde.html berozresani shod"
[feature/update-title 249c0b7] onvan dar inde.html berozresani shod
 1 file changed, 1 insertion(+), 1 deletion(-)

C:\Users\CD CITY\WebProject>git log
commit 249c0b7c681c5caf29d0857efeaf9d4a64c2a30f (HEAD -> feature/update-title)
Author: nobody2229 <141580690+nobody2229@users.noreply.github.com>
Date:   Mon Jan 13 23:28:58 2025 +0330

    onvan dar inde.html berozresani shod

commit 3994a2d0e6afcf8bced226aa882285569ce00018 (main)
Author: nobody2229 <141580690+nobody2229@users.noreply.github.com>
Date:   Mon Jan 13 23:25:48 2025 +0330

    avalin commit ba filhaye CSS,HTML,JS

C:\Users\CD CITY\WebProject>git show  249c0b7c681c5caf29d0857efeaf9d4a64c2a30f
commit 249c0b7c681c5caf29d0857efeaf9d4a64c2a30f (HEAD -> feature/update-title)
Author: nobody2229 <141580690+nobody2229@users.noreply.github.com>
Date:   Mon Jan 13 23:28:58 2025 +0330

    onvan dar inde.html berozresani shod

diff --git a/index.html b/index.html
index abe4580..980c509 100644
--- a/index.html
+++ b/index.html
@@ -2,7 +2,7 @@
 <html>
     <head>
         <title>
-           پروژه وب  من
+           پروژه وب بروزرسانی شده  من
         </title>
         <link rel="stylesheet" href="style.css">


C:\Users\CD CITY\WebProject>git checkout main
Switched to branch 'main'

C:\Users\CD CITY\WebProject>git log
commit 3994a2d0e6afcf8bced226aa882285569ce00018 (HEAD -> main)
Author: nobody2229 <141580690+nobody2229@users.noreply.github.com>
Date:   Mon Jan 13 23:25:48 2025 +0330

    avalin commit ba filhaye CSS,HTML,JS

C:\Users\CD CITY\WebProject>git merge feature/update-title
Updating 3994a2d..249c0b7
Fast-forward
 index.html | 2 +-
 1 file changed, 1 insertion(+), 1 deletion(-)

C:\Users\CD CITY\WebProject>git branch -d feature/update-title
Deleted branch feature/update-title (was 249c0b7).

C:\Users\CD CITY\WebProject>git status
On branch main
nothing to commit, working tree clean

C:\Users\CD CITY\WebProject>git log
commit 249c0b7c681c5caf29d0857efeaf9d4a64c2a30f (HEAD -> main)
Author: nobody2229 <141580690+nobody2229@users.noreply.github.com>
Date:   Mon Jan 13 23:28:58 2025 +0330

    onvan dar inde.html berozresani shod

commit 3994a2d0e6afcf8bced226aa882285569ce00018
Author: nobody2229 <141580690+nobody2229@users.noreply.github.com>
Date:   Mon Jan 13 23:25:48 2025 +0330

    avalin commit ba filhaye CSS,HTML,JS

C:\Users\CD CITY\WebProject>git show  249c0b7c681c5caf29d0857efeaf9d4a64c2a30f
commit 249c0b7c681c5caf29d0857efeaf9d4a64c2a30f (HEAD -> main)
Author: nobody2229 <141580690+nobody2229@users.noreply.github.com>
Date:   Mon Jan 13 23:28:58 2025 +0330

    onvan dar inde.html berozresani shod

diff --git a/index.html b/index.html
index abe4580..980c509 100644
--- a/index.html
+++ b/index.html
@@ -2,7 +2,7 @@
 <html>
     <head>
         <title>
-           پروژه وب  من
+           پروژه وب بروزرسانی شده  من
         </title>
         <link rel="stylesheet" href="style.css">


C:\Users\CD CITY\WebProject>git branch feature/conflict-example

C:\Users\CD CITY\WebProject>git checkout feature/conflict-example
Switched to branch 'feature/conflict-example'

C:\Users\CD CITY\WebProject>git branch
* feature/conflict-example
  main

C:\Users\CD CITY\WebProject>git status
On branch feature/conflict-example
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   index.html

no changes added to commit (use "git add" and/or "git commit -a")

C:\Users\CD CITY\WebProject>git add index.html

C:\Users\CD CITY\WebProject>gti commit -m"changes in feature branch"
'gti' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\CD CITY\WebProject>git commit -m"changes in feature branch"
[feature/conflict-example 83eddb3] changes in feature branch
 1 file changed, 1 insertion(+), 1 deletion(-)


C:\Users\CD CITY\WebProject>git checkout main
Switched to branch 'main'

operable program or batch file.

C:\Users\CD CITY\WebProject>git status
On branch main
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   index.html

no changes added to commit (use "git add" and/or "git commit -a")

C:\Users\CD CITY\WebProject>git add index.html

C:\Users\CD CITY\WebProject>git commit -m "changes in main branch"
[main ddc0163] changes in main branch
 1 file changed, 1 insertion(+), 1 deletion(-)

C:\Users\CD CITY\WebProject>git merge feature/conflict-example
Auto-merging index.html
CONFLICT (content): Merge conflict in index.html
Automatic merge failed; fix conflicts and then commit the result.

C:\Users\CD CITY\WebProject>git log
commit ddc0163e10375b1833bf60a0d197f597075e7a6b (HEAD -> main)
Author: nobody2229 <141580690+nobody2229@users.noreply.github.com>
Date:   Mon Jan 13 23:50:51 2025 +0330

    changes in main branch

commit 249c0b7c681c5caf29d0857efeaf9d4a64c2a30f
Author: nobody2229 <141580690+nobody2229@users.noreply.github.com>
Date:   Mon Jan 13 23:28:58 2025 +0330

    onvan dar inde.html berozresani shod

commit 3994a2d0e6afcf8bced226aa882285569ce00018
Author: nobody2229 <141580690+nobody2229@users.noreply.github.com>
Date:   Mon Jan 13 23:25:48 2025 +0330

    avalin commit ba filhaye CSS,HTML,JS

C:\Users\CD CITY\WebProject>git status
On branch main
You have unmerged paths.
  (fix conflicts and run "git commit")
  (use "git merge --abort" to abort the merge)

Unmerged paths:
  (use "git add <file>..." to mark resolution)
        both modified:   index.html

no changes added to commit (use "git add" and/or "git commit -a")



C:\Users\CD CITY\WebProject>git add index.html

C:\Users\CD CITY\WebProject>git commit -m "taghiir nahayee pas az conflict"
[main ebd500b] taghiir nahayee pas az conflict

C:\Users\CD CITY\WebProject>git log
commit ebd500b3ad8a4d83b4e894eb91e74aea8ccfa8fd (HEAD -> main)
Merge: ddc0163 83eddb3
Author: nobody2229 <141580690+nobody2229@users.noreply.github.com>
Date:   Mon Jan 13 23:54:20 2025 +0330

    taghiir nahayee pas az conflict

commit ddc0163e10375b1833bf60a0d197f597075e7a6b
Author: nobody2229 <141580690+nobody2229@users.noreply.github.com>
Date:   Mon Jan 13 23:50:51 2025 +0330

    changes in main branch

commit 83eddb32649607080c87b9e4d6d4333e642075e9 (feature/conflict-example)
Author: nobody2229 <141580690+nobody2229@users.noreply.github.com>
Date:   Mon Jan 13 23:48:35 2025 +0330

    changes in feature branch

commit 249c0b7c681c5caf29d0857efeaf9d4a64c2a30f
Author: nobody2229 <141580690+nobody2229@users.noreply.github.com>
Date:   Mon Jan 13 23:28:58 2025 +0330

    onvan dar inde.html berozresani shod

commit 3994a2d0e6afcf8bced226aa882285569ce00018
Author: nobody2229 <141580690+nobody2229@users.noreply.github.com>
Date:   Mon Jan 13 23:25:48 2025 +0330


C:\Users\CD CITY\WebProject>git status
On branch main
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   script.js

no changes added to commit (use "git add" and/or "git commit -a")

C:\Users\CD CITY\WebProject>git add script.js

C:\Users\CD CITY\WebProject>git commit -m"afzodan payam eshtebah be script.js"
[main 0e1a899] afzodan payam eshtebah be script.js
 1 file changed, 1 insertion(+)

C:\Users\CD CITY\WebProject>git log
commit 0e1a899bf0223c36c7b3ee69de978542fffd2b88 (HEAD -> main)
Author: nobody2229 <141580690+nobody2229@users.noreply.github.com>
Date:   Mon Jan 13 23:59:45 2025 +0330

    afzodan payam eshtebah be script.js

commit ebd500b3ad8a4d83b4e894eb91e74aea8ccfa8fd
Merge: ddc0163 83eddb3
Author: nobody2229 <141580690+nobody2229@users.noreply.github.com>
Date:   Mon Jan 13 23:54:20 2025 +0330

    taghiir nahayee pas az conflict

commit ddc0163e10375b1833bf60a0d197f597075e7a6b
Author: nobody2229 <141580690+nobody2229@users.noreply.github.com>
Date:   Mon Jan 13 23:50:51 2025 +0330

    changes in main branch

commit 83eddb32649607080c87b9e4d6d4333e642075e9 (feature/conflict-example)
Author: nobody2229 <141580690+nobody2229@users.noreply.github.com>
Date:   Mon Jan 13 23:48:35 2025 +0330

    changes in feature branch

commit 249c0b7c681c5caf29d0857efeaf9d4a64c2a30f
Author: nobody2229 <141580690+nobody2229@users.noreply.github.com>
Date:   Mon Jan 13 23:28:58 2025 +0330



C:\Users\CD CITY\WebProject>git show 0e1a899bf0223c36c7b3ee69de978542fffd2b88
commit 0e1a899bf0223c36c7b3ee69de978542fffd2b88 (HEAD -> main)
Author: nobody2229 <141580690+nobody2229@users.noreply.github.com>
Date:   Mon Jan 13 23:59:45 2025 +0330

    afzodan payam eshtebah be script.js

diff --git a/script.js b/script.js
index 3cf9980..6dc5935 100644
--- a/script.js
+++ b/script.js
@@ -1 +1,2 @@
 console.log('!به پروژه من خوش آمدید');
+alert('!ین یک هشدار اشتباه است');
\ No newline at end of file

C:\Users\CD CITY\WebProject>git revert 0e1a899bf0223c36c7b3ee69de978542fffd2b88
[main f542799] Revert "afzodan payam eshtebah be script.js"
 1 file changed, 1 deletion(-)

C:\Users\CD CITY\WebProject>git log
commit f5427995a3bb0558a98dfedc43cc357488848f38 (HEAD -> main)
Author: nobody2229 <141580690+nobody2229@users.noreply.github.com>
Date:   Tue Jan 14 00:01:33 2025 +0330

    Revert "afzodan payam eshtebah be script.js"

    This reverts commit 0e1a899bf0223c36c7b3ee69de978542fffd2b88.

commit 0e1a899bf0223c36c7b3ee69de978542fffd2b88
Author: nobody2229 <141580690+nobody2229@users.noreply.github.com>
Date:   Mon Jan 13 23:59:45 2025 +0330

    afzodan payam eshtebah be script.js

commit ebd500b3ad8a4d83b4e894eb91e74aea8ccfa8fd
Merge: ddc0163 83eddb3
Author: nobody2229 <141580690+nobody2229@users.noreply.github.com>
Date:   Mon Jan 13 23:54:20 2025 +0330

    taghiir nahayee pas az conflict

commit ddc0163e10375b1833bf60a0d197f597075e7a6b
Author: nobody2229 <141580690+nobody2229@users.noreply.github.com>
Date:   Mon Jan 13 23:50:51 2025 +0330

    changes in main branch

commit 83eddb32649607080c87b9e4d6d4333e642075e9 (feature/conflict-example)
Author: nobody2229 <141580690+nobody2229@users.noreply.github.com>

C:\Users\CD CITY\WebProject>git show f5427995a3bb0558a98dfedc43cc357488848f38
commit f5427995a3bb0558a98dfedc43cc357488848f38 (HEAD -> main)
Author: nobody2229 <141580690+nobody2229@users.noreply.github.com>
Date:   Tue Jan 14 00:01:33 2025 +0330

    Revert "afzodan payam eshtebah be script.js"

    This reverts commit 0e1a899bf0223c36c7b3ee69de978542fffd2b88.

diff --git a/script.js b/script.js
index 6dc5935..3cf9980 100644
--- a/script.js
+++ b/script.js
@@ -1,2 +1 @@
 console.log('!به پروژه من خوش آمدید');
-alert('!ین یک هشدار اشتباه است');
\ No newline at end of file

C:\Users\CD CITY\WebProject>git remote add WebProject https://github.com/nobody2229/WebProject.git

C:\Users\CD CITY\WebProject>git push -u WebProject main
C:\Users\CD CITY\WebProject>git clone https://github.com/nobody2229/WebProject.git
Cloning into 'WebProject'...
remote: Enumerating objects: 44, done.
remote: Counting objects: 100% (44/44), done.
remote: Compressing objects: 100% (35/35), done.
remote: Total 44 (delta 14), reused 29 (delta 9), pack-reused 0 (from 0)
Receiving objects: 100% (44/44), 11.36 KiB | 90.00 KiB/s, done.
Resolving deltas: 100% (14/14), done.
