Task 4 - Git Version Control

Project Overview

This project demonstrates a version-controlled DevOps project using Git and GitHub. It implements a practical Git workflow with branches, meaningful commits, Pull Requests, merging, and project documentation.

Objective

The objective of this project is to manage a DevOps project using Git best practices and understand a structured GitHub workflow.

Tools Used

Git

GitHub

Visual Studio Code


Project Structure

Task-4-git-version-control/
│
├── index.html
├── README.md
├── .gitignore
│
└── docs/
    └── git-workflow.md

File Description

index.html - Simple project landing page used to demonstrate a feature change.

README.md - Project overview and Git workflow documentation.

.gitignore - Defines files and directories that should not be tracked by Git.

docs/git-workflow.md - Detailed documentation of the Git workflow used in this project.


Git Branching Strategy

The project uses three branches:

main
  ↑
dev
  ↑
feature/update-project

main

The main branch represents the stable version of the project.

dev

The dev branch is used for integrating completed development changes before they are merged into main.

feature/update-project

The feature branch was created to implement the project landing page change without directly modifying the stable branch.

Git Workflow

The following workflow was implemented:

Create Project
      ↓
Initialize Git Repository
      ↓
Initial Commit
      ↓
Create main, dev and feature branches
      ↓
Develop Feature
      ↓
Commit Changes
      ↓
Push Feature Branch to GitHub
      ↓
Pull Request: feature/update-project → dev
      ↓
Merge into dev
      ↓
Pull Request: dev → main
      ↓
Merge into main

Commits

The project includes meaningful commits to maintain a clear version history.

Initial Commit

Initial project setup

Created the initial project structure and Git repository.

Feature Commit

Add project landing page

Added the project landing page in index.html through the feature branch.

Pull Request Workflow

Pull Requests were used to merge changes between branches instead of directly merging development work into the stable branch.

Pull Request 1

feature/update-project → dev

The feature branch containing the landing page change was reviewed and merged into dev.

Pull Request 2

dev → main

The completed development changes were promoted from dev to the stable main branch.

.gitignore

The .gitignore file is included to prevent unnecessary or local files from being tracked by Git.

It helps keep the repository clean and prevents files that should remain local from being committed.

Git Commands Used

Some of the Git commands used during the project include:

git init
git status
git add .
git commit
git branch
git branch -M main
git switch -c dev
git switch -c feature/update-project
git remote add origin
git remote -v
git push
git checkout main

Final Verification

The final repository was verified using Git status and GitHub.

The final main branch was synchronized with the remote repository and the working tree was clean.

On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean

What I Learned

Through this project, I practiced:

Initializing and managing a Git repository

Creating and managing branches

Making meaningful commits

Connecting a local repository with GitHub

Pushing branches to GitHub

Creating and merging Pull Requests

Using a feature → development → main workflow

Maintaining project documentation with Markdown

Keeping the repository clean using .gitignore

Verifying the final repository state


Conclusion

This project provided practical experience with Git version control and a structured GitHub workflow. The completed workflow demonstrates how development changes can be isolated in feature branches, integrated through dev, and finally merged into the stable main branch using Pull Requests.