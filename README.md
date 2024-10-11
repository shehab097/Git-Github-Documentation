# Git Workflow Overview

###Working Directory ➡️ Staging Area ➡️ Local Repository ➡️ Remote Repository

### Test Project ➡️ git add ➡️ git commit ➡️ git push


------------

###Git Status

##### To check the state of your project files (tracked, untracked):

```bash
git status
```

- **Tracked Files:** Files that are already being tracked by Git.

- **Untracked Files: **Files that are not tracked yet (need to be added to version control).



### Git Staging

##### Move files to the staging area (prepare them for commit):

```bash
git add <file_name>  # Add specific file
git add .            # Add all changes in the directory

```


### Git Track

##### Git tracks changes or versions for every file:

- To check if a file is updated or added:

```bash
git status
```



### Git Diff

##### To view the difference between the current state of the working directory and the last commit:

```bash
git diff
```

- Shows changes that have been made but not yet staged or committed.


### Stage and Unstage

##### If you want to restore a file to the previous condition (before changes were made):

```bash
git restore <file_name>  # Restore file to its previous state
```


------------

# Moving from Staging Area to Local Repository

##### Once the files are staged, commit them to the local repository:

```bash
git commit -m "message"   # Make sure the message is short and meaningful
```

### Git Commit Status

##### To unstage files (remove them from staging area but keep changes):

```bash
git log             # Detailed log
git log --oneline   # Condensed log with one-line summaries

```

### Git Unstage

##### To unstage files (remove them from staging area but keep changes):

```bash
git reset
```

------------

# Version Control with Git

##### View the commit history in a condensed form:

```bash
git log --oneline
```

### Example

```bash
bf22a77 (HEAD -> master) one
f9636d7 Bangladesh added
43668c0 c++ updated

```

### Switching Between Commits

##### To go back to a previous commit:

```bash
git checkout <commit-id>   # Example: git checkout f9636d7
```

##### To return to the latest commit (master):

```bash
git checkout master
```


------------

# Best Practices for Commits

> **Make commits often**- Make commits often, but not too frequently. Keep your changes logically grouped.

>**Keep commit messages short** (50 characters or less).

>Use **imperative mood** in commit messages (e.g., "Add:", "Remove:").

### Commit with Details

```bash
git commit -m "description" -m "additional details if needed"
```

------------

# Undoing Commits

### Soft Reset (Undo last commit but keep changes)
```bash
git reset --soft <commit-id>
```

### Hard Reset (Undo commits and discard changes)

```bash
git reset --hard <commit-id>
```

### Git Revert (Undo changes but keep commit history)

```bash
git revert <commit-id>
```

------------

>This documentation outlines the main Git commands, how to manage files, and best practices for version control in your project.







