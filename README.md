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
- git checkout -b "branch name": create branch, and then check it out
- git branch: list branches
- git stash: stash/store changes from working directory
- git stash list: list stashes
- got stash pop: apply stashed changes to working directory
- git show: show a single commit
- git diff: show the difference between commits, the working directories, and the staging area
- git merge: merge changes from different branches
- git remote add <remote> <url>: add new <remote> at <url>
- git remote -v: list remote repositories
- git push -u <remote> <branch>: push <branch> to <remote>, and set default upstream for <branch>

## What is a branch?

A branch is a ref(erence) to commit. When Head points to a branch, we say we are 'on' that branch. When we make a commit when we are on that branch, the branch is updated to refer to the new commit.

## What is HEAD?

HEAD is a ref(erence) to the "current" branch (or sometimes a commit.... more on that later). Git commands like `status`, `log`, and `branch` use HEAD. `git checkout` updates HEAD to ref(er) to a different branch.

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
