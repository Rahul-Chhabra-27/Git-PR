### 1. Initialize a Repository (`git init`)
- This command is used to start tracking version control in your project.
- It creates a `.git` directory, which stores all Git-related configurations and history.
- After running this, your project becomes a Git repository.


### 2. Check the Status (`git status`)
- Shows the state of your working directory and staging area.
- Helps you see which files have been modified, staged, or remain untracked.
- Useful to verify what changes will be included in the next commit.


### 3. Commit Changes (`git commit -m "commit message"`)
- Saves the current state of your staged files into the project’s history.
- Each commit is assigned a unique **hash** to identify it.
- The message `"commit message"` helps document what changes were made.


### 4. Commit All Tracked Files (`git commit -a -m "commit message"`)
- Directly commits modified tracked files without using `git add`.
- Files that were already under Git's monitoring are included in the commit.
- New files still need to be added manually using `git add` before committing.


### 5. View Commit History (`git log`)
- Displays a list of all past commits.
- Shows details like author name, date, and commit message.
- Helps track changes made over time.


### 6. Stage All Changes (`git add .`)
- Moves all modified and new files into the staging area.
- This prepares them for committing in the next step.
- Only staged files will be included in the commit.


### 7. Switch to a Different Commit or Branch (`git checkout <commit-hash>`)
- Allows you to move between branches or past commits.
- Using a branch name switches to that branch.
- Using a commit hash rolls back to an earlier state in the project.

