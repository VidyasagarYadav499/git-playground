# Hello World! 🌏
Hi there!👋, my name is **Vidyasagar Yadav**.  
And this is the **first repository** that i have created, to embark on a journey of learning and practicing **Git** &amp; **Github** along with it's functions and features.

# Git & GitHub Workflow 📚✨🌐

## 1. Clone the Repository 💾✨🌍

To start working on a project, clone the repository from GitHub to your local machine.

```
git clone <repo-url>
```

## 2. Create a New Branch 🌳✨🔧

Before making changes, create a new branch to keep your work separate from the main branch.

```
git checkout -b <branch-name>  # Creates and switches to a new branch
git branch <branch-name>        # Creates a new branch
git checkout <branch-name>      # Switches to the newly created branch
```

Alternatively, you can use:

```
git branch -c <branch-name>     # Creates a new branch and copies the current branch's history
```

## 3. Work on Your Branch 📚🌿✨

Make your changes, then stage and commit them.

```
git add .                       # Stages all changes in the current directory
git commit -m "commit message"  # Commits the staged changes with a descriptive message
```

Use these additional commands if needed:

```
git status                      # Shows the status of the working directory
git diff                        # Shows the differences between the working directory and the index
```

## 4. Push Your Branch to Remote Repository 🌐📢✨

Push your branch to the remote repository to share your changes.

```
git push -u origin <branch-name>  # Pushes the branch and sets the upstream reference
```

## 5. Create a Pull Request on GitHub 🔧📚🌟

Go to GitHub, navigate to your repository, and create a pull request to propose your changes for review.

## 6. Review and Merge 💡🌿🔄

After the pull request is reviewed and approved, merge it into the main branch on GitHub.

## 7. Update Your Local Repository (main branch) 🌐🔧🌿

Keep your local main branch up-to-date with the remote repository.

```
git switch main                 # Switches to the main branch
git pull origin main            # Pulls the latest changes from the remote main branch
```

Alternatively, you can use:

```
git checkout main               # Switches to the main branch
git fetch origin                # Fetches changes from the remote repository
git merge origin/main           # Merges the fetched changes into the main branch
```

# Rough-Notes 📝

## Git-Commands 📖
| Command | Description |
|---|---|
| **Initialization Commands** | |
| `git init` | Initializes a new git repository by adding a `.git` folder to it. |
| `git clone [url]` | Creates a copy of an existing repository from a remote URL. |
| **Staging Commands** | |
| `git add -A` | Adds all changes (tracked and untracked) to the staging area. |
| `git add .` | Adds new/untracked files or modified files to the staging area in the current directory. |
| `git add [file]` | Adds a specific file to the staging area. |
| **Commit Commands** | |
| `git commit -m "message"` | Commits changes with a message. |
| `git commit --amend` | Adds changes to the latest commit and allows editing the commit message. |
| `git commit -a -m "message"` | Commits all tracked files with a message, skipping the staging area. |
| **Status Commands** | |
| `git status` | Displays the status of the working directory and staging area. |
| `git status -s` | Shows a short format for the status. |
| **Configuration Commands** | |
| `git config --global alias.sta "status"` | Creates a global alias for `git status`. |
| `git config --global --edit` | Opens the global Git configuration file for editing. |
| `git config --global user.name "Your Name"` | Sets the global username for commits. |
| `git config --global user.email "you@example.com"` | Sets the global email for commits. |
| **Checkout Commands** | |
| `git checkout .` | Discards all changes in the working directory (cannot be undone). |
| `git checkout [branch]` | Switches to a specified branch. |
| `git checkout -b [new-branch]` | Creates and switches to a new branch. |
| **Remote Commands** | |
| `git push origin main` | Pushes changes to the `main` branch of the remote repository. |
| `git remote -v` | Displays the URLs of the remote repositories linked to your local Git repository. |
| `git remote add [name] [url]` | Adds a new remote repository. |
| **Log Commands** | |
| `git log` | Shows the commit history. |
| `git log --all --decorate --oneline --graph` | Displays a detailed log with all commits, decorations, oneline format, and a graph view. |
| `git log -p` | Shows the commit history with the diffs of each commit. |
| **Reset and Stash Commands** | |
| `git reset HEAD` | Unstages a file without removing changes. |
| `git reset --hard` | Resets the working directory and staging area to the last commit, discarding all changes. |
| `git stash` | Stashes uncommitted changes temporarily. |
| `git stash pop` | Applies the last stashed changes. |
| **Clean Commands** | |
| `git clean -df` | Removes untracked files and directories forcefully. |
| `git clean -n` | Shows what would be removed by `git clean`. |
| **Pull and Rebase Commands** | |
| `git pull --rebase` | Pulls changes and rebases them on top of your local commits. |
| `git rebase --abort` | Aborts the rebase process. |
| `git rebase [branch]` | Rebases the current branch onto another branch. |
| **Branch Commands** | |
| `git branch -a` | Lists all branches, including remote branches. |
| `git branch -r` | Lists remote branches. |
| `git branch -d [branch]` | Deletes a local branch. |
| **Fetch Commands** | |
| `git fetch --prune` | Removes references to branches deleted from the remote. |
| `git fetch [remote]` | Fetches branches and history from a remote repository. |
| **Miscellaneous** | |
| `git tag [tagname]` | Creates a tag at the current commit. |
| `git diff` | Shows changes between commits, the working directory, and staging area. |

## Important Points ⚠

1. Suppose you create a branch, say `my-branch` and you work on this and do not commit the changes and try to switch to some other branch, say `main` you may loose the changes you made on `my-branch`. Commit your changes before switching branches!