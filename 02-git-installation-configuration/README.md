# 02. Git Installation and Configuration

## 1. Module Overview
This module covers installing Git on Windows and configuring Git so it can be used reliably from terminals and development tools.

## 2. Learning Objectives
After completing this module, you will be able to:
- Install Git for Windows and verify the installation.
- Understand Git Bash and Git command-line access.
- Configure your Git username and email.
- Distinguish global and local Git configuration.
- Inspect and manage Git settings.

## 3. Topic Roadmap

| No. | Topic | Notebook |
|---|---|---|
| 01 | Installing Git on Windows | [01_installing_git_on_windows.ipynb](01_installing_git_on_windows.ipynb) |
| 02 | Verifying Git Installation | [02_verifying_git_installation.ipynb](02_verifying_git_installation.ipynb) |
| 03 | Understanding Git Bash and Git CLI | [03_understanding_git_bash_and_git_cli.ipynb](03_understanding_git_bash_and_git_cli.ipynb) |
| 04 | Configuring Username and Email | [04_configuring_username_and_email.ipynb](04_configuring_username_and_email.ipynb) |
| 05 | Git Global vs Local Configuration | [05_git_global_vs_local_configuration.ipynb](05_git_global_vs_local_configuration.ipynb) |
| 06 | Checking and Managing Git Settings | `06_checking_and_managing_git_settings.ipynb` |

## 4. Key Concepts and Terminology
- **Git for Windows:** The Windows distribution of Git command-line tools.
- **Git Bash:** A Bash-like terminal environment included with Git for Windows.
- **PATH:** A Windows environment variable that helps terminals locate executable programs.
- **Git configuration:** Settings that control Git behavior, including user identity.
- **Global configuration:** Settings generally applied to the current Windows user.
- **Local configuration:** Settings stored for a specific repository and taking precedence over global settings for that repository.

## 5. Basic Git Configuration Workflow
The module will cover these commands:

```bash
git --version
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
git config --list
```

Use your own name and email when practising. Do not copy the example identity literally.

## 6. Practical Module Exercises
1. Install Git for Windows if it is not already installed.
2. Verify that Git is available from PowerShell and Git Bash.
3. Inspect the Git executable location.
4. Configure a Git username and email.
5. Compare global and repository-local configuration.
6. Inspect the effective Git configuration.

## 7. Practice Completion Record
Record your actual commands, outputs, and observations in the relevant topic notebooks. Clearly distinguish your actual output from illustrative expected output.

## 8. Sticky Notes – Quick Revision
- Install Git for Windows from the official Git website.
- Reopen terminals after installation or PATH changes.
- Git Bash and PowerShell are different terminal environments; both can run Git.
- Git identity is configured with `git config`.
- Local repository settings take precedence over global settings for that repository.

## 9. Common Troubleshooting
### `git` is not recognized
Reopen the terminal and verify that Git for Windows is installed and available on PATH.

### Git uses an unexpected username or email
Inspect configuration with `git config --list` and check whether a local setting overrides the global setting.

### A configuration value appears more than once
Use `git config --show-origin --list` to inspect where settings are defined.

## 10. Interview Questions
1. What is Git for Windows?
2. What is Git Bash?
3. What is the purpose of PATH?
4. What is the difference between global and local Git configuration?
5. Which command displays Git configuration?
6. Why might a repository use a different Git email from the global email?

## 11. Knowledge Check
1. Which command checks the installed Git version?
2. Which command sets the global username?
3. Which configuration scope applies only to one repository?
4. Which command helps identify the source file for a configuration setting?

## 12. Answer Key
1. `git --version`
2. `git config --global user.name "Your Name"`
3. Local configuration.
4. `git config --show-origin --list`

## 13. Revision and Self-Assessment
Before completing this module, make sure you can:
- Verify Git installation from a terminal.
- Explain Git Bash and command-line access.
- Set and inspect Git identity.
- Explain global and local configuration precedence.

## 14. Module Completion Checklist
- [x] Topic 01 – Installing Git on Windows
- [x] Topic 02 – Verifying Git Installation
- [x] Topic 03 – Understanding Git Bash and Git CLI
- [x] Topic 04 – Configuring Username and Email
- [x] Topic 05 – Git Global vs Local Configuration
- [ ] Topic 06 – Checking and Managing Git Settings

## 15. Module Summary
This module establishes a working Git installation and the configuration needed to use Git consistently. Complete the topics in order and record practical results in the notebooks. The next module covers repository management.
