# Gym-Git-Exercise-Solutions
# Bundle 1
```bash
HP@ian MINGW32 ~ (main)
$ mkdir bundle1

HP@ian MINGW32 ~ (main)
$ cd bundle1

HP@ian MINGW32 ~/bundle1 (main)
$ git init
Initialized empty Git repository in C:/Users/HP/bundle1/.git/

HP@ian MINGW32 ~/bundle1 (master)
$ vim bundle1.py

HP@ian MINGW32 ~/bundle1 (master)
$ ls
bundle1.py

HP@ian MINGW32 ~/bundle1 (master)
$ git branch -m main

HP@ian MINGW32 ~/bundle1 (main)
$ git branch

HP@ian MINGW32 ~/bundle1 (main)
$ git add --all
warning: in the working copy of 'bundle1.py', LF will be replaced by CRLF the next time Git touches it

HP@ian MINGW32 ~/bundle1 (main)
$ git commit -m "Created the first bundle1 commit"
[main (root-commit) af85a83] Created the first bundle1 commit
 1 file changed, 5 insertions(+)
 create mode 100644 bundle1.py

HP@ian MINGW32 ~/bundle1 (main)
$ ssh-keygen -t rsa -b 4096 -C "i.ganza@alustudent.com"
Generating public/private rsa key pair.
Enter file in which to save the key (/c/Users/HP/.ssh/id_rsa):
/c/Users/HP/.ssh/id_rsa already exists.
Overwrite (y/n)? y
Enter passphrase (empty for no passphrase):
Enter same passphrase again:
Your identification has been saved in /c/Users/HP/.ssh/id_rsa
Your public key has been saved in /c/Users/HP/.ssh/id_rsa.pub
The key fingerprint is:
SHA256:mqBzzmhJFWrD/rhUAC6Nyn0fG7VecBX1Aox90DguOlk i.ganza@alustudent.com
The key's randomart image is:
+---[RSA 4096]----+
|.          +o*o. |
|.+  .     . *.o .|
|ooo. .   o o o. .|
|+ *..   . E .  . |
|.+ +o. oS= o     |
|  oo...oO .      |
| .++. oo o       |
| .+*.            |
| .o.o            |
+----[SHA256]-----+

HP@ian MINGW32 ~/bundle1 (main)
$ cat ~/.ssh/id_rsa.pub
ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAACAQDblVY6HTjPe5nP1yFiq8mN07Zw554TS3u9k80w+15zY1+v2t4slPgzX8y8LYva8r281zo4lMeEBUDxShMMc1pjMon4Za9CbxSbt0bqf7ukcLGc/gmKuDrme9cYHSGm0MnAi3E+dCg4HnrIBDZdo98h6T958SzAA5TSTZNhBdkiVFkmaB9sf6nZ8uZd4Vmufn6Iy/UrnhvEzJ0kcUjTmSCoDwSJYWmkjJATCnkT/YLJbFrzniNVb0SbVGlAZT9cXnzpvvFYP9qe2UxYt5k2xDY+7Z8yCvG7Ji4I8y8IaThGNchpuq31M4sZq09Iv2UHV3v+Xoxs6NsSe0fQI4iknlsAqOLUQv75Bs7/okX/QjrmAQYjNEO2wvwA8efHkfDcoHhisIDrfwruj6eBCc82/QQ3mhIRCgCY0JteJ+Puaoauku0oyNIDLEy6PU7KUlMN4mq7vgpbmUhGUMUtkndpLiTqtSpJp3YVptkmVWZ3fwPD0V3VahtLujIDOnNm5BhMHTqApdw0BH2LduHL6f9pKYnDxl2HQ8htf2drFPWxFWyU99TPp/x62sJszxAkO3VMdGb1WrMR7WZbiYSYmkk4rAbEFTlakxXLSALdtDhIAL2TC7A3NyHkWEN1MlcK/RpjCywMAWP71VgvFktSwRQ30eUpicZQ4jawGu6DdsqRxYa7mQ== i.ganza@alustudent.com

HP@ian MINGW32 ~/bundle1 (main)
$ git clone git@github.com:i-ganza007/Bundle-1-.git
Cloning into 'Bundle-1-'...
The authenticity of host 'github.com (20.87.245.0)' can't be established.
ED25519 key fingerprint is SHA256:+DiY3wvvV6TuJJhbpZisF/zLDA0zPMSvHdkr4UvCOqU.
This key is not known by any other names.
Are you sure you want to continue connecting (yes/no/[fingerprint])? yes
Warning: Permanently added 'github.com' (ED25519) to the list of known hosts.
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Compressing objects: 100% (2/2), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Receiving objects: 100% (3/3), done.

HP@ian MINGW32 ~/bundle1 (main)
$ git remote add origin git@github.com:i-ganza007/Bundle-1-.git

HP@ian MINGW32 ~/bundle1 (main)
$ git remote -v
origin  git@github.com:i-ganza007/Bundle-1-.git (fetch)
origin  git@github.com:i-ganza007/Bundle-1-.git (push)

HP@ian MINGW32 ~/bundle1 (main)
$ git status
On branch main
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        Bundle-1-/

nothing added to commit but untracked files present (use "git add" to track)

HP@ian MINGW32 ~/bundle1 (main)
$ git add bundle1.py

HP@ian MINGW32 ~/bundle1 (main)
$ git commit -m "Adding Bundle 1 first commit"
On branch main
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        Bundle-1-/

nothing added to commit but untracked files present (use "git add" to track)

HP@ian MINGW32 ~/bundle1 (main)
$ git add -all
error: did you mean `--all` (with two dashes)?

HP@ian MINGW32 ~/bundle1 (main)
$ git add --all
warning: adding embedded git repository: Bundle-1-
hint: You've added another git repository inside your current repository.
hint: Clones of the outer repository will not contain the contents of
hint: the embedded repository and will not know how to obtain it.
hint: If you meant to add a submodule, use:
hint:
hint:   git submodule add <url> Bundle-1-
hint:
hint: If you added this path by mistake, you can remove it from the
hint: index with:
hint:
hint:   git rm --cached Bundle-1-
hint:
hint: See "git help submodule" for more information.

HP@ian MINGW32 ~/bundle1 (main)
$ git push -u origin main
To github.com:i-ganza007/Bundle-1-.git
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'github.com:i-ganza007/Bundle-1-.git'
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

HP@ian MINGW32 ~/bundle1 (main)
$ ^C

HP@ian MINGW32 ~/bundle1 (main)
$ git pull origin main
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Compressing objects: 100% (2/2), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (3/3), 1.45 KiB | 92.00 KiB/s, done.
From github.com:i-ganza007/Bundle-1-
 * branch            main       -> FETCH_HEAD
 * [new branch]      main       -> origin/main
fatal: refusing to merge unrelated histories

HP@ian MINGW32 ~/bundle1 (main)
$ git add --all

HP@ian MINGW32 ~/bundle1 (main)
$ git commit -m "Adding Bundle 1 first commit"
[main 7933eab] Adding Bundle 1 first commit
 1 file changed, 1 insertion(+)
 create mode 160000 Bundle-1-

HP@ian MINGW32 ~/bundle1 (main)
$ git push -u origin main
To github.com:i-ganza007/Bundle-1-.git
 ! [rejected]        main -> main (non-fast-forward)
error: failed to push some refs to 'github.com:i-ganza007/Bundle-1-.git'
hint: Updates were rejected because the tip of your current branch is behind
hint: its remote counterpart. Integrate the remote changes (e.g.
hint: 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

HP@ian MINGW32 ~/bundle1 (main)
$ git push origin main
To github.com:i-ganza007/Bundle-1-.git
 ! [rejected]        main -> main (non-fast-forward)
error: failed to push some refs to 'github.com:i-ganza007/Bundle-1-.git'
hint: Updates were rejected because the tip of your current branch is behind
hint: its remote counterpart. Integrate the remote changes (e.g.
hint: 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

HP@ian MINGW32 ~/bundle1 (main)
$ git pull origin main
From github.com:i-ganza007/Bundle-1-
 * branch            main       -> FETCH_HEAD
fatal: refusing to merge unrelated histories

HP@ian MINGW32 ~/bundle1 (main)
$ ^C

HP@ian MINGW32 ~/bundle1 (main)
$ git push origin main --force
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (5/5), 532 bytes | 133.00 KiB/s, done.
Total 5 (delta 0), reused 0 (delta 0), pack-reused 0
To github.com:i-ganza007/Bundle-1-.git
 + ca0f030...7933eab main -> main (forced update)

HP@ian MINGW32 ~/bundle1 (main)
$ git add Bundle1.py

HP@ian MINGW32 ~/bundle1 (main)
$ ls
Bundle-1-/  bundle1.py

HP@ian MINGW32 ~/bundle1 (main)
$ git add bundle1.py

HP@ian MINGW32 ~/bundle1 (main)
$ git commit -m "Adding Bundle 1 first commit"
On branch main
nothing to commit, working tree clean

HP@ian MINGW32 ~/bundle1 (main)
$ git push origin main --force
Everything up-to-date

HP@ian MINGW32 ~/bundle1 (main)
$ cd ..

HP@ian MINGW32 ~ (main)
$ ls
 -1.14-windows.xml
 0x00-shell_basics/
 AndroidStudioProjects/
 AppData/
'Application Data'@
 BST
 Contacts/
 Cookies@
 Desktop/
 Documents/
 Downloads/
 Events
 Favorites/
 IntelGraphicsProfiles/
 LingvanexTranslator/
 Links/
'Local Settings'@
 MagiskOnWSALocal/
 Music/
'My Documents'@
 NTUSER.DAT
 NTUSER.DAT{a2332f18-cdbf-11ec-8680-002248483d79}.TM.blf
 NTUSER.DAT{a2332f18-cdbf-11ec-8680-002248483d79}.TMContainer00000000000000000001.regtrans-ms
 NTUSER.DAT{a2332f18-cdbf-11ec-8680-002248483d79}.TMContainer00000000000000000002.regtrans-ms
 NetHood@
 OneDrive/
 Pictures/
 PixelSee/
'Postman Agent'/
 PrintHood@
 PycharmProjects/
 Recent@
'Saved Games'/
 Searches/
 SendTo@
'Start Menu'@
 Templates@
 TopG/
 Untitled-1.html
 Untitled-2.js
 Videos/
 _netrc
 alu-AirBnB_clone.git/
 alx-pre_course/
 base_model.py
 bash.sh*
 bts/
 bundle1/
 django_project/
 doit.txt*
 eclipse/
 edb_languagepack_4.exe*
 edb_npgsql.exe*
 edb_pgagent_pg16.exe*
 edb_pgbouncer.exe*
 edb_pgjdbc.exe*
 edb_psqlodbc.exe*
 edb_psqlodbc.exe-20231220153201*
 friends/
 get-pip.py*
 github/
 himom.sh*
'kwita izina project.html'
 mentalpal/
 ntuser.dat.LOG1
 ntuser.dat.LOG2
 ntuser.ini
 op
 pemhttpd.exe*
 pemhttpd.exe-20231220153233*
 vue-start-spa/
 vueApp/
 w3gitpractice/

HP@ian MINGW32 ~ (main)
$ cd Bundle1

HP@ian MINGW32 ~/Bundle1 (main)
$ ls
Bundle-1-/  bundle1.py

HP@ian MINGW32 ~/Bundle1 (main)
$ ls Bundle-1-
LICENSE

HP@ian MINGW32 ~/Bundle1 (main)
$ git add bundle1.py

HP@ian MINGW32 ~/Bundle1 (main)
$ cat bundle1.py
array = [1,2,3,4,5]
def ArrReturn(arr){
    return arr
        }


HP@ian MINGW32 ~/Bundle1 (main)
$ git commit -m "Adding bundle1.py"
On branch main
nothing to commit, working tree clean

HP@ian MINGW32 ~/Bundle1 (main)
$ git checkout -b dev
Switched to a new branch 'dev'

HP@ian MINGW32 ~/Bundle1 (dev)
$ git checkout -b test
Switched to a new branch 'test'

HP@ian MINGW32 ~/Bundle1 (test)
$ git checkout dev
Switched to branch 'dev'

HP@ian MINGW32 ~/Bundle1 (dev)
$ git branch -d test
Deleted branch test (was 7933eab).
```
# Bundle 1 Exercise 2
```bash
HP@ian MINGW32 ~/Bundle1 (main)
$ git checkout dev
Switched to branch 'dev'

HP@ian MINGW32 ~/Bundle1 (dev)
$ ls
Bundle-1-/  bundle1.py

HP@ian MINGW32 ~/Bundle1 (dev)
$ touch home.html

HP@ian MINGW32 ~/Bundle1 (dev)
$ ls
Bundle-1-/  bundle1.py  home.html

HP@ian MINGW32 ~/Bundle1 (dev)
$ vim home.html

HP@ian MINGW32 ~/Bundle1 (dev)
$ git status
On branch dev
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        home.html

nothing added to commit but untracked files present (use "git add" to track)

HP@ian MINGW32 ~/Bundle1 (dev)
$ git status --short
?? home.html

HP@ian MINGW32 ~/Bundle1 (dev)
$ vim home.html

HP@ian MINGW32 ~/Bundle1 (dev)
$ git status --short
?? home.html

HP@ian MINGW32 ~/Bundle1 (dev)
$ git status
#On branch dev
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        home.html

nothing added to commit but untracked files present (use "git add" to track)

HP@ian MINGW32 ~/Bundle1 (dev)
$ git add --all
warning: in the working copy of 'home.html', LF will be replaced by CRLF the next time Git touches it

HP@ian MINGW32 ~/Bundle1 (dev)
$ git status
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   home.html


HP@ian MINGW32 ~/Bundle1 (dev)
$ vim home.html

HP@ian MINGW32 ~/Bundle1 (dev)
$ git status
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   home.html

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   home.html


HP@ian MINGW32 ~/Bundle1 (dev)
$ git stash save "Stashing the changes of the home html"
warning: in the working copy of 'home.html', LF will be replaced by CRLF the next time Git touches it
Saved working directory and index state On dev: Stashing the changes of the home html

HP@ian MINGW32 ~/Bundle1 (dev)
$ vim about.html

HP@ian MINGW32 ~/Bundle1 (dev)
$ git add --a;;
bash: syntax error near unexpected token `;;'

