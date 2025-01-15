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
| **Initialization Commands** |  |
| `git init` | Initializes a new git repository by adding a `.git` folder to it. |
| `git clone ` | Creates a copy of an existing repository from a remote URL. |
| **Staging Commands** |  |
| `git add -A` | Adds all changes (tracked and untracked) to the staging area. |
| `git add .` | Adds new/untracked files or modified files to the staging area in the current directory. |
| `git add ` | Adds a specific file to the staging area. |
| **Commit Commands** |  |
| `git commit -m "message"` | Commits changes with a message. |
| `git commit --amend` | Adds changes to the latest commit and allows editing the commit message. |
| `git commit -a -m "message"` | Commits all tracked files with a message, skipping the staging area. |
| **Status Commands** |  |
| `git status` | Displays the status of the working directory and staging area. |
| `git status -s` | Shows a short format for the status. |
| **Push Commands** |  |
| `git push` | Pushes changes from the local repository to the remote repository's default branch. |
| `git push ` | Pushes changes to the specified remote repository's default branch. |
| `git push  ` | Pushes the specified branch to the specified remote repository. |
| `git push --force` | Forces the push by overwriting the remote branch history with local history. |
| `git push --all` | Pushes all local branches to the specified remote repository. |
| `git push --tags` | Pushes all tags to the remote repository. |
| `git push --set-upstream  ` | Sets the remote branch as the upstream branch for the local branch and pushes to it. |
| `git push origin main` | Pushes changes to the `main` branch of the remote repository. |
| `git push --force` | Overwrites the remote history. |
| **Fetch Commands** |  |
| `git fetch` | Downloads all branches, tags, and commits from the default remote repository `origin` but does not update the local branches automatically. |
| `git fetch ` | Fetches data (branches, history,. etc) from a specified remote repository. For example, `git fetch origin` retrieves changes from the `origin` remote. |
| `git fetch  ` | Fetches updates from a specific branch of the remote repository. Example: `git fetch origin main` Fetches the latest updates from the `main` branch of the `origin` remote. |
| `git fetch --all` | Fetches updates from all configured remotes. |
| `git fetch --prune` | Removes references to branches deleted from the remote. |
| `git fetch --dry-run` | Simulates the fetch process and shows what would be updated without actually fetching the data. |
| **Pull Commands** |  |
| `git pull` | Fetches and merges changes from the default remote and branch into the current branch. |
| `git pull ` | Pulls updates from a specified remote repository into the current branch. |
| `git pull  ` | Pulls changes from a specific branch of the remote repository into the current branch. |
| `git pull --rebase` | Fetches changes from the remote and rebases the local branch on top of the remote branch. |
| `git pull --strategy=` | Uses a specific merge strategy when pulling changes. |
| `git pull --dry-run` | Simulates the pull process without making any changes. |
| **Checkout Commands** |  |
| `git checkout ` | Switches to the specified branch. |
| `git checkout -b ` | Creates a new branch and switches to it. |
| `git checkout ` | Checks out a specific commit, detaching the HEAD. |
| `git checkout ` | Restores a specific file from the last commit or the index. |
| **Branch Commands** |  |
| `git branch` | Lists all local branches. |
| `git branch ` | Creates a new branch with the specified name. |
| `git branch -d ` | Deletes the specified branch. |
| `git branch -m  ` | Renames the specified branch. |
| `git branch -r` | Lists all remote branches. |
| `git branch -a` or `--all` | Lists all branches, including remote branches. |
| **Configuration Commands** |  |
| `git config --global alias.sta "status"` | Creates a global alias for `git status`. |
| `git config --global --edit` | Opens the global Git configuration file for editing. |
| `git config --global user.name "Your Name"` | Sets the global username for commits. |
| `git config --global user.email "you@example.com"` | Sets the global email for commits. |
| **Remote Commands** |  |
| `git remote` | Lists all the remote repositories configured for the current repository. |
| `git remote -v` | Lists all the remote repositories with their URLs. |
| `git remote add <name> <url>` | Adds a new remote repository with the specified name and URL. |
| `git remote remove <name>` | Removes the specified remote repository. |
| `git remote rename <old> <new>` | Renames a remote repository from `` to ``. |
| `git remote show <name>` | Displays detailed information about the specified remote repository. |
| `git remote set-url <name> <url>` | Changes the URL of a remote repository. |
| **Log Commands** |  |
| `git log` | Shows the commit history. |
| `git log --all --decorate --oneline --graph` | Displays a detailed log with all commits, decorations, oneline format, and a graph view. |
| `git log -p` | Shows the commit history with the diffs of each commit. |
| **Reset Commands** |  |
| `git reset HEAD` | Unstages a file without removing changes. |
| `git reset --hard` | Resets the working directory and staging area to the last commit, discarding all changes. |
| **Stash Commands** |  |
| `git stash` | Stashes uncommitted changes temporarily. |
| `git stash pop` | Applies the last stashed changes. |
| **Clean Commands** |  |
| `git clean -df` | Removes untracked files and directories forcefully. |
| `git clean -n` | Shows what would be removed by `git clean`. |
| **Rebase Commands** |  |
| `git rebase ` | Rebases the current branch on top of the specified branch. |
| `git rebase /` | Rebases the current branch on top of a remote branch. |
| `git rebase --onto   ` | Rebases the specified branch onto a new base, applying only commits that are not in the upstream. |
| `git rebase --continue` | Continues the rebase process after resolving conflicts. |
| `git rebase --abort` | Aborts the rebase process and returns to the state before rebase started. |
| `git rebase --skip` | Skips the current patch during a rebase if conflicts arise. |
| `git rebase --interactive` | Starts an interactive rebase session allowing you to edit, squash, or reorder commits. |
| **Miscellaneous** |  |
| `git tag ` | Creates a tag at the current commit. |
| `git diff` | Shows changes between commits, the working directory, and staging area. |

