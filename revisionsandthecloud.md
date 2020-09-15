# Class 2: Revisions in the Cloud

**Git:** Git is a version control system that:
- allows multiple developers work on the same code
- shows the history of changes to the code
- lets you view, apply and remove changes
- keeps all project files on one repository
- makes collaboration easier
- tracks changes applied
### Stages of Tracking
- **Committed:** Data is securely stored in a local database
- **Modified:** File has been changed but not committed to the database
- **Staged:** Flagged a file’s changed version to be committed in the next snapshot

- Tracked files can be modified, unmodified, or staged; they were part of the most recent file snapshot.
- Untracked files were not in the last snapshot and do not currently reside in the staging area.
 
**GitHub** uses Git under the hood and you can import and export repositories from GitHub to your local device and vise versa.

### Importing
- switch to target project's directory using **cd** command
- use git init command 
- to start tracking these repository files, preform an intial commit.

### Cloning
-use the git clone command to clone existing repositories into the local device. Cloning copies all versions of all files of a project.

### Anatomy of a Local Repository
- **Working Directory:** Where the actual files live.
- **Index:** Area used for staging.
- **Head:** The most recent commit.

### Add, Commit, Push
- **Track (Add) one file:** git add filename
-**Track (Add) all files:** git add *
- use git status in between steps to check status of file
- **Commit a file:** git commit -m (-m denotes a commit message, they are important for keeping track of your changes)
- **Commit all files:** git commit -a
- **Push to remote Repo:** git push origin master
- you can stash changes without commiting them by using git stash command.
 
