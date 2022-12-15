# gitconfig
Various useful aliases for using the git cli

# Aliases
- `git ac "my commit message"`
  - Adds the changed files and commits them with the specified message
- `git publish`
  - Gets the current local branch's name and publishes it to origin under the same name
  ```
  # Usage:
  
  $ git checkout -b my-new-branch
  $ git publish
  -> Branch 'my-new-branch' set up to track remote branch 'my-new-branch' from 'origin'. 
  ```
- `git squash-template`
  - Rebases the branch (`main` should be checked out) back to the root commit
  - Allows you to `pick` the first commit and `squash` the rest into it
  - Useful for when a using a repository as a template, pushing cleanup commits to it (like readme, naming, config, etc), and then resetting the repository to start with those changes as the initial commit