HP@ian MINGW32 ~/Bundle1 (dev)
$ git add --all
warning: in the working copy of 'about.html', LF will be replaced by CRLF the next time Git touches it

HP@ian MINGW32 ~/Bundle1 (dev)
$ git status
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html


HP@ian MINGW32 ~/Bundle1 (dev)
$ vim about.html

HP@ian MINGW32 ~/Bundle1 (dev)
$ git status
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   about.html


HP@ian MINGW32 ~/Bundle1 (dev)
$ git diff
warning: in the working copy of 'about.html', LF will be replaced by CRLF the next time Git touches it
diff --git a/about.html b/about.html
index 2943159..0a0c849 100644
--- a/about.html
+++ b/about.html
@@ -6,10 +6,7 @@
 <body>

 <h1>This is a About  page</h1>
-<p>Common bro is lame</p>
+<p>Common cook is lame</p>
 <p>Copying is sorry</p>
 </body>
 </html>
-
-
-

HP@ian MINGW32 ~/Bundle1 (dev)
$ git stash save "Stashing the changes of the about html living"
warning: in the working copy of 'about.html', LF will be replaced by CRLF the next time Git touches it
Saved working directory and index state On dev: Stashing the changes of the about html living

HP@ian MINGW32 ~/Bundle1 (dev)
$ vim team.html

