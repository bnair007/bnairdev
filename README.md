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

Checking existing SSH Keys

$ ls -al ~/.ssh         # Lists the files in your .ssh directory, if they exist



Generate an SSH Key

# Generates public/private rsa key pair with default values - DON'T RUN THIS ONE
$ ssh-keygen           

 # 't' for type of key, 'b' for length of key, 'C' for comment for maintaining multiple keys                                
$ ssh-keygen -t rsa -b 2048 - C "home machine"


         
Enable SSH Agent & add the SSH Key to the agent

# start the ssh-agent in the background
$ eval "$(ssh-agent -s)"        

# Add your SSH key to the ssh-agent    
$ ssh-add ~/.ssh/id_rsa.pub           



Testing SSH connection

# Verify SSH connection; here 'git" is the user name; note that you cannot use your github user name such as 'william'
$ ssh -T git@github.com                 

# another alternative way to verify if firewall issues are present
$ ssh -T -p 443 git@github.com          



Remote URL switching and SSH push

# List your existing remotes in order to get the name of the remote you want to change
$ git remote -v      

 # set remote URL
$ git git remote set-url origin git@github.com:USERNAME/OTHERREPOSITORY.git       

 # Verify new remote URL  
$ git remote -v                                



Changing passphrase

# for changing password occasionally
$ ssh-keygen -p          

 
Browse Q&A
Continue


   
Go to Dashboard


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

=============================================

SSH
=============================================

Command Summary (GitHub via SSH)
Section 10, Lecture 53
Checking existing SSH Keys

$ ls -al ~/.ssh         # Lists the files in your .ssh directory, if they exist



Generate an SSH Key

# Generates public/private rsa key pair with default values - DON'T RUN THIS ONE
$ ssh-keygen           

 # 't' for type of key, 'b' for length of key, 'C' for comment for maintaining multiple keys                                
$ ssh-keygen -t rsa -b 2048 - C "home machine"


         
Enable SSH Agent & add the SSH Key to the agent

# start the ssh-agent in the background
$ eval "$(ssh-agent -s)"        

# Add your SSH key to the ssh-agent    
$ ssh-add ~/.ssh/id_rsa.pub           



Testing SSH connection

# Verify SSH connection; here 'git" is the user name; note that you cannot use your github user name such as 'william'
$ ssh -T git@github.com                 

# another alternative way to verify if firewall issues are present
$ ssh -T -p 443 git@github.com          



Remote URL switching and SSH push

# List your existing remotes in order to get the name of the remote you want to change
$ git remote -v      

 # set remote URL
$ git git remote set-url origin git@github.com:USERNAME/OTHERREPOSITORY.git       

 # Verify new remote URL  
$ git remote -v                                



Changing passphrase

# for changing password occasionally
$ ssh-keygen -p          

 
Browse Q&A
Continue


   
Go to Dashboard

