# <span style="color:orange"> GitHub Commands Cheatsheet for Team Collaboration </span>

### <span style="color:blue"> Feel free to use this cheatsheet as a quick reference for your team's collaboration on GitHub. </span>

#### <span style="color:orange"> **Setup and Configuration** </span>
- **Clone a repository**: `git clone <repository-url>`
  - Example: `git clone https://github.com/username/repo.git`
- **Configure user name**: `git config --global user.name "Your Name"`
  - Example: `git config --global user.name "Jane Doe"`
- **Configure email**: `git config --global user.email "your.email@example.com"`
  - Example: `git config --global user.email "jane.doe@example.com"`

#### <span style="color:orange"> **Branching and Merging** </span>
- **Create a new branch**: `git checkout -b <branch-name>`
  - Example: `git checkout -b feature/new-feature`
- **Switch to a branch**: `git checkout <branch-name>`
  - Example: `git checkout main`
- **List all branches**: `git branch`
  - Example: `git branch`
- **Merge a branch into the current branch**: `git merge <branch-name>`
  - Example: `git merge feature/new-feature`
- **Delete a branch**: `git branch -d <branch-name>`
  - Example: `git branch -d feature/old-feature`

#### <span style="color:orange"> **Committing Changes** </span>
- **Check status of changes**: `git status`
  - Example: `git status`
- **Stage changes**: `git add <file-name>` or `git add .` (to stage all changes)
  - Example: `git add index.html` or `git add .`
- **Commit changes**: `git commit -m "Commit message"`
  - Example: `git commit -m "Add new feature"`
- **Amend the last commit**: `git commit --amend -m "New commit message"`
  - Example: `git commit --amend -m "Update feature implementation"`

#### <span style="color:orange"> **Collaborating** </span>
- **Pull latest changes from remote**: `git pull origin <branch-name>`
  - Example: `git pull origin main`
- **Push changes to remote**: `git push origin <branch-name>`
  - Example: `git push origin feature/new-feature`
- **Fetch changes from remote**: `git fetch origin`
  - Example: `git fetch origin`
- **Rebase your branch with the latest changes**: `git rebase origin/<branch-name>`
  - Example: `git rebase origin/main`

#### <span style="color:orange"> **Resolving Conflicts** </span>
- **View conflicts**: `git status`
  - Example: `git status`
- **Resolve conflicts in files**: Manually edit the files to resolve conflicts
  - Example: Open `index.html` and resolve the conflicts
- **Mark conflicts as resolved**: `git add <file-name>`
  - Example: `git add index.html`
- **Continue rebase after resolving conflicts**: `git rebase --continue`
  - Example: `git rebase --continue`
- **Abort rebase**: `git rebase --abort`
  - Example: `git rebase --abort`

#### <span style="color:orange"> **Review and Collaboration Tools** </span>
- **Create a pull request**: Go to the repository on GitHub and click "New pull request"
  - Example: Navigate to your repository on GitHub and click "New pull request"
- **Review a pull request**: Go to the pull request on GitHub, add comments, and approve or request changes
  - Example: Open the pull request on GitHub, add comments, and click "Approve" or "Request changes"
- **Merge a pull request**: Click "Merge pull request" on GitHub
  - Example: Click "Merge pull request" on the pull request page on GitHub

#### <span style="color:orange"> **Miscellaneous** </span>
- **View commit history**: `git log`
  - Example: `git log`
- **View a specific commit**: `git show <commit-hash>`
  - Example: `git show 1a2b3c4d`
- **Stash changes**: `git stash`
  - Example: `git stash`
- **Apply stashed changes**: `git stash apply`
  - Example: `git stash apply`
