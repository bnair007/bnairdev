# bnairdev


https://github.com/bijithnair007/bnairdev.git

…or create a new repository on the command line

echo "# bnairdev" >> README.md
git init
git add README.md
git commit -m "first commit"
git remote add origin https://github.com/bijithnair007/bnairdev.git
git push -u origin master
…or push an existing repository from the command line

git remote add origin https://github.com/bijithnair007/bnairdev.git
git push -u origin master
…or import code from another repository
You can initialize this repository with code from a Subversion, Mercurial, or TFS project.

Import code

---
ssh

git@github.com:bijithnair007/bnairdev.git

…or create a new repository on the command line

echo "# bnairdev" >> README.md
git init
git add README.md
git commit -m "first commit"
git remote add origin git@github.com:bijithnair007/bnairdev.git
git push -u origin master
…or push an existing repository from the command line

git remote add origin git@github.com:bijithnair007/bnairdev.git
git push -u origin master

====================
git add <filename>
git rm <filename>
git status
git commit -m "log"
git status
git push -u origin master

error
====
[root@scriptdev Linux_Server]# git push -u origin master
To git@github.com:bijithnair007/bnairdev.git
 ! [rejected]        master -> master (non-fast-forward)
error: failed to push some refs to 'git@github.com:bijithnair007/bnairdev.git'
To prevent you from losing history, non-fast-forward updates were rejected
Merge the remote changes before pushing again.  See the 'Note about
fast-forwards' section of 'git push --help' for details.
--
sol:git pull --rebase
