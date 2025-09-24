# gitconfig
Various useful aliases for using the git cli

# Aliases
- `git ac "my commit message"`
  - Adds the changed files and commits them with the specified message
  
- `git del-file-log src/full-path/some-file-name.ext`
  - Shows the commit log for a deleted file in the repository
  - This is useful for finding a commit / PR a file was deleted in
  - It can be used with `git del-file-path` to find the full path(s) the file lived in while it was used
  
- `git del-file-path some-file-name.ext`
  - Shows the full path(s) a deleted file lived in while it was used
  
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
 
- `git clean-all`
  - Removes all files and folders in .gitignore
  - Useful for removing all build artifacts
