# Git and GitHub Cheat Sheets

This collection of cheat sheets provides quick references for common Git and GitHub operations. Whether you're a beginner looking to grasp essential commands or an experienced user in need of a quick reminder, these cheat sheets will help you work more efficiently and effectively with version control and collaboration.

## Git Cheat Sheet

### Configurations

- Configure Git: `git config --global user.name "Your Name"` and `git config --global user.email "youremail@example.com"`
- Set a default text editor: `git config --global core.editor "editor_name"`
- View current configurations: `git config --list`

### Basic Commands

- Initialize a Git repository: `git init`
- Clone a remote repository: `git clone <repository_url>`
- Check status: `git status`
- Add changes to the staging area: `git add <file>`
- Commit changes: `git commit -m "Commit message"`
- View commit history: `git log`

### Branching

- Create a new branch: `git branch <branch_name>`
- Switch to a branch: `git checkout <branch_name>`
- Merge branches: `git merge <branch_name>`
- Delete a branch: `git branch -d <branch_name>`

### Remote Repositories

- Add a remote repository: `git remote add <remote_name> <repository_url>`
- Push changes to a remote repository: `git push <remote_name> <branch_name>`
- Pull changes from a remote repository: `git pull`

## GitHub Cheat Sheet

### Repository Operations

- Create a new repository: Click the "+" button on GitHub and choose "New repository."
- Fork a repository: Click "Fork" on the top right of a repository's page.
- Clone a repository: `git clone <repository_url>`

### Collaborative Work

- Create a branch: `git checkout -b <branch_name>`
- Create a pull request: From your branch, click "New Pull Request."
- Review and merge pull requests: Collaborate on changes effectively.
- Resolve merge conflicts: Address conflicts during pull request reviews.

### GitHub Actions

- Create a GitHub Actions workflow: Define a `.github/workflows` YAML file.
- Set up continuous integration: Automate testing and build processes.
- Deploy with GitHub Actions: Automate deployment pipelines.

## Markdown Cheat Sheet

- Create headings: `# Header 1`, `## Header 2`, ...
- Create lists: `- Item 1`, `- Item 2`, ...
- Add links: `[Text](URL)`
- Insert images: `![Alt text](URL)`

## Advanced Git Commands

- Rebase instead of merge: `git rebase <branch_name>`
- Cherry-pick specific commits: `git cherry-pick <commit_hash>`
- Amend the last commit: `git commit --amend`
- Use Git hooks for custom actions.

- Create tables:
  ```markdown
  | Header 1 | Header 2 |
  |----------|----------|
  | Content 1| Content 2|
  ```
## Additional Resources

In addition to the cheat sheets, explore these resources for further learning:

- [Pro Git Book](https://git-scm.com/book/en/v2) - A comprehensive guide to Git.
- [GitHub Learning Lab](https://learn.microsoft.com/training/github/?WT.mc_id=%3Fwt.mc_id%3Dstudentamb_260352) - Interactive courses on Git and GitHub.
- [A Guided Tour of GitHub](https://github.com/skills/introduction-to-github) - In-depth tutorials on Git concepts.

### Acknowledgment

We acknowledge and thank the wider open-source community for their valuable contributions and the creation of these cheat sheets.
