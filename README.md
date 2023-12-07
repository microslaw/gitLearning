# Learning git

---

### I part - git basics

commands to cover:

#### linux:

- `ls` - list files in current directory
- `cd` - move to a specific directory. `cd ..` - move to parent directory
- `explorer.exe .` - opens file explorer in current directory
- `code .` - opens the best code editor in current directory

#### git:

1. `git clone` - download all files from a specific repositorium

2. `git init` - creates a new git repository in current directory

3. `git add filename.txt` - similar to putting some items (changes) into a box. It's easy to get them out, and they are all in one place.
   - `git add .` - generally considered bad practice (but you will start doing it anyway). Adds all changes you made in repository.

4. `git status` - lists files on staging area

5. `git commit -m "text"` - equivalent of sealing the package an putting it into a post box. A bit harder to **revert**, package has date and name on it. Usually used with `-m` flag to quickly add commit message.

6. `git push` - comparable to postman taking your package somwhere. Pretty hard to cancel, package is in a **remote** location.
   - `git push -f` - force push. Overwrites data on remote with yours. Usefull when you want to remove commits from a remote. Use with caution.

7. `git pull` - a bit like getting a delivery. git pull tries to automatically merge your changes with remote
   - `git fetch` - sub-command of git pull. Downloads changes, but does not merge them.

8. `git reset`
   - `HEAD^` - allows you to delete last commit
   - `HEAD~2` - allows you to delete last two commits
   - `--hard` - removes changes completely
   - `--soft` - removes commit, and moves changes back to staging area

9. `git stash` - similar to a commit, but it should exist only temporarly.

10. `git checkout` - allows you to peek at a particular commit, or change branch
    - `git switch` - allows you to change branch

11. `git log` - shows you info about last commits
    - `git log --oneline` - more brief info
    - vim - to exit press :q
    - `git log --oneline --graph` - shows you a graph of commits. usefull on more complex repositiories
    - `git log --graph --pretty=oneline --abbrev-commit` - same but prettier

---

### II part - co-editing a repository

12. `git branch` - lists all local branches of your repository

    - `git branch new`
    - `git branch -a` - lists all branches (remote included)
13. `git rebase` - preffered over merge. "Uproots" branch you are currently on, and attaches it to specified other branch/commit

    - `git rebase -i` - interactive rebase. Allows you to change commits before they are applied to the branch you are rebasing on. Very powerfull and versatile, detailed instruction appears after running the command
14. `git merge` - unifies two distinct timelines

15. `git revert` - creates a new commit that reverts changes from a specified commit (it adds another commit, cancelling changes from previous, but does not delete it's predacessor)
