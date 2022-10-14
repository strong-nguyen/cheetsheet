# Useful Git commands

* Diff a file with HEAD after modified:
  * If file is not added: `git diff myfile.txt`
  * If file is added: `git diff --cached myfile.txt`
* Safer force push (ensure that do not override other's work to a branch): `git push --force-with-lease`
