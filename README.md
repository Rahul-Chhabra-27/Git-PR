# Git Commands

## Git Init
Creates a new Git repository in your current folder. This command sets up a special hidden .git folder that will track all the changes you make to your files. After running this, your regular folder becomes a Git-enabled project where you can start saving different versions of your work. This is always the first command you use when starting with Git on a new project.

## Git Status
Shows you what's happening in your project right now. It displays which files you've changed but haven't saved to Git yet (unstaged changes), which files are ready to be committed (staged changes), and which files Git doesn't know about yet (untracked files). It also tells you which branch you're working on. Use this command often to check what's going on before you commit your changes.

## Git Add <file>
Tells Git that you want to include changes to a specific file in your next commit. This puts the file in the "staging area" - a place where changes wait before being permanently saved. For example: git add index.html would stage just that file, while git add css/styles.css would stage your stylesheet. This helps you control exactly which changes get included in each commit.

## Git Commit -m "commit message"
Saves your staged changes to Git with a note explaining what you did. This creates a permanent snapshot of your files at this point in time that you can always return to later. The -m flag lets you write a message directly in the command. Your message should clearly describe what changes you made, such as "Fixed navigation bar layout" or "Added user registration form".

## Git Commit -a -m "commit message"
A faster way to save changes to files Git is already tracking. The "-a" option automatically stages all modified files without having to use git add first. This only works for files Git already knows about - brand new files still need git add. This command is useful when you've made several changes to existing files and want to commit them all at once.

## Git Log
Shows you the history of all your commits from newest to oldest. For each commit, you can see who made it, when it happened, the unique commit ID (hash), and what message they wrote. This helps you keep track of how your project has changed over time and find specific versions you might want to return to. It's like a journal of all the saved points in your project's history.

## Git Add .
Stages all changes in your current folder and its subfolders at once. The dot (.) means "everything here." This command is useful when you want to include all your recent changes in the next commit without adding files one by one. It will stage modified files, new files, and will also recognize deleted files. Note that it respects your .gitignore file, so excluded files won't be staged.

## Git Checkout
Takes you back to see how your project looked at an earlier point in time. You need to use the unique ID (hash) of the commit you want to visit, which you can find using git log. This lets you explore your project's past versions without losing your current work. When you're in this state, you're in what's called "detached HEAD" mode - if you want to make changes from this old version, you should create a new branch first.
