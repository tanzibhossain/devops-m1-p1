# Module 1 Project 1 - Version Control using Git and GitHub

## Project Overview
This project demonstrates fundamental version control operations using Git and GitHub, including:

- Initializing a local Git repository
- Staging and committing changes
- Creating and switching branches
- Pushing changes to a remote repository
- Creating and merging pull requests on GitHub
- **Automating tasks with GitHub Actions**

## Topics Covered
- Git basics: commit, branch, merge
- Remote repositories with GitHub
- Collaboration workflow using pull requests
- **CI/CD basics using GitHub Actions**

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

# Module 2 Project_2

You have a `hello.txt` file in your existing Git repository from your previous assignment. Create a GitHub Actions workflow to read and output the content of this file to the workflow's log when code is pushed to the `main` branch.

## Steps

1. **Verify Existing Repository**  
   Ensure you have a GitHub repository with a `hello.txt` file in the `main` branch.

2. **Create Workflow File**  
   Create a GitHub Actions workflow file in the `.github/workflows` directory, setting the trigger for pushes to `main`.

3. **Checkout Code**  
   Add a step to checkout the repository's code.

4. **Read and Output**  
   Add a step to read the `hello.txt` file and print its content to the workflow's log.

5. **Push and Observe**  
   Push your workflow file and observe the workflow's execution in GitHub Actions.

### Example Workflow File

```yaml
name: Read hello.txt

on:
  push:
    branches:
      - main

jobs:
  read-file:
    runs-on: ubuntu-latest
    steps:
      - name: Checkout repository
        uses: actions/checkout@v3

      - name: Read hello.txt
        run: cat hello.txt
