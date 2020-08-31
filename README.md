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
