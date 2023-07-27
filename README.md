$ sudo apt-get update
Hit:1 http://security.ubuntu.com/ubuntu focal-security InRelease
Hit:2 http://archive.ubuntu.com/ubuntu focal InRelease
Hit:3 http://archive.ubuntu.com/ubuntu focal-updates InRelease
Hit:4 http://archive.ubuntu.com/ubuntu focal-backports InRelease
Reading package lists... Done
$ sudo apt-get install git
Reading package lists... Done
Building dependency tree       
Reading state information... Done
The following additional packages will be installed:
  git-man liberror-perl
Suggested packages:
  git-daemon-run | git-daemon-sysvinit git-doc git-el git-email git-gui gitk gitweb git-cvs git-mediawiki git-svn
The following NEW packages will be installed:
  git git-man liberror-perl
0 upgraded, 3 newly installed, 0 to remove and 0 not upgraded.
Need to get 6,195 kB of archives.
After this operation, 34.3 MB of additional disk space will be used.
Do you want to continue? [Y/n] y
Get:1 http://archive.ubuntu.com/ubuntu focal/main amd64 liberror-perl all 0.17029-1 [26.2 kB]
Get:2 http://archive.ubuntu.com/ubuntu focal-updates/main amd64 git-man all 1:2.25.1-1ubuntu3.1 [803 kB]
Get:3 http://archive.ubuntu.com/ubuntu focal-updates/main amd64 git amd64 1:2.25.1-1ubuntu3.1 [5,366 kB]
Fetched 6,195 kB in 1s (4,464 kB/s)
Selecting previously unselected package liberror-perl.
(Reading database ... 170983 files and directories currently installed.)
Preparing to unpack .../liberror-perl_0.17029-1_all.deb ...
Unpacking liberror-perl (0.17029-1) ...
Selecting previously unselected package git-man.
Preparing to unpack .../git-man_1%3a2.25.1-1ubuntu3.1_all.deb ...
Unpacking git-man (1:2.25.1-1ubuntu3.1) ...
Selecting previously unselected package git.
Preparing to unpack .../git_1%3a2.25.1-1ubuntu3.1_amd64.deb ...
Unpacking git (1:2.25.1-1ubuntu3.1) ...
Setting up liberror-perl (0.17029-1) ...
Setting up git-man (1:2.25.1-1ubuntu3.1) ...
Setting up git (1:2.25.1-1ubuntu3.1) ...
$ git config --global user.name "Your Name"
$ git config --global user.email "your.email@example.com"
$ mkdir rebrain-devops-task1
$ cd rebrain-devops-task1
$ git init
Initialized empty Git repository in /home/user/rebrain-devops-task1/.git/
$ nano nginx.conf # добавляем конфигурацию nginx
$ nano README.md # добавляем описание репозитория
$ git add README.md
$ git commit -m "Added README.md"
[master (root-commit) 9e1f10e] Added README.md
 1 file changed, 1 insertion(+)
 create mode 100644 README.md
$ git add nginx.conf
$ git commit -m "Added nginx.conf"
[master 0c97b1d] Added nginx.conf
 1 file changed, 23 insertions(+)
 create mode 100644 nginx.conf
$ git log
commit 0c97b1d6a0a1df7d2b2b8a8f9d2b7f1d3a3b2f4c (HEAD -> master)
Author: Your Name <your.email@example.com>
Date:   Tue Jul 27 08:00:00 2023 +0000

    Added nginx.conf

commit 9e1f10ea0a1df7d2b2b8a8f9d2b7f1d3a3b2f4c
Author: Your Name <your.email@example.com>
Date:   Tue Jul 27 07:50:00 2023 +0000

    Added README.md

$ git status
On branch master
nothing to commit, working tree clean
