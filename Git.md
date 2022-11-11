# Useful Git commands

* Diff a file with HEAD after modified:
  * If file is not added: `git diff myfile.txt`
  * If file is added: `git diff --cached myfile.txt`
* Safer force push (ensure that do not override other's work to a branch): `git push --force-with-lease`
* Assume a file is unchanged:
  * Assump file unchange: `git update-index --assume-unchanged [files]`
  * Undo: `git update-index --no-assume-unchanged [files]`
  * List of dirs/files that are assumped unchanged: `git ls-files -v|grep '^h'`
