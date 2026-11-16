# 01. Git & GitHub Fundamentals

**Module:** 01  
**Level:** Beginner  
**Topics:** 9  
**Status:** Learning content completed  
**Repository:** [GitHub-learning](https://github.com/nikhil-patel-ai/GitHub-learning)

---

## Module Overview

This module introduces version control, Git, GitHub, repositories, and the GitHub website. It builds the foundation needed to manage code, track changes, and collaborate using Git and GitHub.

## Learning Objectives

By the end of this module, you should be able to:

- Explain version control and why developers use it.
- Describe Git and GitHub and distinguish between them.
- Explain the benefits of version control.
- Understand repositories, commits, branches, and remotes.
- Distinguish local repositories from remote repositories.
- Navigate the main areas of a GitHub repository.
- Understand GitHub profiles and basic account security.
- Follow a basic workflow for synchronizing local work with GitHub.

## Topic Roadmap and Notebook Links

Complete the notebooks in order.

| No. | Topic | Notebook |
|---:|---|---|
| 01 | Introduction to Version Control | [01_introduction_to_version_control.ipynb](01_introduction_to_version_control.ipynb) |
| 02 | What is Git? | [02_what_is_git.ipynb](02_what_is_git.ipynb) |
| 03 | What is GitHub? | [03_what_is_github.ipynb](03_what_is_github.ipynb) |
| 04 | Git vs GitHub | [04_git_vs_github.ipynb](04_git_vs_github.ipynb) |
| 05 | Why Developers Use Git | [05_why_developers_use_git.ipynb](05_why_developers_use_git.ipynb) |
| 06 | Understanding Repositories | [06_understanding_repositories.ipynb](06_understanding_repositories.ipynb) |
| 07 | Local vs Remote Repositories | [07_local_vs_remote_repositories.ipynb](07_local_vs_remote_repositories.ipynb) |
| 08 | GitHub Interface Overview | [08_github_interface_overview.ipynb](08_github_interface_overview.ipynb) |
| 09 | GitHub Profile and Account Setup | [09_github_profile_and_account_setup.ipynb](09_github_profile_and_account_setup.ipynb) |

## Key Concepts and Terminology

| Term | Meaning |
|---|---|
| Version control | A system for tracking changes to files over time. |
| Git | A distributed version control system. |
| GitHub | A platform for hosting Git repositories and collaborating. |
| Repository (repo) | A project location that stores files and their history. |
| Local repository | A Git repository stored on your computer. |
| Remote repository | A Git repository hosted elsewhere, such as GitHub. |
| Commit | A recorded snapshot of repository changes. |
| Branch | An independent line of development. |
| Clone | Downloading a repository and its history to your computer. |
| Push | Sending local commits to a remote repository. |
| Fetch | Downloading remote updates without integrating them into the current branch. |
| Pull | Fetching remote changes and integrating them into the current branch. |
| Origin | A common default name for a remote repository. |
| Pull request | A proposal to review and merge changes between branches. |
| Issue | A place to track bugs, questions, and work. |
| GitHub Actions | GitHub's workflow automation feature. |
| README | A document that explains a project or folder. |
| 2FA | Two-factor authentication; an additional account verification step. |

## Basic Git Workflow

A common beginner workflow is:

```text
Working directory
      |
      | git add
      v
Staging area
      |
      | git commit
      v
Local repository
      |
      | git push
      v
Remote repository (GitHub)
```

Useful commands introduced in this module:

```bash
git status
git add <file>
git commit -m "Describe your change"
git remote -v
git branch -r
git fetch origin
git pull --rebase origin main
git push origin main
```

Run Git commands from inside your local repository folder. Replace `<file>` and the commit message with the relevant values for your work.

## Practical Module Exercises

Use your learning repository to practise these tasks:

- [x] Identify the purpose of version control.
- [x] Explain the difference between Git and GitHub in your own words.
- [x] Identify a repository, commit, and branch.
- [x] Explain local and remote repositories.
- [x] Inspect the configured remote using `git remote -v`.
- [x] Inspect remote branches using `git branch -r`.
- [x] Explore the Code, Issues, Pull requests, Actions, and Settings areas on GitHub.
- [x] Open your GitHub profile and review the information you choose to make public.
- [x] Locate your contribution graph and pinned repositories.
- [x] Review the available account security settings.

## Practice Completion Record

Update this record based on work you have actually completed. Do not mark an activity complete just because you have read about it.

| No. | Topic / Activity | Status | Notes |
|---:|---|---|---|
| 01 | Introduction to Version Control | Completed | Notebook uploaded and verified |
| 02 | What is Git? | Completed | Notebook uploaded and verified |
| 03 | What is GitHub? | Completed | Notebook uploaded and verified |
| 04 | Git vs GitHub | Completed | Notebook uploaded and verified |
| 05 | Why Developers Use Git | Completed | Notebook uploaded and verified |
| 06 | Understanding Repositories | Completed | Notebook uploaded and verified |
| 07 | Local vs Remote Repositories | Completed | Notebook uploaded and verified |
| 08 | GitHub Interface Overview | Completed | Notebook uploaded and verified |
| 09 | GitHub Profile and Account Setup | Completed | Notebook uploaded and verified |
| 10 | Practical module exercises | Update your status | Complete the checklist above |
| 11 | Module revision and self-assessment | Update your status | Use the revision section below |

## Sticky Notes – Quick Revision

- **Version control** tracks changes and helps recover earlier work.
- **Git** is the version control tool; **GitHub** hosts Git repositories and supports collaboration.
- A **repository** contains project files and their version history.
- A **commit** records a set of changes.
- A **branch** provides a separate line of development.
- A **local repository** is on your computer; a **remote repository** is hosted elsewhere.
- `git add` stages changes; `git commit` records them locally; `git push` sends commits to a remote.
- `git fetch` downloads remote updates; `git pull` downloads and integrates them.
- `origin` is a common name for the remote repository.
- **Issues** track work; **pull requests** propose changes for review; **Actions** automates workflows.
- A profile README repository must have the same name as your GitHub username.
- Protect your account with a strong unique password and 2FA. Never publish passwords, API keys, or tokens.

## Common Troubleshooting

### `fatal: not a git repository`

You are probably running the command outside your repository.

```powershell
cd "C:\Users\Nikhil\NVSCode\02_Git_&_GitHub"
```

Then run the Git command again.

### `error: remote origin already exists`

The remote is already configured. Inspect it instead of adding it again:

```bash
git remote -v
```

### `! [rejected] main -> main (non-fast-forward)`

The remote branch contains commits that your local branch does not yet include. First integrate the remote changes, then push:

```bash
git pull --rebase origin main
git push origin main
```

If Git reports a conflict, stop and resolve it carefully before continuing. Do not use force push as a routine fix.

### `LF will be replaced by CRLF`

This is a line-ending warning commonly seen on Windows. By itself, it is not a failed commit or push.

## Interview Questions

1. What is version control, and why is it useful?
2. What is Git?
3. What is GitHub?
4. Explain the difference between Git and GitHub.
5. What is a repository?
6. What is the difference between a local and remote repository?
7. What is a commit?
8. What is a branch?
9. Explain `git add`, `git commit`, and `git push`.
10. What is the difference between `git fetch` and `git pull`?
11. What is the purpose of a pull request?
12. What are GitHub Issues and GitHub Actions?
13. What is a profile README?
14. Why should you enable two-factor authentication?

## Knowledge Check

Try answering without looking at the notebooks.

1. Which tool is the distributed version control system: Git or GitHub?
2. Where is a local repository stored?
3. Which command records staged changes in the local repository?
4. Which command sends local commits to a remote repository?
5. Which command downloads remote updates without integrating them?
6. What is the usual name of the default remote?
7. Which GitHub feature is used to propose changes for review?
8. Which GitHub feature can automate tests and deployments?
9. What should the profile README repository be named?
10. What does 2FA add to account security?

### Answer Key

1. Git.
2. On your computer.
3. `git commit`.
4. `git push`.
5. `git fetch`.
6. `origin`.
7. Pull request.
8. GitHub Actions.
9. Exactly the same as your GitHub username.
10. An additional verification step beyond the password.

## Revision and Self-Assessment

Before moving to the next module, check each statement:

- [x] I can explain version control in simple words.
- [x] I can distinguish Git from GitHub.
- [x] I understand repositories, commits, and branches.
- [x] I can explain local versus remote repositories.
- [x] I understand the basic add–commit–push workflow.
- [x] I know the difference between fetch and pull.
- [x] I can navigate a GitHub repository page.
- [x] I understand Issues, Pull requests, and Actions.
- [x] I know the purpose of a GitHub profile README.
- [x] I understand basic GitHub account security.

**My self-assessment:** Beginner / Developing / Confident

**Topics I should revise:** _Write topic numbers or concepts here._

**Questions I still have:** _Write your questions here._

## Module Completion Checklist

- [x] All 9 topic notebooks studied.
- [x] All practical exercises completed.
- [x] Knowledge-check questions attempted.
- [x] Incorrect answers revised.
- [x] Interview questions reviewed.
- [x] Sticky notes revised.
- [x] Self-assessment completed.

## Module Summary

In this module, you learned the foundations of version control, Git, and GitHub. You explored repositories, local and remote workflows, the GitHub interface, and your GitHub profile. These concepts prepare you for practical Git commands and repository configuration in the next module.

**Next module:** 02 – Git Installation and Configuration.

---

*Learning note: Keep this README as the module-level guide and progress tracker. Use each topic notebook for its detailed explanations, examples, exercises, troubleshooting, and topic-specific revision.*
