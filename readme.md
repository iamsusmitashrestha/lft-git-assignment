## 1. Can we have a global .gitignore ?

Yes, we can have a global `.gitignore` file that applies to all of the Git repositories on the computer.

---

## 2. How to find difference between two commits?

To find the difference between two commits in Git, we can use the `git diff` command followed by the commit hashes or references for the two commits we want to compare.

Here's an example command to find the difference between two commits:  
`git diff <commit-hash-1> <commit-hash-2>`

---

## 3. Write difference between git add and git commit commands.

`git add`: This command adds changes to the staging area, also known as the index. When we make changes to our project files, those changes are not immediately committed to the Git repository. Instead, we need to add the changes to the staging area using the `git add` command.

`git commit`: This command creates a new commit in the Git repository with the changes that have been added to the staging area using `git add`.

---

## 4. How to unstage files?

We can unstage files by using this command:  
`git reset <filename>`

---

## 5. How to revert a commit?

To revert a commit in Git, you can use the git revert command. This command creates a new commit that undoes the changes made in the previous commit. Here are the steps:

- First, identify the commit you want to revert. You can use the git log command to view the commit history and find the commit hash.

- Once you have identified the commit, use the git revert command followed by the commit hash. For example:  
  `git revert abc123`

---

## 6. Difference between revert and reset.

`git revert`: This command creates a new commit that undoes the changes made in a specific commit. When we use git revert, Git creates a new commit that contains the opposite of the changes made in the specified commit. This means that the changes are still present in the Git history, but they are undone in a new commit. `git revert` is useful when we want to undo changes that have already been pushed to a remote repository, or when we want to keep a record of the changes that were undone.

`git reset`: This command allows us to undo changes by resetting our Git repository to a previous commit. When we use `git reset`, Git erases the changes made in one or more commits, and sets the Git repository back to a previous state. `git reset` is useful when we want to undo changes that have not yet been pushed to a remote repository, or when we want to remove unwanted changes from the Git history entirely.

---
