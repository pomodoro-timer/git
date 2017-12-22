# git
For practicing git functions

# Contributing users
* ijklim
* pomodoro-timer

# Events

## Dec 22, 2017
* pomodoro-timer
  * Create repository on github.com, name `git`
  * Create new SSH key under Settings
  * Clone `git` to local machine
  * Create and check out new branch `ptm` (for pomodoro-timer)
  ```bash
  git clone git@github.com:pomodoro-timer/git.git git
  git checkout -b ptm
  ```
  * Update README.md
  * Commit change and upload to github
  ```bash
  git add README.md
  git commit -m 'Record actions taken to create repository'
  git fetch
  git push origin ptm
  ```
  * Look for new branch under https://github.com/pomodoro-timer/git/branches
  * Create a pull request by clicking on `New pull request`
  * Status: *This branch has no conflicts with the base branch*
  * Pull request accepted by *ijklim*
  * Check main page https://github.com/pomodoro-timer/git, README is updated
  * Repeat commands from above with a different message

* ijklim
  * Accept pull requests from *pomodoro-timer*
  * Clone `git` to local machine
  * Create and check out new branch `ijklim`
  ```bash
  git clone https://github.com/pomodoro-timer/git.git git
  git checkout -b ijklim
  ```
  * Update README.md
  * Commit change and upload to github
  ```bash
  git add README.md
  git commit -m 'Download repo from another user and record actions taken'
  git fetch
  git push origin ijklim
  ```
  * Create a pull request
  * Pull request accepted by *pomodoro-timer*
  * README is updated under the `Code` tab
  * Accept pull request from *pomodoro-timer*

* pomodoro-timer
  * Accept pull request from *ijklim*
  * Fetch changes from remote repo
  ```bash
  git fetch
  ```
  * Still in `ptm` branch, do NOT see changes reflect in README.md
  * Update files to reflect changes
  ```bash
  git merge origin/master
  ```
  * Changes from *ijklim* are now shown in README.md
  * Update README.md
  * Commit change and upload to github
  ```bash
  git add README.md
  git commit -m 'Update README after fetching changes from ijklim'
  git fetch
  git push origin ptm
  ```

* ijklim
  * Update README.md
  * Commit change and upload to github
  ```bash
  git add README.md
  git commit -m 'Attempt to upload changes without fetch after accepting pull request'
  ```
  * Some changes have been stashed, but cannot be popped without committing change