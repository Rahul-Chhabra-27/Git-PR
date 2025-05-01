git init ⇒ Used to initialize the Git repository.git init is used to create a new Git repository in your current project folder.
Creates a hidden .git/ directory in your project. Starts tracking versions of your files using Git. Prepares your folder to use Git commands like add, commit, and push.

git status ⇒ Displays your application's current state.git status is employed to indicate the current state of your working directory and staging area.
It indicates Modified files that aren't staged. Files that are staged and can be committed. Untracked files. Which branch you're currently on and whether you're ahead/behind the remote .

git commit -m "commit message" ⇒ Save changes with a message.This command is employed to save (commit) the staged changes to your local Git repository with a message about what was changed.It takes a snapshot of your project at the moment. Commits it to the Git history. The -m flag allows you to include a brief description of what the commit did.

git commit -a -m "commit message" ⇒ Committed tracked files directly.This command stages and commits all existing modified, already tracked files at once, together with a commit message.It skips the need for git add for tracked files. Doesn't include new (untracked) files — still use git add for them. Saves the commit with your message.

git log ⇒ Displays all the commit history.git log is used to print the list of all commits done in a Git repository, in reverse chronological order (most recent first).It commit hash (ID), Commit Author, Commit Date, and the Commit message.

git add. ⇒ Add all the changes to the staged area.
It stages all new and modified files in the present directory and subdirectories, making them ready for committing.It Stages all tracked and untracked (new) files with changes in the staging area. Ignores files specified in .gitignore.

git checkout ⇒ Switch to a particular commit or branch. This command allows you to view or revert to a particular commit in your Git history with the hash ID of the commit, or switch between branches.It use git checkout with a branch name to switch branches, or with a commit hash to view an older state.
