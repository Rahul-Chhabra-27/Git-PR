# git init => used to initialize the git.
  git init — Initialize a Git Repository
Purpose:
git init is used to create a new Git repository in your current project folder.
What it does:
Creates a hidden .git/ directory in your project.
Starts tracking versions of your files using Git.
Prepares your folder to use Git commands like add, commit, and push.
Usage Example:
mkdir my-project
cd my-project
git init
Now my-project is a Git repository.
Result:
You're ready to start version controlling your project!


# git status ==> it shows the current status of your application.
 git status — Show the Current State of the Repository
Purpose:
git status is used to display the current status of your working directory and staging area.
What it shows:
Files that are modified but not staged.
Files that are staged and ready to be committed.
Untracked files (new files not yet added to Git).
which branch you're on and if you're ahead/behind the remote (if applicable).
Usage Example:
git status
Example Output:
On branch main
Changes not staged for commit:
  modified:   style.css
Untracked files:
  newfile.js
Result:
You can see what has changed, what needs to be staged, and what will be included in the next commit.

 
#git commit -m "commit message"
 git commit -m "commit message" — Save Changes with a Message
Purpose:
This command is used to save (commit) the staged changes to your local Git repository with a message describing what was changed.
What it does:
Creates a snapshot of your project at that point in time.
Records it in the Git history.
The -m flag lets you add a short message explaining the commit.
Usage Example:
git commit -m "Added homepage layout and CSS styles"
Result:
Your staged changes are saved with the message so you and others can understand what was done in that commit.
 

# git commit -a -m "commit message" ==> tracked to commited
 git commit -a -m "commit message" — Commit Tracked Changes Directly
Purpose:
This command automatically stages and commits all modified, already tracked files in one step, along with a commit message.
What it does:
Skips git add for tracked files.
Does not include new (untracked) files — you still need git add for those.
Saves the commit with your message.
Usage Example:
git commit -a -m "Fixed bugs in login and updated styles"
Result:
All modified tracked files are committed with the message provided


# git log ==> to show all the commits timeline.
git log — View Commit History
Purpose:
git log is used to display the list of all commits made in a Git repository, in reverse chronological order (most recent first).
What it shows:
Commit hash (ID)
Author of the commit
Date of the commit
The commit message
Usage Example:
git log
Sample Output:
commit 1a2b3c4d5e...
Author: John Doe <john@example.com>
Date:   Tue Apr 30 14:12:45 2025 +0530
Result:
You get a full timeline of commits, useful for tracking changes or debugging.


# git add . ==> add all the changes to the staged area.
git add . — Stage All Changes
Purpose:
git add . stages all modified and new files in the current directory and its subdirectories, preparing them to be committed.
What it does:
Adds all tracked and untracked (new) files that have changes to the staging area.
Excludes files listed in .gitignore.
Usage Example:
git add .
Result:
All your changes are now staged and ready for git commit.


# git checkout <commit-message>
git checkout <commit-hash> — Switch to a Specific Commit
Purpose:
This command lets you view or go back to a specific commit in your Git history using the commit's hash ID, not the message.
Correct Usage:
git checkout 1a2b3c4d
What it does:
Moves your working directory to the state it was in at that specific commit.
Puts you in a detached HEAD state — you’re not on any branch.
Important:
You can't commit new changes in this state unless you create a new branch from it:
git checkout -b new-branch-name 1a2b3c4d
 git checkout "commit message" → Invalid
 git checkout <commit hash> → Valid

# git stash ==> Temporarily save uncommitted changes
git stash —
When you're in the middle of changes and need to shift focus (like switching branches or pulling updates), git stash stores your modified tracked files in a temporary stack. Your working directory is then cleaned to the last committed state.

# git stash list ==> View all saved stashes
git stash list —
Shows a list of all stashed changes saved in your repository.
#### Sample Output
```
stash@{0}: WIP on main: 9fceb02 Add navbar and logo
stash@{1}: WIP on main: 3d1e4f5 Fix login redirect
stash@{2}: On dev: 4a3bc90 Add contact form
```

# git stash push -m <message> ==> Create a stash with a custom name
git stash push -m "feature/like" —
By default, Git automatically generates stash messages like stash@{0} : WIP on main: 9fceb02. However, using the -m (message) flag, you can provide your own description when stashing. 

# git stash pop ==> Apply and remove the most recent stash
git stash pop —
It retrieves the most recent stashed changes and applies them back to your working directory.

# git stash apply ==> Apply stashed changes without deleting them
git stash apply —
Applies the most recent stash (stash@{0}) to your working directory, but keeps it in the stash list. By default, it applies the most recent stash (stash@{0}), but you can specify another one (like stash@{1}).
