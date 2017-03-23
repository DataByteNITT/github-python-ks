# Now, lets look at some other functionality of git:
* `git log` this is used to look at the project history and what we have done so far.
* `git log --stat --summary` this is used for viewing summary and stats about each commit done so far.


###### <u>NOTE: the following content is on test-branch</u>

# Branches are next
- Run this command `git branch`, and you will see
	- *master
	- and more branches will be listed depending on the repo 
- To create a new branch run `git branch test-branch` and run `git branch`
	- *master
	- test-branch
- to switch to a branch, use `git checkout <branch-name>`, and the currently active branch will be indicated with `*<branch-name>` when you run `git branch` again.