HP@ian MINGW32 ~/Bundle1 (dev)
$ git add --all
warning: in the working copy of 'team.html', LF will be replaced by CRLF the next time Git touches it

HP@ian MINGW32 ~/Bundle1 (dev)
$ vim team.html

HP@ian MINGW32 ~/Bundle1 (dev)
$ git diff
warning: in the working copy of 'team.html', LF will be replaced by CRLF the next time Git touches it
diff --git a/team.html b/team.html
index d76b382..2bb6e84 100644
--- a/team.html
+++ b/team.html
@@ -7,7 +7,7 @@

 <h1>This is a Team  page</h1>
 <p>Common bro is teaming</p>
-<p>Copying is sorry</p>
+<p>Copying is</p>
 </body>
 </html>


HP@ian MINGW32 ~/Bundle1 (dev)
$ git stash save "Stashing the changes of the twam html live"
warning: in the working copy of 'team.html', LF will be replaced by CRLF the next time Git touches it
Saved working directory and index state On dev: Stashing the changes of the twam html live

HP@ian MINGW32 ~/Bundle1 (dev)
$ git stash list
stash@{0}: On dev: Stashing the changes of the twam html live
stash@{1}: On dev: Stashing the changes of the about html living
stash@{2}: On dev: Stashing the changes of the home html
stash@{3}: WIP on dev: 7933eab Adding Bundle 1 first commit

HP@ian MINGW32 ~/Bundle1 (dev)
$ git stash show -p stash@{1}
diff --git a/about.html b/about.html
new file mode 100644
index 0000000..0a0c849
--- /dev/null
+++ b/about.html
@@ -0,0 +1,12 @@
+<!DOCTYPE html>
+<html>
+<head>
+<title>Page Title</title>
+</head>
+<body>
+
+<h1>This is a About  page</h1>
+<p>Common cook is lame</p>
+<p>Copying is sorry</p>
+</body>
+</html>

HP@ian MINGW32 ~/Bundle1 (dev)
$ git stash pop stash@{1}
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html

Dropped stash@{1} (b6045611d715a729ee3fdb9152f51859d0fad03b)

HP@ian MINGW32 ~/Bundle1 (dev)
$ git stash pop stash@{2}
Auto-merging about.html
CONFLICT (add/add): Merge conflict in about.html
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   home.html
        new file:   team.html

Unmerged paths:
  (use "git restore --staged <file>..." to unstage)
  (use "git add <file>..." to mark resolution)
        both added:      about.html

The stash entry is kept in case you need it again.

HP@ian MINGW32 ~/Bundle1 (dev)
$ ^C

HP@ian MINGW32 ~/Bundle1 (dev)
$ cat about.html
<<<<<<< Updated upstream
<!DOCTYPE html>
<html>
<head>
<title>Page Title</title>
</head>
<body>

