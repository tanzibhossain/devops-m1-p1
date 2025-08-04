# Module 1 Project 1 - Version Control using Git and GitHub

## Project Overview
This project demonstrates fundamental version control operations using Git and GitHub, including:

- Initializing a local Git repository
- Staging and committing changes
- Creating and switching branches
- Pushing changes to a remote repository
- Creating and merging pull requests on GitHub

## Topics Covered
- Git basics: commit, branch, merge
- Remote repositories with GitHub
- Collaboration workflow using pull requests

---

## Step-by-Step Process

### 1. Set Up a Local Git Repository
- Initialize a new Git repository locally using `git init`.
- Create a `README.md` file with an initial project description.
- Stage and commit the `README.md` file with a descriptive commit message.

### 2. Create a New GitHub Repository
- Create a new repository on GitHub.
- Link your local repository to the GitHub remote with `git remote add origin <repo-url>`.
- Push local commits to GitHub using `git push -u origin main`.

### 3. Branching
- Create a new branch called `dev` locally with `git branch dev`.
- Switch to the `dev` branch: `git checkout dev`.
- Add a new file `hello.txt` and commit the changes.

### 4. Pushing the New Branch
- Push the `dev` branch to the remote repository: `git push origin dev`.
- Verify that the `dev` branch appears on GitHub.

### 5. Create a Pull Request
- On GitHub, open a pull request to merge `dev` into `main`.
- Provide a clear description of the changes made in the pull request.

### 6. Merge the Pull Request
- Review and merge the pull request on GitHub.
- Update your local `main` branch after merging: `git checkout main` and `git pull origin main`.

---

## Submission Requirements
- The GitHub repository must be **public**.
- Include:
  - Initial commit with `README.md`.
  - A `dev` branch with changes and an open pull request.
  - A merged pull request back into the `main` branch.
- Use meaningful commit messages and branch names.
- Provide descriptive pull request summaries explaining the purpose and changes.

---


## Notes
- Follow Git best practices for commit hygiene and branch management.
- Ensure the repository structure is clear and organized.
- Practice collaborative workflows using pull requests to merge code safely.

---

Thank you for reviewing this project!