# Git Advanced Commands

We'll explore advanced Git commands that can help you streamline your workflow, manage complex scenarios, and improve your version control skills.

## Table of Contents

1. [Interactive Rebase](#interactive-rebase)
2. [Cherry-Pick](#cherry-pick)
3. [Stash](#stash)
4. [Reflog](#reflog)
5. [Bisect](#bisect)

## Interactive Rebase

Interactive rebase is a powerful tool for rewriting your commit history. Here's how to use it:

1. **Start an interactive rebase:** Use the following command to start an interactive rebase for the last N commits, where N is the number of commits you want to include:

   ```bash
   git rebase -i HEAD~N
   ```

2. **Edit commits:** In the interactive rebase interface, you can choose to reword, edit, squash, or split commits as needed.

3. **Complete the rebase:** Save and exit the text editor to finish the interactive rebase.

Interactive rebase is useful for cleaning up your commit history, squashing multiple commits into one, and organizing your changes logically.

## Cherry-Pick

Cherry-picking allows you to apply specific commits from one branch to another:

1. **Find the commit you want to cherry-pick:** Identify the commit hash you want to apply.

2. **Switch to the target branch:** Ensure you are on the branch where you want to apply the commit.

3. **Cherry-pick the commit:** Use the following command, replacing `<commit-hash>` with the actual commit hash:

   ```bash
   git cherry-pick <commit-hash>
   ```

This is handy for applying specific fixes or features from one branch to another without merging the entire branch.

## Stash

The stash command lets you temporarily save your changes and switch to another branch:

1. **Stash your changes:** Use the following command to stash your uncommitted changes:

   ```bash
   git stash
   ```

2. **Switch to another branch:** After stashing, you can switch to another branch to work on different tasks.

3. **Apply the stash:** When you return to your original branch, you can apply the stash using:

   ```bash
   git stash apply
   ```

Stashing is helpful when you need to switch context quickly without committing half-finished work.

## Reflog

The reflog is a useful history of your branch references, which can help you recover lost commits or branches:

1. **View the reflog:** Use the following command to see the reflog:

   ```bash
   git reflog
   ```

2. **Recover lost commits:** You can identify lost commits in the reflog and use checkout or branch commands to recover them.

The reflog is a safety net when you accidentally delete branches or commits.

## Bisect

Git bisect is a tool to help you find the specific commit that introduced a bug in your code:

1. **Start the bisect process:** Use the following commands to begin the bisect process:

   ```bash
   git bisect start
   git bisect bad <bad-commit>
   git bisect good <good-commit>
   ```

2. **Test specific commits:** Git will guide you through testing different commits, marking them as "good" or "bad."

3. **Identify the faulty commit:** After testing, Git will pinpoint the exact commit where the bug was introduced.

Git bisect is a valuable tool for debugging and identifying the source of issues in your code.