<h1>This is a About  page</h1>
<p>Common cook is lame</p>
<p>Copying is sorry</p>
</body>
</html>
=======
<!DOCTYPE>
<html>
<head>
<title>Wagwaan</title>
</head>
<body>
<h1>About Page</h1>
<p>This is an about page</p>
</body>
</html>
Bomboclat
>>>>>>> Stashed changes

HP@ian MINGW32 ~/Bundle1 (dev)
$ vim about.html

HP@ian MINGW32 ~/Bundle1 (dev)
$ git add about.html

HP@ian MINGW32 ~/Bundle1 (dev)
$ git status
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   home.html
        new file:   team.html


HP@ian MINGW32 ~/Bundle1 (dev)
$ cat team.html
No time to code but this is the plain text html file
Bomboclat

HP@ian MINGW32 ~/Bundle1 (dev)
$ git status
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   home.html
        new file:   team.html


HP@ian MINGW32 ~/Bundle1 (dev)
$ git commit -m "Commiting the old files from stash"
[dev 0dfe2f7] Commiting the old files from stash
 3 files changed, 32 insertions(+)
 create mode 100644 about.html
 create mode 100644 home.html
 create mode 100644 team.html

HP@ian MINGW32 ~/Bundle1 (dev)
$ git push -u origin dev
Enumerating objects: 6, done.
Counting objects: 100% (6/6), done.
Delta compression using up to 8 threads
Compressing objects: 100% (5/5), done.
Writing objects: 100% (5/5), 865 bytes | 288.00 KiB/s, done.
Total 5 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'dev' on GitHub by visiting:
remote:      https://github.com/i-ganza007/Bundle-1-/pull/new/dev
remote:
To github.com:i-ganza007/Bundle-1-.git
 * [new branch]      dev -> dev
branch 'dev' set up to track 'origin/dev'.

HP@ian MINGW32 ~/Bundle1 (dev)
$ git stash pop stash@{0}
Auto-merging team.html
CONFLICT (add/add): Merge conflict in team.html
On branch dev
Your branch is up to date with 'origin/dev'.

Unmerged paths:
  (use "git restore --staged <file>..." to unstage)
  (use "git add <file>..." to mark resolution)
        both added:      team.html

no changes added to commit (use "git add" and/or "git commit -a")
The stash entry is kept in case you need it again.

HP@ian MINGW32 ~/Bundle1 (dev)
$ cat team.html
<<<<<<< Updated upstream
No time to code but this is the plain text html file
Bomboclat
=======
<!DOCTYPE html>
<html>
<head>
<title>Page Title</title>
</head>
<body>

<h1>This is a Team  page</h1>
<p>Common bro is teaming</p>
<p>Copying is</p>
</body>
</html>



>>>>>>> Stashed changes

HP@ian MINGW32 ~/Bundle1 (dev)
$ vim team.html

HP@ian MINGW32 ~/Bundle1 (dev)
$ git status
On branch dev
Your branch is up to date with 'origin/dev'.

Unmerged paths:
  (use "git restore --staged <file>..." to unstage)
  (use "git add <file>..." to mark resolution)
        both added:      team.html

no changes added to commit (use "git add" and/or "git commit -a")

HP@ian MINGW32 ~/Bundle1 (dev)
$ git add team.html

HP@ian MINGW32 ~/Bundle1 (dev)
$ git status
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   team.html


HP@ian MINGW32 ~/Bundle1 (dev)
$ git reset --hard HEAD
HEAD is now at 0dfe2f7 Commiting the old files from stash

HP@ian MINGW32 ~/Bundle1 (dev)
$ git stash
No local changes to save

HP@ian MINGW32 ~/Bundle1 (dev)
$ git checkout stash@{2} -- home.html

HP@ian MINGW32 ~/Bundle1 (dev)
$ git checkout stash@{1} -- about.html
error: pathspec 'about.html' did not match any file(s) known to git

HP@ian MINGW32 ~/Bundle1 (dev)
$ git stash list
stash@{0}: On dev: Stashing the changes of the twam html live
stash@{1}: On dev: Stashing the changes of the home html
stash@{2}: WIP on dev: 7933eab Adding Bundle 1 first commit
```
#Bundle 2 Exercise 1
```bash
git checkout -b ft/bundle-2
Switched to a new branch 'ft/bundle-2'

HP@ian MINGW32 ~/Bundle1 (ft/bundle-2)
$ vim services.html

HP@ian MINGW32 ~/Bundle1 (ft/bundle-2)
$ git add --all
warning: in the working copy of 'services.html', LF will be replaced by CRLF the next time Git touches it

HP@ian MINGW32 ~/Bundle1 (ft/bundle-2)
$ echo "New line to services" >> services.html

HP@ian MINGW32 ~/Bundle1 (ft/bundle-2)
$ cat services.html
 <!DOCTYPE html>
<html>
<head>
<title>Hello World!</title>
<link rel="stylesheet" href="bluestyle.css">
</head>
<body>

<h1>Hello world!</h1>
<p>This is the services file.</p>
<p>A new line in our file!</p>

</body>
</html>
New line to services

HP@ian MINGW32 ~/Bundle1 (ft/bundle-2)
$ git add --all
warning: in the working copy of 'services.html', LF will be replaced by CRLF the next time Git touches it

HP@ian MINGW32 ~/Bundle1 (ft/bundle-2)
$ git commit -m "Bundle 2 exercises 1 commit"
[ft/bundle-2 684b1d8] Bundle 2 exercises 1 commit
 1 file changed, 15 insertions(+)
 create mode 100644 services.html

HP@ian MINGW32 ~/Bundle1 (ft/bundle-2)
$ git push
fatal: The current branch ft/bundle-2 has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/bundle-2

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


HP@ian MINGW32 ~/Bundle1 (ft/bundle-2)
$ git push -u ft/bundle-2 main
fatal: 'ft/bundle-2' does not appear to be a git repository
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.

HP@ian MINGW32 ~/Bundle1 (ft/bundle-2)
$ git push -u origin main
Everything up-to-date
branch 'main' set up to track 'origin/main'.

HP@ian MINGW32 ~/Bundle1 (ft/bundle-2)
$ git push -u origin ft/bundle-2
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 488 bytes | 122.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
remote:
remote: Create a pull request for 'ft/bundle-2' on GitHub by visiting:
remote:      https://github.com/i-ganza007/Bundle-1-/pull/new/ft/bundle-2
remote:
To github.com:i-ganza007/Bundle-1-.git
 * [new branch]      ft/bundle-2 -> ft/bundle-2
