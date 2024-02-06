Sir im facing issue with pushing files on to remote repo.
PS C:\Users\abhij\ecom> git push -u ecom-practise-website main
fatal: 'ecom-practise-website' does not appear to be a git repository
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.
 adn when i check the branch and repo initialised the info i had given the commands are correct but still showing error.

 PS C:\Users\abhij\ecom> git init
Reinitialized existing Git repository in C:/Users/abhij/ecom/.git/
PS C:\Users\abhij\ecom> git branch
* main
PS C:\Users\abhij\ecom> ls 


    Directory: C:\Users\abhij\ecom


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
d-----          2/6/2024  10:10 AM                node_modules
d-----          2/6/2024  10:09 AM                public
d-----          2/6/2024  10:43 AM                src
-a----         1/29/2024   2:28 PM            526 .eslintrc.cjs
-a----         1/29/2024   2:28 PM            253 .gitignore
-a----          2/6/2024  11:44 AM           1972 index.html
-a----          2/6/2024  10:10 AM         144203 package-lock.json
-a----          2/6/2024  10:09 AM            649 package.json
-a----          2/6/2024  10:39 AM        5548424 product1.jpg
-a----          2/6/2024  10:38 AM        6520065 product2.jpg
-a----          2/6/2024  10:38 AM        8367103 product3.jpg
-a----          2/6/2024  10:37 AM         949078 product4.jpg
-a----         1/29/2024   2:28 PM            451 README.md
-a----         1/29/2024   2:28 PM            163 vite.config.js


PS C:\Users\abhij\ecom> git remote add origin https://github.com/ABHI-PANCHAMI/ecom-practise-website.git
error: remote origin already exists.
PS C:\Users\abhij\ecom> git pull origin main  
remote: Enumerating objects: 13, done.
remote: Counting objects: 100% (13/13), done.
remote: Compressing objects: 100% (13/13), done.
remote: Total 13 (delta 0), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (13/13), 18.96 MiB | 3.62 MiB/s, done.
From https://github.com/ABHI-PANCHAMI/ecom-practise-website
 * branch            main       -> FETCH_HEAD
 * [new branch]      main       -> origin/main
fatal: refusing to merge unrelated histories
PS C:\Users\abhij\ecom> git status
On branch main
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   index.html
        modified:   src/index.css

no changes added to commit (use "git add" and/or "git commit -a")
PS C:\Users\abhij\ecom> git add .
warning: in the working copy of 'index.html', LF will be replaced by CRLF the next time Git touches it
warning: in the working copy of 'src/index.css', LF will be replaced by CRLF the next time Git touches it
PS C:\Users\abhij\ecom> git add .
PS C:\Users\abhij\ecom> git push
fatal: The current branch main has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin main

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

PS C:\Users\abhij\ecom>  git push --set-upstream origin main
To https://github.com/ABHI-PANCHAMI/ecom-practise-website.git
 ! [rejected]        main -> main (non-fast-forward)
error: failed to push some refs to 'https://github.com/ABHI-PANCHAMI/ecom-practise-website.git'
hint: Updates were rejected because the tip of your current branch is behind
hint: its remote counterpart. If you want to integrate the remote changes,
hint: use 'git pull' before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
PS C:\Users\abhij\ecom> git pull
There is no tracking information for the current branch.
Please specify which branch you want to merge with.
See git-pull(1) for details.

    git pull <remote> <branch>

If you wish to set tracking information for this branch you can do so with:

    git branch --set-upstream-to=origin/<branch> main

PS C:\Users\abhij\ecom> git pull https://github.com/ABHI-PANCHAMI/ecom-practise-website.git main        
From https://github.com/ABHI-PANCHAMI/ecom-practise-website
 * branch            main       -> FETCH_HEAD
fatal: refusing to merge unrelated histories
PS C:\Users\abhij\ecom>




