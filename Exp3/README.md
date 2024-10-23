### 1. **Create a New Branch**

First, ensure you're on the branch from which you want to create a new branch, usually `main` or `master`. You can check your current branch using:

```bash
git branch
```

To create and switch to a new branch:

```bash
git checkout -b feature-branch
```

This creates a new branch named `feature-branch` and switches to it.

Alternatively, you can also use:

```bash
git branch feature-branch  # Creates the branch
git checkout feature-branch # Switches to the branch
```

### 2. **Make Changes in the Branch**

Now that you're on the `feature-branch`, make changes to your web application code as needed.

After making the changes, add them to the staging area:

```bash
git add .
```

Commit your changes:

```bash
git commit -m "Describe your changes"
```

### 3. **Push the Branch to Remote Repository**

If you are working with a remote repository (like GitHub, GitLab, etc.), push the branch to the remote:

```bash
git push origin feature-branch
```

### 4. **Switching Between Branches**

To switch back to another branch (e.g., `main`):

```bash
git checkout main
```

### 5. **Merging the Branch**

Once you've completed the work on your branch and you're ready to merge it into the `main` branch, follow these steps:

- First, switch back to the `main` branch:

```bash
git checkout main
```

- Pull the latest changes:

```bash
git pull origin main
```

- Merge your feature branch into `main`:

```bash
git merge feature-branch
```

- After merging, you can push the updated `main` branch to the remote:

```bash
git push origin main
```

### 6. **Delete the Feature Branch (Optional)**

Once the branch is merged and no longer needed, you can delete it locally:

```bash
git branch -d feature-branch
```

To delete it from the remote repository:

```bash
git push origin --delete feature-branch
```

### Summary of Git Commands:

1. **Create and Switch to a Branch**: `git checkout -b feature-branch`
2. **Commit Changes**: `git add .` and `git commit -m "message"`
3. **Push Branch to Remote**: `git push origin feature-branch`
4. **Merge Branch**: `git checkout main` then `git merge feature-branch`
5. **Delete Branch**: `git branch -d feature-branch`

This approach keeps the main codebase clean and ensures smooth collaboration in team-based projects.
