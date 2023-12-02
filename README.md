## gitLearning

commands to cover:

linux:
ls
cd
explorer.exe .
code .

1. `git add filename.txt` - similar to putting some items (changes) into a box. It's easy to get them out, and they are all in one place.
    - `git add .` - generally considered bad practice (but you will start doing it anyway). Adds all changes you made in repository.

2. `git commit -m "text"` - equivalent of sealing the package an putting it into a post box. A bit harder to **revert**, package has date and name on it. Usually used with `-m` flag to quickly add commit message.

3. `git push` - comparable to postman taking your package somwhere. Pretty hard to cancel, package is in a **remote** location.
    - `git push -f` - force push. Overwrites data on remote with yours. Usefull when you want to remove commits from a remote. Use with caution.

4. `git pull` - a bit like getting a delivery. git pull tries to automatically merge your changes with remote
    - `git fetch` - sub-command of git pull. Downloads changes, but does not merge them.

5. `git reset`
    - `HEAD^` - allows you to delete last commit
    - `--hard` - removes changes completely
    - `--soft` - removes commit, and moves changes back to staging area

6. `git status` - lists files on staging ara

7. `git stash` - similar to a commit, but it should exist only temporarly.

8. `git clone` - download all files from a specific repositorium

9. `git branch`
    - `git branch new`

10. `git rebase` - preffered over merge. "Uproots" branch you are currently on, and attaches it to specified other branch/commit

11. `git merge` - unifies two distinct timelines

12. `git squash`

13. `git checkout` - allows you to peek at a particular commit, or change branch
    - `git switch` - allows you to change branch

14. `git log` - shows you info about last commits
    - `git log --oneline` -
    - vim

15. `git init`

16. `git revert`

topics:
git vs github (porn vs pornhub)
pull requests
markdown (ctrl + shift + v)

do not commit on master
staging area
repository
commit messages
commit frequency
