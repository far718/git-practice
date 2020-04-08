# Practice repository to start learning Git

## Commands used

- git init: create a repository
- git status: compare working directory, staging area, and current branch
- git add: add changes from working directory to staging area
- git commit: commit changes from staging area to current branch
- git config: set or get configuration
- git log: show history of project commits
- git branch: list branches
- git checkout: check out a branch (Update HEAD)
- git checkout -b "branch name": create branch, and then check it out


## What is a branch?

A branch is a ref(erence) to commit. When Head points to a branch, we say we are 'on' that branch. When we make a commit when we are on that branch, the branch is updated to refer to the new commit.

## What is HEAD?

HEAD is a ref(erence) to the "current" branch (or sometimes a commit.... more on that later). Git commands like `status`, `log`, and `branch` use HEAD. `git checkout` updates HEAD to ref(er) to a different branch.

## Commit messages

- default editor is vim (this can be changed)
- `i` to enter *insert* mode
- type commit message
- `Esc` -> `:wq` -> `Enter` to write message and quit
or use `git commit -m "<message>"`

- First line should be clear, accurate, and concise
- use proper, spelling, grammar and punctuation
- don't end with a `.`

For more advice, see: https://chris.beams.io/posts/git-commit/