branch 'ft/bundle-2' set up to track 'origin/ft/bundle-2'.
```
#Bundle 2 Exercise 2 
```bash
 git checkout -b ft/service-redesign
Switched to a new branch 'ft/service-redesign'

HP@ian MINGW32 ~/Bundle1 (ft/service-redesign)
$ ls
Bundle-1-/  bundle1.py  services.html

HP@ian MINGW32 ~/Bundle1 (ft/service-redesign)
$ vim services.html

HP@ian MINGW32 ~/Bundle1 (ft/service-redesign)
$ git add --all

HP@ian MINGW32 ~/Bundle1 (ft/service-redesign)
$ git commit -m "Adding changes to the services for for bundle 2 exercise 2"
[ft/service-redesign 843c615] Adding changes to the services for for bundle 2 exercise 2
 1 file changed, 1 deletion(-)

HP@ian MINGW32 ~/Bundle1 (ft/service-redesign)
$ git push -u origin main
Everything up-to-date
branch 'main' set up to track 'origin/main'.

HP@ian MINGW32 ~/Bundle1 (ft/service-redesign)
$ cat services.htm
cat: services.htm: No such file or directory

HP@ian MINGW32 ~/Bundle1 (ft/service-redesign)
$ cat services.html
 <!DOCTYPE html>
<html>
<head>
<title>Hello World!</title>
<link rel="stylesheet" href="bluestyle.css">
</head>
<body>

<h1>Hello world!</h1>
<p>This is the services file.</p>

</body>
</html>
New line to services

HP@ian MINGW32 ~/Bundle1 (ft/service-redesign)
$ vim services.html

HP@ian MINGW32 ~/Bundle1 (ft/service-redesign)
$ git add services.html

HP@ian MINGW32 ~/Bundle1 (ft/service-redesign)
$ git status
On branch ft/service-redesign
nothing to commit, working tree clean

HP@ian MINGW32 ~/Bundle1 (ft/service-redesign)
$ git push -u origin ft/service-redesign
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 310 bytes | 103.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
remote:
remote: Create a pull request for 'ft/service-redesign' on GitHub by visiting:
remote:      https://github.com/i-ganza007/Bundle-1-/pull/new/ft/service-redesign
remote:
To github.com:i-ganza007/Bundle-1-.git
 * [new branch]      ft/service-redesign -> ft/service-redesign
branch 'ft/service-redesign' set up to track 'origin/ft/service-redesign'.

HP@ian MINGW32 ~/Bundle1 (ft/service-redesign)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

HP@ian MINGW32 ~/Bundle1 (main)
$ ls
Bundle-1-/  bundle1.py  services.html

HP@ian MINGW32 ~/Bundle1 (main)
$ vim services.html

HP@ian MINGW32 ~/Bundle1 (main)
$ git add --all

HP@ian MINGW32 ~/Bundle1 (main)
$ vim services.html

HP@ian MINGW32 ~/Bundle1 (main)
$ git add --all

HP@ian MINGW32 ~/Bundle1 (main)
$ git commit -m "Commiting from the main branch of the Bundle 2 Exercise 2"
[main df72430] Commiting from the main branch of the Bundle 2 Exercise 2
 1 file changed, 1 deletion(-)

HP@ian MINGW32 ~/Bundle1 (main)
$ git push -u origin main
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 310 bytes | 155.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To github.com:i-ganza007/Bundle-1-.git
   7dce98b..df72430  main -> main
branch 'main' set up to track 'origin/main'.

HP@ian MINGW32 ~/Bundle1 (main)
$ git checkout -b ft/service-redesign
fatal: a branch named 'ft/service-redesign' already exists

HP@ian MINGW32 ~/Bundle1 (main)
$ git checkout  ft/service-redesign
Switched to branch 'ft/service-redesign'
Your branch is up to date with 'origin/ft/service-redesign'.

HP@ian MINGW32 ~/Bundle1 (ft/service-redesign)
$ ls
Bundle-1-/  bundle1.py  services.html

HP@ian MINGW32 ~/Bundle1 (ft/service-redesign)
$ git diff

HP@ian MINGW32 ~/Bundle1 (ft/service-redesign)
$ cat services.html
 <!DOCTYPE html>
<html>
<head>
<title>Hello World!</title>
<link rel="stylesheet" href="bluestyle.css">
</head>
<body>

<h1>Hello world!</h1>
<p>This is the services file.</p>

</body>
</html>
New line to services

HP@ian MINGW32 ~/Bundle1 (ft/service-redesign)
$ git checkout  main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

HP@ian MINGW32 ~/Bundle1 (main)
$ ls
Bundle-1-/  bundle1.py  services.html

HP@ian MINGW32 ~/Bundle1 (main)
$ cat services.html
 <!DOCTYPE html>
<html>
<head>
<title>Hello World!</title>
<link rel="stylesheet" href="bluestyle.css">
</head>
<body>

<h1>Hello world!</h1>
<p>This is the services file.</p>

</body>
</html>
New line to services

HP@ian MINGW32 ~/Bundle1 (main)
$ git diff

HP@ian MINGW32 ~/Bundle1 (main)
$ git checkout  ft/service-redesign
Switched to branch 'ft/service-redesign'
Your branch is up to date with 'origin/ft/service-redesign'.

HP@ian MINGW32 ~/Bundle1 (ft/service-redesign)
$ git branch
  dev
  ft/bundle-2
* ft/service-redesign
  main

HP@ian MINGW32 ~/Bundle1 (ft/service-redesign)
$ git diff main..ft/service-redesign

HP@ian MINGW32 ~/Bundle1 (ft/service-redesign)
$ git checkout  ft/service-redesign
Already on 'ft/service-redesign'
Your branch is up to date with 'origin/ft/service-redesign'.

HP@ian MINGW32 ~/Bundle1 (ft/service-redesign)
$ vim services.html

HP@ian MINGW32 ~/Bundle1 (ft/service-redesign)
$ git add --all

HP@ian MINGW32 ~/Bundle1 (ft/service-redesign)
$ git commit -m "Commited to this branch to change stuff"
[ft/service-redesign fa5a39a] Commited to this branch to change stuff
 1 file changed, 1 insertion(+), 1 deletion(-)

