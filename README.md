#Introduction
This is the testing repo where you can do everything GIT!

#Git HELP
##cvs update
Git doesn't have the update command so, to pull updated from a branch, you do ``git pull origin <branch>``

##merge branch
``git checkout <target_branch>``

``git merge <working_branch>``

##tagging
``git tag -a x.x.x -m 'message'``

``git push --tags``

##branching
Git allows you to make branches locallay without having to push them back to the origin repo

Lets say you wanted to work on a new feature in a new branch you could do this:

``git checkout -b some-feature develop`` which is ``git checkout -b <new_branch> <source_branch>``

from there you can do

``
git status
git add <some-file>
git commit
``

to add more files. Then to merge back into the development branch and remove your custom feature branch:

``
git pull origin develop; 
git checkout develop; 
git merge some-feature; 
git push; 
git branch -d some-feature
``
DO YOU BELIEVE IN LIFE AFTER LOVE?!?!?