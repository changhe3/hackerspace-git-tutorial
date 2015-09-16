Git Tutorial for Hackerspace
============================

**Terminology:**

*Forking*: make a copy of one person's repository on your own GitHub (or other git service) account

*Branching*: make a copy of the base branch (what you're currently on) into another branch and modify files as you please, not affecting the base branch

*Pull request*: sending your changes to your own repository back to the original repository that you forked from


**Handy git commands:**

`git status`

- displays the status of your local copy from git (untracked/tracked files, modified files, deleted files, etc)

`git add <filename>`

- add a change to a file to be tracked by git
- Useful modifier:
    `git add -A`
    - Add all untracked changes/files to git

`git commit -m <message>`

- commit the changes into a local commit
- for multiple line commit messages, remove the -m and message arguments
- cool trick to add new changes to your last commit is to use the `--amend` tag

`git push`

- pushes to your most recently pushed to branch, or master if that doesnt exist
- Longer form:
    `git push origin master`

`git branch <name>`

- makes a new git branch with that name

`git checkout <name>`

- switch to a previously created branch
- can save a step if you want to create a new branch and switch to it using `git checkout -b <branch name>`

Other useful commands:

`git reset` (DANGEROUS!!)

- reset commit history to a certain time (time travel!)
- number of different options (`--hard` or `--soft` or a commit SHA)
- ex. `git commit --hard HEAD`
    or
    `git commit --hard de9db22e60294b35eeb8d756897f4a5a330558a5`