HP@ian MINGW32 ~/Bundle1 (ft/service-redesign)
$ git push -u origin ft/service-redesign
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 331 bytes | 331.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To github.com:i-ganza007/Bundle-1-.git
   843c615..fa5a39a  ft/service-redesign -> ft/service-redesign
branch 'ft/service-redesign' set up to track 'origin/ft/service-redesign'.

HP@ian MINGW32 ~/Bundle1 (ft/service-redesign)
$ git diff

HP@ian MINGW32 ~/Bundle1 (ft/service-redesign)
$ git diff main..ft/service-redesign
diff --git a/services.html b/services.html
index 8523465..301acd6 100644
--- a/services.html
+++ b/services.html
@@ -8,7 +8,7 @@

 <h1>Hello world!</h1>
 <p>This is the services file.</p>
-
+<h1>Diego Dalot & Cincinatti</h1>
 </body>
 </html>
 New line to services

HP@ian MINGW32 ~/Bundle1 (ft/service-redesign)
$ git checkout main
Switched to branch 'main'

hint: Waiting for your editor to close the file.
[main 19b6199] Merge branch 'ft/service-redesign
```
#Bundle 3 Exercise 1 
```bash
HP@ian MINGW32 ~/Bundle1 (main)
$ git checkout -b ft/team-page
Switched to a new branch 'ft/team-page'

HP@ian MINGW32 ~/Bundle1 (ft/team-page)
$ vim team.html

HP@ian MINGW32 ~/Bundle1 (ft/team-page)
$ echo "<p>Adding some changes to the file</p>" >> team.html

HP@ian MINGW32 ~/Bundle1 (ft/team-page)
$ git add --all
warning: in the working copy of 'team.html', LF will be replaced by CRLF the next time Git touches it

HP@ian MINGW32 ~/Bundle1 (ft/team-page)
$ git commit -m "Commiting the team file"
[ft/team-page c006523] Commiting the team file
 1 file changed, 25 insertions(+)
 create mode 100644 team.html

HP@ian MINGW32 ~/Bundle1 (ft/team-page)
$ git push -u origin ft/team-page
Enumerating objects: 17, done.
Counting objects: 100% (17/17), done.
Delta compression using up to 8 threads
Compressing objects: 100% (14/14), done.
Writing objects: 100% (14/14), 2.47 KiB | 841.00 KiB/s, done.
Total 14 (delta 7), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (7/7), completed with 2 local objects.
remote:
remote: Create a pull request for 'ft/team-page' on GitHub by visiting:
remote:      https://github.com/i-ganza007/Bundle-1-/pull/new/ft/team-page
remote:
To github.com:i-ganza007/Bundle-1-.git
 * [new branch]      ft/team-page -> ft/team-page
branch 'ft/team-page' set up to track 'origin/ft/team-page'.

HP@ian MINGW32 ~/Bundle1 (ft/team-page)
$ git checkout main
Switched to branch 'main'
Your branch is ahead of 'origin/main' by 3 commits.
  (use "git push" to publish your local commits)

HP@ian MINGW32 ~/Bundle1 (main)
$ git checkout -b ft/contact-page
Switched to a new branch 'ft/contact-page'

HP@ian MINGW32 ~/Bundle1 (ft/contact-page)
$ git checkout ft/team-page
Switched to branch 'ft/team-page'
Your branch is up to date with 'origin/ft/team-page'.

HP@ian MINGW32 ~/Bundle1 (ft/team-page)
$ git log
commit c006523456a0904d04c5fa7f103b0c54700906bc (HEAD -> ft/team-page, origin/ft/team-page)
Author: i-ganza007 <i.ganza@alustudent.com>
Date:   Tue Dec 17 12:29:25 2024 +0200

    Commiting the team file

commit 19b6199ab91fe9e6882e5263e264dfd78a2ca1d7 (main, ft/contact-page)
Merge: df72430 fa5a39a
Author: i-ganza007 <i.ganza@alustudent.com>
Date:   Tue Dec 17 12:04:50 2024 +0200

    Merge branch 'ft/service-redesign'

commit fa5a39a64540004ef8d0e78f17d1e5d758516a71 (origin/ft/service-redesign, ft/service-redesign)
Author: i-ganza007 <i.ganza@alustudent.com>
Date:   Tue Dec 17 11:59:07 2024 +0200

    Commited to this branch to change stuff

commit df724301097f022bb66cca7678e26b51b954eccc (origin/main)
:
commit c006523456a0904d04c5fa7f103b0c54700906bc (HEAD -> ft/team-page, origin/ft/team-page)
Author: i-ganza007 <i.ganza@alustudent.com>
Date:   Tue Dec 17 12:29:25 2024 +0200

    Commiting the team file

commit 19b6199ab91fe9e6882e5263e264dfd78a2ca1d7 (main, ft/contact-page)
Merge: df72430 fa5a39a
Author: i-ganza007 <i.ganza@alustudent.com>
Date:   Tue Dec 17 12:04:50 2024 +0200

    Merge branch 'ft/service-redesign'

commit fa5a39a64540004ef8d0e78f17d1e5d758516a71 (origin/ft/service-redesign, ft/service-redesign)
Author: i-ganza007 <i.ganza@alustudent.com>
Date:   Tue Dec 17 11:59:07 2024 +0200

    Commited to this branch to change stuff

commit df724301097f022bb66cca7678e26b51b954eccc (origin/main)


HP@ian MINGW32 ~/Bundle1 (ft/team-page)
$

HP@ian MINGW32 ~/Bundle1 (ft/team-page)
$ git checkout ft/contact-page
Switched to branch 'ft/contact-page'

HP@ian MINGW32 ~/Bundle1 (ft/contact-page)
$ git cherry-pick fa5a39a64540004ef8d0e78f17d1e5d758516a71
Auto-merging services.html
CONFLICT (content): Merge conflict in services.html
error: could not apply fa5a39a... Commited to this branch to change stuff
hint: After resolving the conflicts, mark them with
hint: "git add/rm <pathspec>", then run
hint: "git cherry-pick --continue".
hint: You can instead skip this commit with "git cherry-pick --skip".
hint: To abort and get back to the state before "git cherry-pick",
hint: run "git cherry-pick --abort".

