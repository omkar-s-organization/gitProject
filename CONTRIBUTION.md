# Contributing Guidelines

## Quick Start

1. Open an issue before starting work.
2. Use branch names like: `feature/xyz` or `fix/bug-name`.
3. PRs must link the issue and be clearly explained.

## How to Contribute: From Issue to Pull Request 🚀

Hey there! If you landed on the Issues page and want to contribute, this guide walks you through every step — whether it's your first time or you're already familiar with forks and branches.

### Step 1: Finding or Creating an Issue

- Look for an existing issue related to what you want to work on.
- If one exists, comment to let others know you're working on it.
- If not, create a new issue with a clear title and description:
  - What you plan to do and why it's needed.

### Step 2: Preparing Your Local Repo

If you're new to this repo:
- Fork the repo by clicking the "Fork" button at the top-right.
- Clone your fork locally:
  ```bash
  git clone https://github.com/<your-username>/<repo-name>.git
  cd <repo-name>
  ```
- Add the original repo as an upstream remote:
  ```bash
  git remote add upstream https://github.com/<upstream-owner>/<repo-name>.git
  ```

If you already have a fork:
- Make sure your local main is up to date:
  ```bash
  git checkout main
  git fetch upstream
  git merge upstream/main
  git push origin main
  ```

### Step 3: Start Your Work on a Branch

- Create a new branch for your issue:
  ```bash
  git checkout -b feature/your-issue-name
  ```
- Work on your changes locally.

### Step 4: Commit Your Changes

- Stage and commit with a message referencing the issue:
  ```bash
  git add .
  git commit -m "feat: your description (closes #issue-number)"
  ```

### Step 5: Push and Open a Pull Request (PR)

- Push your branch:
  ```bash
  git push origin feature/your-issue-name
  ```
- On GitHub, go to your fork and click "Compare & pull request."
- Make sure your PR:
  - Targets the main branch of the original repo (upstream)
  - Has a clear title and description
  - Includes `Closes #issue-number` to auto-close the issue on merge

### Step 6: After Your PR is Merged

- Sync your local and fork main branch:
  ```bash
  git checkout main
  git fetch upstream
  git merge upstream/main
  git push origin main
  ```
- Delete your feature branch locally and remotely:
  ```bash
  git branch -d feature/your-issue-name
  git push origin --delete feature/your-issue-name
  ```

## Extra Tips for a Smooth Contribution Flow

- Always keep your fork synced to avoid conflicts.
- Make commit messages descriptive and reference issue number.
- Don't work directly on main — always branch out.
- Before submitting a PR, double-check your changes locally.
- Respect the issue thread: communicate clearly if you take it or need help.

Thanks for contributing and helping make this project awesome! 🙌

Happy coding! 💻🔥