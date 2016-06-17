# Git Hooks

## prepare-commit-msg
This hook will try to parse a number out of the current branch name in the form of: feature/1234-my-awesome-feature.
Afterwards it will prepend a given string and this number before your commit message: CLOUDAC-1234 #yourcommit

## pre-commit
This hook will check the files to commit for the expressions "describe.only" or "it.only" and cancel your commit if it finds any. There is some more logic in it to save unstaged changes in case of aborting the commit
