# git-alias
List of common git aliases I've created/found and find useful.

## Usage
Add any of these aliases to your .gitconfig under the ```[alias]``` section. Commands can be used via ```git <alias>```.

### Short form
These aliases are just to satisfy the lazy bastard in me and reduce the need of memorizing some of the switches.
- co ```git checkout```
- aa ```git add --all```
- au ```git add --update```
- ca ```git commit --amend``` Amends the previous commit.
- cm ```git commit -m``` Commit with message
- cp ```git cherry-pick```
- purge ```git clean -fdx``` Removes ignored and untracked files recursively. Useful for resetting from scratch.
- ls ```git ls-files``` Shows file information from the current tree.
- dt ```git difftool```
- mt ```git mergetool```
- nb ```git checkout -b``` Checkout to a new branch, e.g. ```git nb my-new-branch```
- branches ```git branch -l``` Lists the local branches
- trim ```git branch -d``` Deletes a local branch
- logh = ```git log --date=human``` Displays the log with human readable dates.
- ig ```git update-index --assume-unchanged``` Ignores changes to a tracked file or path.
- sig ```update-index --no-assume-unchanged``` Resumes normal tracking for changes to a tracked file or path.

### Helpers
- myconfig -- Opens the global git configuration for editing
- feature -- Creates a new branch with a 'feature' prefix.  _e.g. ```git feature my-updates``` will create a new branch as 'feature/my-new-updates'_
- bugfix -- Creates a new branch with a 'bugfix' prefix similar to ```feature```.
- buzzsaw -- Attempts to delete all local branches. Sketchy. Usually will fail to delete the checked out branch, so it's useful if there's a pile of dead branches in your local sources.
