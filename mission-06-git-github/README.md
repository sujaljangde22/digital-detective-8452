# Mission 6 — Git and GitHub

## Task / Objective

Practise staging and committing changes, publish a branch to GitHub, and open a pull request.

## Work Completed

I checked the repository status, staged the Mission 5 README update, committed it, and checked the recent commit history. I created the `update-about` branch and added a **My Learning** section to the root `README.md`. After pushing the branch, I opened [pull request #1](https://github.com/sujaljangde22/digital-detective-8452/pull/1) into `main`.

## Commands / Tools Used

| Command | What it does |
|---|---|
| `git init` | Initializes a Git repository in the current folder. |
| `git status` | Shows the current branch and which changes are staged, unstaged, or untracked. |
| `git add <file>` | Stages the current contents of a specific file for the next commit. |
| `git commit -m "message"` | Records the staged changes in the local repository with a message. |
| `git log --oneline` | Shows a compact list of commits. |
| `git branch` | Lists local branches. |
| `git switch -c update-about` | Creates the branch and switches to it. |
| `git switch main` | Switches back to the `main` branch. |
| `git push -u origin update-about` | Publishes the branch and links it to its remote counterpart. |
| `git pull` | Retrieves and integrates changes from the remote branch. |

## My Understanding

Staging selects what goes into the next commit. Committing records that selection in the repository’s history. A branch lets me make changes independently of `main`. A pull request shows those changes and gives people a place to review and discuss them before merging.

## Difficulties Faced

My first commit attempt returned `nothing to commit` because Git did not see any saved changes to the root README.

## How I Resolved Them

I edited and saved the root README, then staged and committed the change on `update-about`.

## Evidence / Files

- The root `README.md` contains the **My Learning** section on `update-about`.
- [Pull request #1](https://github.com/sujaljangde22/digital-detective-8452/pull/1) shows the proposed change to `main`.

## Commit Details

- Push status: Verified on GitHub (commit `609f529`).
- Pull request #1: Open from `update-about` into `main`. Not merged.