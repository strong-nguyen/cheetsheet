# Useful Git commands

* Diff a file with HEAD after modified:
  * If file is not added: `git diff myfile.txt`
  * If file is added: `git diff --cached myfile.txt`
* Safer force push (ensure that do not override other's work to a branch): `git push --force-with-lease`
* Assume a file is unchanged:
  * Assump file unchange: `git update-index --assume-unchanged [files]`
  * Undo: `git update-index --no-assume-unchanged [files]`
  * List of dirs/files that are assumped unchanged: `git ls-files -v|grep '^h'`
* Checkout to a specific tag: `git checkout tags/<tag> -b <branch>`
* Fetch a remote branch to local:
```
git fetch origin <branch_name>
git checkout -b branch_name FETCH_HEAD
```
* Show what has changed: `git whatchanged`
* Change branch name: `git branch -m new_name`
