#  Git-Exp-1

### 1. **Install Git**
First, we need to install Git on our system:
- **Windows:** Download and install Git from [git-scm.com](https://git-scm.com/).
- **Linux:** Install using the package manager. Example for Ubuntu:
  ```bash
  sudo apt-get update
  sudo apt-get install git
  ```
- **macOS:** Install using Homebrew:
  ```bash
  brew install git
  ```

### 2. **Initialize a Git Repository**
Navigate to the root directory of our project (website or software) and initialize a Git repository.
```bash
cd /path/to/your/project
git init
```
This creates a hidden `.git` folder to track our changes.

### 3. **Add Files to Staging**
We can add files that we want to track. For all files, use:
```bash
git add .
```
For a specific file:
```bash
git add filename.html
```

### 4. **Commit Changes**
Once files are staged, commit them to the repository with a meaningful message:
```bash
git commit -m "Initial commit with basic website structure"
```

### 5. **Connect to a Remote Repository**
If we want to collaborate or backup code, we can connect our local repository to a remote repository like GitHub, GitLab, or Bitbucket.
- Create a repository on GitHub.
- Then, connect our local repository:
  ```bash
  git remote add origin https://github.com/yourusername/your-repo.git
  ```

### 6. **Push Changes to Remote**
To upload our changes to the remote repository:
```bash
git push -u origin master
```

### 7. **Track Changes**
- To check the status of our repository:
  ```bash
  git status
  ```
- To see a log of all commits:
  ```bash
  git log
  ```

### 8. **Create Branches**
We can create branches to work on new features without affecting the main codebase:
```bash
git branch new-feature
git checkout new-feature
```

After completing the feature, we can merge the branch back into the master branch:
```bash
git checkout master
git merge new-feature
```

### 9. **Handle Conflicts**
When merging, there might be conflicts. Git will notify us of the conflicts, and we’ll need to manually resolve them by editing the conflicted files. After resolving:
```bash
git add .
git commit -m "Resolved merge conflict"
```

### 10. **Pull Updates**
If multiple developers are working on the project, we can pull the latest changes from the remote repository before making new changes:
```bash
git pull origin master
```

### Best Practices
- **Commit frequently** with clear messages.
- Use **branches** for new features or bug fixes.
- **Pull** changes regularly when working in a team to avoid conflicts.

Git helps maintain a clean project history and enables collaboration on websites and software. This approach is highly useful when working in teams or managing large projects.
