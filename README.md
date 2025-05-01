**Git Commands for managing repositories**


# git init => used to initialize a new git repo in the current directory.
-> git folder has been created as soon as git init command executed.
-> initializes and controls processes.

# git status ==> it shows the current status of your application like which files are modified,staged,etc.
-> It let you see which changes have been staged, which haven't and which files aren't being tracked ny Git.
-> Status output doesn't show you any information regarding the commited project history.

# git commit -m "commit message" ==> Commits staged changes to local repo with a message.
-> Commit the changes.
-> View the commit.

# git commit -a -m "commit message" ==> tracked to commited
-> Git commit without staged
-> It will automatically stage every changed, already tracked file.

# git add . ==> add all the changes to the staged area.
-> It tells Git that you want to include updates to a particular file in the next commit.
-> It doesn't really affect the repository in any significant way.(changes are not actually recorded untill you run git commit)
# git checkout <commit-message>
-> Navigate between the brances creatd by Git branch.
-> It tells Git to record all new commits on that branch.

# git push ==> Pushes committed changes to the remote repository.
# git pull: Fetches and merges changes from the remote repository to your local working directory.
# git merge ==> Merges changes from the specified branch into the current branch.
# git diff ==> Shows the differences between your working directory and the index (staged changes).
# git log ==> Shows the commit history of the repository.
# git fetch: Downloads objects and refs from another repository (without merging).
# 