## Interactive Rebase 🌵

Interactive Rebase is a tool for optimizing and cleaning up your commit history. It's like a swiss-army knife for git operations.
It can help peform various operations:
 - Change a commit's message.
 - Delete commits.
 - Reorder commits,
 - Squash: Combine multiple commits into one.
 - Edit/split an existing commit into mutliple new ones.

> ⚠️ **Warning:** Do NOT use Interactive Rebase on commits that you have already pushed/shared on a remote repository! Instead, use it to clean your local commit history before merging it into a shared team branch. Remember this mantra, **NEVER REBASE PUSHED COMMITS!**

### Workflow 🍃༄
#### Step 1: Determine the Base Commit
1. **How far do you want to go?**
   - Decide which commit you want to start from, at least the ancestor or parent of the commit you want to change.

2. **Choose the Base Commit**:
   - Use `git log` or `git log --oneline` to find the appropriate commit hash or relative reference.
   
     ```
     git log --oneline
     ```

#### Step 2: Start the Interactive Rebase
1. **Run the Command**:
   - Start the interactive rebase with one of the following commands:

     ```
     git rebase --interactive HEAD~3
     ```
     OR
     ```
     git rebase -i HEAD~3
     ```
     OR
     ```
     git rebase -i <hash>
     ```

#### Step 3: Choose Actions in the Editor
1. **Editor Opens**:
   - A text editor will open, listing commits from the base commit to the HEAD.
   
2. **Determine Actions**:
   - For each commit, specify the action to perform:
     - `pick`: Use the commit as is (default).
     - `reword`: Change the commit message.
     - `edit`: Amend the commit content.
     - `squash`: Combine this commit with the previous one, merging messages.
     - `fixup`: Combine with the previous commit, discarding this commit's message.
     - `drop`: Remove the commit entirely.

3. **Example**:
   ```
   pick abc123 Commit message 1
   reword def456 Commit message 2
   edit ghi789 Commit message 3
   ```

4. **Save and Close**:
   - Save the file and close the editor to proceed.

#### Step 4: Execute Actions
1. **Reword Commit Messages**:
   - If `reword` was chosen, Git will prompt you to edit the commit message. Update the message, save, and close.

2. **Edit Commit Content**:
   - If `edit` was chosen, Git will pause the rebase. Make your changes, stage them, and amend the commit:
     
     ```
     git add <file>
     git commit --amend
     ```
   - Continue the rebase:
     
     ```
     git rebase --continue
     ```

3. **Resolve Conflicts** (if any):
   - If conflicts arise, resolve them manually, then stage the resolved files:
     
     ```
     git add <file>
     ```
   - Continue the rebase:
     
     ```
     git rebase --continue
     ```
   - To abort the rebase if needed:
     
     ```
     git rebase --abort
     ```

#### Step 5: Finalize and Verify
1. **Completion**:
   - Once all commits are processed, the rebase completes successfully.
     
2. **Review History**:
   - Check the updated commit history to ensure everything is as expected:
     
     ```
     git log --oneline
     ```

#### Additional Tips:
- **Backup Branch**: Before rebasing, create a backup branch for safety:
  
  ```
  git branch backup-branch
  ```
  
- **Rebase Shared History**: Be cautious when rebasing commits that have been shared with others. Coordinate with your team to avoid issues.

## Important Points ⚠

1. Suppose you create a branch, say `my-branch` and you work on this and do not commit the changes and try to switch to some other branch, say `main` you may loose the changes you made on `my-branch`. Commit your changes before switching branches!
