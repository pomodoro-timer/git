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