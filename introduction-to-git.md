# Introduction to Git

A brief tour of Git and GitHub for Data Scientists.

By Jeremy Nickurak.

## Version control

### Why version control?

* Can undo in a more fine grained manner.
* Can explain the steps you took.
	* Commits create a 'trail of breadcrumbs'.

## Basics

* `git init`
* `git status`
* `git add`
	* `git add -p` interactively adds data hunk by hunk
* `git commit`
* `git commit --ammend`
	* change commit message
* `git diff`
	* compare your working copy to committed copy
* `git log`
	* lists the commits
	* `git log --oneline` condenses
* `git reflog`
	* automatic trail
	* has hashes that work with reset...
* `git reset --hard ${hash}`
	* Resets the index and working tree to the commit specified by the hash.
	* Without the `--hard` git resets the index but not working tree.
	* Without the hash it will go to the `HEAD`.

### Good commit messages

* As small as they can be.
	* while still adding value
* Can be used to tell a story.
	* This can help you work in a goal-oriented way.

## Basics for working with others

### Distributed version control

* Traditionally version control was centralised.
	* I.e. there was a master branch on a server somewhere.
	* Have to create locks on files.
 
* Every copy is a fully functional repository.
	* Can work without an internet connection.
	* One can recover from virtually anything.
	* This is another reason why git clones the entire repository.

### GitHub 

Most popular hosting solution for Git.
* Also has community features.