PS C:\Users\User\Documents\Github> git clone https://github.com/szabopeter92/git-vizsga.git
Cloning into 'git-vizsga'...
remote: Enumerating objects: 15, done.
remote: Compressing objects: 100% (15/15), done.
Receiving objects: 100% (15/15), 14.06 MiB | 7.80 MiB/s, done.

PS C:\Users\User\Documents\Github> cd git-vizsga
Reinitialized existing Git repository in C:/Users/User/Documents/Github/git-vizsga/.git/

PS C:\Users\User\Documents\Github\git-vizsga> git status
Your branch is up to date with 'origin/main'.
nothing to commit, working tree clean

PS C:\Users\User\Documents\Github\git-vizsga> git checkout -b console
Switched to a new branch 'console'

PS C:\Users\User\Documents\Github\git-vizsga> git branch
* console
  main

PS C:\Users\User\Documents\Github\git-vizsga> git status
On branch console
nothing to commit, working tree clean

PS C:\Users\User\Documents\Github\git-vizsga> git add .

PS C:\Users\User\Documents\Github\git-vizsga> git status
On branch console
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   .gitignore
        new file:   README.MD
        modified:   app.js 

PS C:\Users\User\Documents\Github\git-vizsga> git commit . -m "First Change" 
[console 5d76313] First Change
 3 files changed, 40 insertions(+)
 create mode 100644 .gitignore
 create mode 100644 README.MD

PS C:\Users\User\Documents\Github\git-vizsga> git remote set-url origin git@github.com:Missikito/git-vizsga.git

PS C:\Users\User\Documents\Github\git-vizsga> git status
On branch console
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.MD
        modified:   style.css

no changes added to commit (use "git add" and/or "git commit -a")

PS C:\Users\User\Documents\Github\git-vizsga> git add .

PS C:\Users\User\Documents\Github\git-vizsga> git commit . -m "Second Change"
[console cf34140] Second Change
 2 files changed, 25 insertions(+), 3 deletions(-)
