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
