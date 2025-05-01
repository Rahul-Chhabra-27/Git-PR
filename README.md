git init
Used to initialize a new Git repository in your current project folder. It creates a hidden .git directory that stores all version control information, preparing your project to track changes.

git status
Shows the current state of your working directory and staging area. It lists modified files not yet staged, files staged for commit, untracked files, and your current branch status. This helps you understand what changes need to be staged or committed next.

git commit -m "commit message"
Saves (commits) all staged changes to the local repository with a descriptive message. This creates a snapshot of your project at that point in time, allowing you to track changes over time.

git commit -a -m "commit message"
Automatically stages and commits all modified tracked files (skipping git add for those files) with a message. It does not include new untracked files, which still require git add.

git log
Displays the commit history in reverse chronological order, showing commit hashes, authors, dates, and messages. Useful for reviewing the timeline of changes made to the project.

git add .
Stages all changes (new and modified files) in the current directory and its subdirectories, except those ignored by .gitignore. Prepares these changes to be committed.

git checkout <commit-hash>
Switches your working directory to the state at a specific commit identified by its hash. This puts you in a detached HEAD state, meaning you are not on any branch and new commits won’t be saved unless you create a new branch from this state.

