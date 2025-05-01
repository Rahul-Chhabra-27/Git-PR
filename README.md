Git : 

Git, Global Information Tracker, is a free, open-source distributed version control system used to track changes in software development projects. It allows developers to create branches, merge changes, and track the history of modifications, making it a powerful tool for managing code and collaborating on projects. 


Key Features of Git : 

Branching: Allows developers to create separate versions of a project for different features or experiments.
Merging: Allows developers to integrate changes from different branches.
Commit: Records snapshots of changes to the project, providing a timeline of development. 
Staging: A temporary area where developers can prepare changes before committing them.


Files in Git go through a cycle:

   Working Directory → Staging Area → Repository


Lets understand the git a bit more : 

1. Initialize Git on a folder, Git now creates a hidden folder to keep track of changes in that folder (.git).
   
2. If the folder contains a file before the git is initialized, then git is not aware of it and cannot be able to track it.
    Example : If a.txt is created before the git is initialized, then this a.txt will be in " untracked area ".
   
3. If we want git to know about our file, then we should add it. When the file is added it moves to the " staged area" .
   
4. If the file is in staged area it is ready for the commit, or else we can make modificatiions. If the file is modified, 
   then the newly added or modified content is highlighted by the git. It keeps track of it. At this process the file will be 
   in " tracked area " . We can add the file again to staged area to commit the changes.

5. Once the file is commited, all the changes and content of it are recorded or saved.

Things to remember :

1. A file cannot be committed if it is in untracked area.
2. We can commit it from staged area.
3. We can  commit a file from tracked area by 2 ways 
   ---> by adding to staged area and then commit
   ---> by directly committing from tracked area


Git Commands : 

To do the above mentioned actions, we require commands. The following are the most popular and frequently used commands.

1. git init -- > Initializes a new Git repository in your current directory. It is the first command you run to create a new Git repository. It sets up all the necessary files and directories Git needs to start tracking changes in your project. This includes creating a hidden .git/ folder in your directory, which contains all the metadata, configurations, and version history.

You can use it to initialize both:
   --> Empty repositories (starting a new project)
   --> Existing projects (if you’ve already written some code and now want to start tracking it with Git)
Syntax : 

   # Starting a new project with Git:
       mkdir blog-website
       cd blog-website
       git init
       
   # Adding Git to an existing project:
       cd existing_project
       git init
       
2. git add -- > git add is used to stage changes (Moving to staged area) in your working directory, preparing them to be 
   included in the next commit. It tells Git which files or changes you want to track and save. These can include new files, 
   modified files, or deletions. However, git add does not actually save the changes permanently — it just moves them to the 
   staging area, awaiting a git commit.

Syntax :  

   # Add a specific file:
        git add a.txt

   # Add all files and changes in the current directory:
        git add .


 3. git status -- > The git status command displays the current state of the working directory and the staging area. It 
    shows which files have been modified, added, deleted, or are still untracked. This helps you understand what changes are 
    staged for the next commit, what changes are not staged, and which files are not being tracked by Git at all.

Syntax : 
       
        git status


4. git commit -- > git commit is used to save the staged changes (from git add) into the Git repository. Each commit creates 
   a unique snapshot of your project at a specific point in time, along with a message describing the changes made. Commits 
   form the building blocks of your project history.

Syntax :

      git commit -m "Your commit message"

  # If you only want to commit changes to files already being tracked (not new files), you can skip git add with:

     git commit -a -m "Your commit message"             # (from trcked area to commit )


5. git log -- > The git log command shows the commit history for the current branch. It lists all commits, starting with the 
   most recent, and displays information like commit ID, author, date, and the commit message. This allows you to review the 
   history of changes made in the repository.

Syntax :
      
       git log
       git log --oneline                 # Shows a simplified, one-line log per commit
       git log --graph                   # Visual representation of the commit history
    
6. git checkout <commit message>  -- > git checkout is used for several purposes:

      Switching branches: You can use git checkout to switch between branches in your repository.

      Creating a new branch: By adding the -b flag, you can create a new branch and switch to it immediately.

      Discarding changes in files: If you’ve made changes in a file and want to revert it to the last committed state, git 
      checkout <file> will discard those changes.

    Syntax:

       git checkout <branch-name>      # Switch to an existing branch
       git checkout -b <new-branch>    # Create a new branch and switch to it
       git checkout <file>             # Discard changes in a file (restore to last commit)
       git checkout -- <file>          # Same as above, used to discard changes in the working directory


