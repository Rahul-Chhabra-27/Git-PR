##  Basic Git Commands

### Repository Setup
- `git init`  
  Initializes a new Git repository in the current directory.

- `git clone <repo_url>`  
  Clones a repository from a remote URL to your local machine.

---

###  Staging & Committing
- `git status`  
  Displays the state of the working directory and staging area.

- `git add <file>`  
  Stages the specified file for commit.

- `git add .`  
  Stages all changed files in the current directory.

- `git commit -m "message"`  
  Commits staged changes with a message.

---

###  Syncing with Remote
- `git push`  
  Pushes committed changes to the remote repository.

- `git pull`  
  Fetches and merges changes from the remote repository.

- `git fetch`  
  Downloads objects and refs from the remote repository (without merging).

- `git merge <branch_name>`  
  Merges changes from the specified branch into the current branch.

---

### Review & History
- `git log`  
  Shows the commit history.

- `git diff`  
  Shows the difference between files in working directory and staging area.
