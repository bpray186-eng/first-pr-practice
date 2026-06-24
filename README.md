# First PR Practice

This repository is a low-stakes place to make your first pull request.

Your job is small on purpose: add your name to `Contributors.md` in alphabetical order, open a pull request, read the diff, and wait for the maintainer to merge it. The file change is simple so you can focus on how a branch, commit, push, pull request, review, and merge fit together.

Nothing ships unseen. Copilot can help with the mechanics, but you still review the diff before you ask for a merge.

## What You Need

- A GitHub account
- VS Code
- GitHub Copilot enabled in VS Code
- The GitHub Pull Requests extension signed in to your GitHub account

## The Exercise

You will:

1. Fork this repository.
2. Open your fork in VS Code.
3. Ask Copilot Chat to create a branch and add your name to `Contributors.md`.
4. Review the diff before anything is pushed.
5. Push your branch to your fork.
6. Open a pull request back to this repository.
7. Wait for the maintainer to review and merge it.

## Use Chat To Get Set Up

Open Copilot Chat in VS Code and work one step at a time. You can use prompts like these.

### 1. Fork The Repository

Start in GitHub in your browser. Open this repository and select **Fork**.

Keep the default settings unless your instructor tells you otherwise. When the fork is created, copy the URL of your fork.

### 2. Clone Your Fork

In VS Code, open Copilot Chat and say:

```text
Clone my fork of the first PR practice repo from <paste your fork URL here>, then open it as a new folder in VS Code.
```

Copilot may ask before running Git commands or opening a folder. Read what it is asking to do, then approve it if it matches your intent.

If you prefer to drive the VS Code UI yourself, use **Clone Git Repository** from the Source Control view, paste your fork URL, choose a local folder, and open the cloned repository when VS Code asks.

### 3. Confirm You Are In The Right Repo

Ask:

```text
Confirm this is my fork of the first PR practice repo and show me the current files before changing anything.
```

You should see `README.md`, `Contributors.md`, `CONTRIBUTING.md`, and `.github/pull_request_template.md`.

### 4. Make Your Branch And Edit

Ask Copilot Chat:

```text
In this repo, add my name, <Your Name>, to Contributors.md in alphabetical order on a new branch called add-<your-name>, commit it with a clear message, and show me the diff before pushing anything.
```

Use your real name and a branch name with lowercase letters and hyphens, such as `add-jordan-lee`.

### 5. Read The Diff

Before you approve the push, check the diff.

You should see one added line in `Contributors.md`, and nothing else. Your name should be in alphabetical order.

If the name is in the wrong place, tell Copilot exactly what to fix:

```text
That is not in alphabetical order. Move my name between <name above> and <name below>, then show me the diff again.
```

### 6. Push And Open The Pull Request

When the diff is right, ask:

```text
Push this branch to my fork and open a pull request back to the original first-pr-practice repository's main branch.
```

Check the pull request before creating it:

- The base repository should be the original `Thor-DraperJr/first-pr-practice` repository.
- The base branch should be `main`.
- The compare branch should be your branch from your fork.
- The file changed should be `Contributors.md`.

### 7. Wait For Review And Merge

After you open the pull request, the maintainer will review the diff.

If the maintainer requests a change, come back to Copilot Chat and ask it to make that specific change on the same branch. When the pull request is approved and merged, your name will appear on `main` in the original repository.

## What Good Looks Like

A good pull request for this exercise:

- Adds exactly one name to `Contributors.md`
- Keeps the list in alphabetical order
- Does not edit unrelated files
- Has a clear commit message
- Targets the original repository's `main` branch
- Shows that you read the diff before asking for review

## Maintainer Notes

For live workshops, review each pull request out loud:

1. Confirm the PR targets `main` in this repository.
2. Open the diff and confirm only `Contributors.md` changed.
3. Confirm the new name is in alphabetical order.
4. Merge the pull request.
5. Delete the branch if GitHub offers the option.

The merge is part of the lesson. Participants should see that their branch did not change `main` until the review step was complete.