HP@ian MINGW32 ~/Bundle1 (ft/contact-page|CHERRY-PICKING)
$ ^C

HP@ian MINGW32 ~/Bundle1 (ft/contact-page|CHERRY-PICKING)
$ git cherry-pick fa5a39a
error: Cherry-picking is not possible because you have unmerged files.
hint: Fix them up in the work tree, and then use 'git add/rm <file>'
hint: as appropriate to mark resolution and make a commit.
fatal: cherry-pick failed

HP@ian MINGW32 ~/Bundle1 (ft/contact-page|CHERRY-PICKING)
$ git checkout ft/team-page
error: you need to resolve your current index first
services.html: needs merge

HP@ian MINGW32 ~/Bundle1 (ft/contact-page|CHERRY-PICKING)
$ ^C

HP@ian MINGW32 ~/Bundle1 (ft/contact-page|CHERRY-PICKING)
$ git status
On branch ft/contact-page
You are currently cherry-picking commit fa5a39a.
  (fix conflicts and run "git cherry-pick --continue")
  (use "git cherry-pick --skip" to skip this patch)
  (use "git cherry-pick --abort" to cancel the cherry-pick operation)

Unmerged paths:
  (use "git add <file>..." to mark resolution)
        both modified:   services.html

no changes added to commit (use "git add" and/or "git commit -a")

HP@ian MINGW32 ~/Bundle1 (ft/contact-page|CHERRY-PICKING)
$ git add --all

HP@ian MINGW32 ~/Bundle1 (ft/contact-page|CHERRY-PICKING)
$ git status
On branch ft/contact-page
You are currently cherry-picking commit fa5a39a.
hint: Waiting for your editor to close the file.[ft/contact-page 80fc97f] Commited to this branch to change stuff
 Date: Tue Dec 17 11:59:07 2024 +0200
 1 file changed, 4 insertions(+)

HP@ian MINGW32 ~/Bundle1 (ft/contact-page)
$ ^C

HP@ian MINGW32 ~/Bundle1 (ft/contact-page)
$ git log --oneline
80fc97f (HEAD -> ft/contact-page) Commited to this branch to change stuff
19b6199 (main) Merge branch 'ft/service-redesign'
fa5a39a (origin/ft/service-redesign, ft/service-redesign) Commited to this branch to change stuff
df72430 (origin/main) Commiting from the main branch of the Bundle 2 Exercise 2
843c615 Adding changes to the services for for bundle 2 exercise 2
7dce98b Merge pull request #1 from i-ganza007/ft/bundle-2
684b1d8 (origin/ft/bundle-2, ft/bundle-2) Bundle 2 exercises 1 commit
7933eab (dev) Adding Bundle 1 first commit
af85a83 Created the first bundle1 commit

HP@ian MINGW32 ~/Bundle1 (ft/contact-page)
$ ls
Bundle-1-/  bundle1.py  services.html

HP@ian MINGW32 ~/Bundle1 (ft/contact-page)
$ vim services.html

HP@ian MINGW32 ~/Bundle1 (ft/contact-page)
$ git add --all

HP@ian MINGW32 ~/Bundle1 (ft/contact-page)
$ git commit -a -m "Comming for the bundle 3 Exercise 1"
[ft/contact-page 74c0ba5] Comming for the bundle 3 Exercise 1
 1 file changed, 1 insertion(+)

HP@ian MINGW32 ~/Bundle1 (ft/contact-page)
$ git push -u origin ft/contact-page
Enumerating objects: 8, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 8 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 783 bytes | 391.00 KiB/s, done.
Total 6 (delta 3), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (3/3), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/contact-page' on GitHub by visiting:
remote:      https://github.com/i-ganza007/Bundle-1-/pull/new/ft/contact-page
remote:
To github.com:i-ganza007/Bundle-1-.git
 * [new branch]      ft/contact-page -> ft/contact-page
branch 'ft/contact-page' set up to track 'origin/ft/contact-page'.

HP@ian MINGW32 ~/Bundle1 (ft/contact-page)
$ git checkout -b ft/faq-page
Switched to a new branch 'ft/faq-page'

HP@ian MINGW32 ~/Bundle1 (ft/faq-page)
$ vim faq.html

HP@ian MINGW32 ~/Bundle1 (ft/faq-page)
$ git add --all
warning: in the working copy of 'faq.html', LF will be replaced by CRLF the next time Git touches it

HP@ian MINGW32 ~/Bundle1 (ft/faq-page)
$ git status
On branch ft/faq-page
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   faq.html


HP@ian MINGW32 ~/Bundle1 (ft/faq-page)
$ git commit -m "Commiting from a new branch faq file"
[ft/faq-page 101ae2b] Commiting from a new branch faq file
 1 file changed, 19 insertions(+)
 create mode 100644 faq.html

HP@ian MINGW32 ~/Bundle1 (ft/faq-page)
$ git push -u origin ft/faq-page
Enumerating objects: 11, done.
Counting objects: 100% (11/11), done.
Delta compression using up to 8 threads
Compressing objects: 100% (9/9), done.
Writing objects: 100% (9/9), 1.33 KiB | 169.00 KiB/s, done.
Total 9 (delta 3), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (3/3), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/faq-page' on GitHub by visiting:
remote:      https://github.com/i-ganza007/Bundle-1-/pull/new/ft/faq-page
remote:
To github.com:i-ganza007/Bundle-1-.git
 * [new branch]      ft/faq-page -> ft/faq-page
branch 'ft/faq-page' set up to track 'origin/ft/faq-page'.

HP@ian MINGW32 ~/Bundle1 (ft/faq-page)
$ git checkout -b ft/team-page
fatal: a branch named 'ft/team-page' already exists

HP@ian MINGW32 ~/Bundle1 (ft/faq-page)
$ git checkout  ft/team-page
Switched to branch 'ft/team-page'
Your branch is up to date with 'origin/ft/team-page'.

