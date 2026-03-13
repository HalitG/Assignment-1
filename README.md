The command that were used were:

touch project.txt - to create the file
git init - to initialize the repo
git add project.txt - multiple times while changing the file
git commit -m (with the provided message three times)
git log - so i can see all the commits
git rebase -i --root - for stashing and changing the commit to one line with an effective message
git commit -m "mistake commit" - to pretend i made a mistake
git reset --hard HEAD~1 // HEAD is now at f679aa0 Initial project setup
git reflog - to see where the mistake commit is // it was at fe59977
git checkout fe59977 - it switched to fe59977
git branch recovered-work 
git branch --global alisa.visual "log --online --graph --decorate --all" and the i used git visual and it
displayed: fe59977 (HEAD, recovered-work) mistake commit
           f679aa0 (master) Initial project setup)
git branch main - to create the main branch
git switch main - to locate the HEAD to main branch
git tag -a v1.0 -m "  t  he project version 1.0 is cleaned"

Then finally the push to github using:
git push -u origin main --force
git push origin recovered-work
git push origin v1.0
git push origin master
