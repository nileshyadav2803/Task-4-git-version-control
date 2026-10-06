Git Workflow Documentation

1. Repository Initialization

The project repository was initialized locally using Git.

git init
git add .
git commit -m "Initial project setup"
git branch -M main

2. Branching Strategy

The following branches were used:

main — final stable version

dev — development/integration branch

feature/update-project — feature development branch


3. Feature Development

A feature branch was created from the development branch:

git switch -c feature/update-project

The project landing page was added/updated in index.html.

The changes were committed using:

git add index.html
git commit -m "Add project landing page"

4. GitHub Remote

The local repository was connected to GitHub and the required branches were pushed.

git push -u origin feature/update-project
git push -u origin dev
git push -u origin main

5. Pull Request: Feature → Dev

A Pull Request was created from:

feature/update-project → dev

The Pull Request was reviewed and merged into the dev branch.

6. Pull Request: Dev → Main

After completing the development changes, a second Pull Request was created:

dev → main

The Pull Request was merged into main.

7. Final Verification

The local repository was switched to the main branch and verified.

git checkout main
git status

The working tree was clean and the local main branch was synchronized with origin/main.

8. Git Tag

The final stable project version is tagged as:

v1.0.0

The tag is used to identify the final version of the project.

9. Workflow Summary

Local Project
     ↓
git init
     ↓
Initial Commit
     ↓
main → dev
     ↓
feature/update-project
     ↓
Feature Commit
     ↓
Pull Request
     ↓
feature → dev
     ↓
Pull Request
     ↓
dev → main
     ↓
Final Verification
     ↓
v1.0.0 Tag

10. Key Git Practices Used

Meaningful commit messages

Separate development and feature branches

Pull Requests for merging

.gitignore for unnecessary files

Git tags for version identification

Markdown documentation

Final repository verification