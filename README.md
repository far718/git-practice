# Practice repository to start learning Git

## Commands used

- git init: create a new git repository
- git status: compare working directory, staging area, and current branch
- git add: add changes from working directory to staging area
- git commit: commit changes from staging area to current branch
- git config: set or get configuration
- git log: show a history (aka "log") of project commits
- git checkout "branch name": checkout (switch to) a branch (Update HEAD and apply changes to the working directory)
- git branch -c "branch name": create a branch
- git merge: merge changes from different branches

## Commit messages

- default editor is vim (this can be changed)
- `i` to enter *insert* mode
- type commit message
- `Esc` -> `:wq` -> `Enter` to write message and quit
or use `git commit -m "<message>"`z
- First line should be clear, accurate, and concise
- use proper, spelling, grammar and punctuation
- don't end with a `.`

For more advice, see: https://chris.beams.io/posts/git-commit/

## Merging

Merging means to bring the changes from one branch into another branch

- Fast-merging happens when the target branch was branched from the current one, and there are no new changes to the current branch since then.

- An automatic merge happens when two histories have diverged, but git is able to reconcile them into one set of changes. This creates a new commit in current branch.  
