git clone ssh

ls      list everything from directory

git status      shows the file that was not part of last commit and modified files

git add .       to track all the new files and modified one
git add file.ex/path        to track single file
git commit -m "summery" -m "description"
git push
git push origin master


start repository locally
cd path         to change the file path
git init        make the non-repo file a git repo
the repo doesn't exist on github thats why can't be pushed
to push local repo to github, a same name repo is made on github
git remote add origin githubSSH
git push -u origin master
now on git push will work fine.

git undoing
git add .       stag all the changes
git reset fileName/.       to unstag the git change

undoing after commit
git commit -m ""
git reset HEAD~1        to go one commit before
git diff        to see the modifications
git log         to see the commits
git reset HASHnum       to go back to a specific commit and unstag any change
git reset --hard HASHnum        not only unstag the change also erase the change

copying others repo
fork
pull request        to at the my file to the original repo where I copied the repo from.


git pull
git fetch
git fetch --all