HP@ian MINGW32 ~/Bundle1 (ft/team-page)
$ <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <style>
        *{
            font-family: sans-serif;
        }
        #main-photo{
            max-width: 280px;
            border-radius: 10px;
        }
        .outer-container{
            display: flex;
            flex-direction: column;
        }
        .order-container{
            display: flex;
            border: 1.3px solid;
            max-width: 187px;
            text-align: center;
            justify-content: center;
            gap: 7px;
            border-radius: 30px;
</html>:q>div> id="price">$6.50</p></h2> Cart</p
bash: !DOCTYPE: event not found
bash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `newline'
bash: *{: command not found
bash: font-family:: command not found
bash: syntax error near unexpected token `}'
bash: max-width:: command not found
bash: border-radius:: command not found
bash: syntax error near unexpected token `}'
bash: .outer-container{: command not found
bash: display:: command not found
bash: flex-direction:: command not found

bash: syntax error near unexpected token `}'

bash: .order-container{: command not found


bash: display:: command not found
bash: text-align:: command not found
bash: gap:: command not foundnd not found
bash: border-radius:: command not found
bash: outline:: command not found
bash: position:: command not found
bash: left:: command not found
bash: bottom:: command not found
bash: opacity:: command not found
bash: background-color:: command not found
bash: margin-bottom:: command not found

bash: syntax error near unexpected token `}'
bash: font-weight:: command not found
bash: syntax error near unexpected token `}'
bash: color:: command not found
bash: syntax error near unexpected token `}'
bash: syntax error near unexpected token `('
bash: font-weight:: command not found
bash: syntax error near unexpected token `}'





bash: .text-content{: command not found
bash: max-height:: command not found
bash: syntax error near unexpected token `}'
bash: .text-content: command not found

bash: margin-top:-0.5rem: command not found
bash: margin-bottom:: command not found
bash: syntax error near unexpected token `}'
bash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `newline'
ash: syntax error near unexpected token `newline'
ash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `newline'
;bash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `newline'
;bash: syntax error near unexpected token `newline'
bash: syntax error near unexpected token `newline'
;bash: syntax error near unexpected token `newline'

bash: syntax error near unexpected token `newline'
qbash: syntax error near unexpected token `newline'
bash: /html: No such file or directory
q
HP@ian MINGW32 ~/Bundle1 (ft/team-page)
$ ^[;;;;;q
bash: syntax error near unexpected token `;;'
q
HP@ian MINGW32 ~/Bundle1 (ft/team-page)
$ qqq
bash: qqq: command not found

q
HP@ian MINGW32 ~/Bundle1 (ft/team-page)
$

HP@ian MINGW32 ~/Bundle1 (ft/team-page)
$ qq
bash: qq: command not found

HP@ian MINGW32 ~/Bundle1 (ft/team-page)
$ git cherry-pick
usage: git cherry-pick [--edit] [-n] [-m <parent-number>] [-s] [-x] [--ff]
                       [-S[<keyid>]] <commit>...
   or: git cherry-pick (--continue | --skip | --abort | --quit)

    --quit                end revert or cherry-pick sequence
    --continue            resume revert or cherry-pick sequence
    --abort               cancel revert or cherry-pick sequence
    --skip                skip current commit and continue
    --cleanup <mode>      how to strip spaces and #comments from message
    -n, --no-commit       don't automatically commit
    -e, --edit            edit the commit message
    -s, --signoff         add a Signed-off-by trailer
    -m, --mainline <parent-number>
                          select mainline parent
    --rerere-autoupdate   update the index with reused conflict resolution if possible
    --strategy <strategy>
                          merge strategy
    -X, --strategy-option <option>
                          option for merge strategy
    -S, --gpg-sign[=<key-id>]
                          GPG sign commit
    -x                    append commit name
    --ff                  allow fast-forward
    --allow-empty         preserve initially empty commits
    --allow-empty-message
                          allow commits with empty messages
    --keep-redundant-commits
                          keep redundant, empty commits


HP@ian MINGW32 ~/Bundle1 (ft/team-page)
$ git log
commit c006523456a0904d04c5fa7f103b0c54700906bc (HEAD -> ft/team-page, origin/ft/team-page)
Author: i-ganza007 <i.ganza@alustudent.com>
Date:   Tue Dec 17 12:29:25 2024 +0200

    Commiting the team file

commit 19b6199ab91fe9e6882e5263e264dfd78a2ca1d7 (main)
Merge: df72430 fa5a39a
Author: i-ganza007 <i.ganza@alustudent.com>
Date:   Tue Dec 17 12:04:50 2024 +0200

    Merge branch 'ft/service-redesign'

commit fa5a39a64540004ef8d0e78f17d1e5d758516a71 (origin/ft/service-redesign, ft/service-redesign)
Author: i-ganza007 <i.ganza@alustudent.com>
Date:   Tue Dec 17 11:59:07 2024 +0200

    Commited to this branch to change stuff

commit df724301097f022bb66cca7678e26b51b954eccc
(origin/main)
:
commit c006523456a0904d04c5fa7f103b0c54700906bc (HEAD -> ft/team-page, origin/ft/team-page)
Author: i-ganza007 <i.ganza@alustudent.com>
Date:   Tue Dec 17 12:29:25 2024 +0200

    Commiting the team file

commit 19b6199ab91fe9e6882e5263e264dfd78a2ca1d7 (main)
Merge: df72430 fa5a39a
Author: i-ganza007 <i.ganza@alustudent.com>
Date:   Tue Dec 17 12:04:50 2024 +0200

    Merge branch 'ft/service-redesign'

commit fa5a39a64540004ef8d0e78f17d1e5d758516a71 (origin/ft/service-redesign, ft/service-redesign)
Author: i-ganza007 <i.ganza@alustudent.com>
Date:   Tue Dec 17 11:59:07 2024 +0200

    Commited to this branch to change stuff

commit df724301097f022bb66cca7678e26b51b954eccc (origin/main)
Author: i-ganza007 <i.ganza@alustudent.com>

HP@ian MINGW32 ~/Bundle1 (ft/team-page)
$
q
HP@ian MINGW32 ~/Bundle1 (ft/team-page)
hint: Waiting for your editor to close the file.[ft/team-page 817b688] Revert "Commiting the team file"
 1 file changed, 25 deletions(-)
 delete mode 100644 team.html

HP@ian MINGW32 ~/Bundle1 (ft/team-page)
$ git push origin ft/team-page
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 253 bytes | 84.00 KiB/s, done.
Total 2 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To github.com:i-ganza007/Bundle-1-.git
   c006523..817b688  ft/team-page -> ft/team-pag
```
