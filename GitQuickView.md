# Git QuickView

- [Pro Git book](https://git-scm.com/book/en/v2)
- [Reference](https://git-scm.com/docs)
- [Git CHEAT SHEET from GitHub](/git/github-git-cheat-sheet.pdf)

Git Overview:

- ![Git Cheetsheet](/images/git_cheatsheet.png)

## Configuration

Configure user information for all local repositories:

| Command                                            | Description                                                     |
| -------------------------------------------------- | --------------------------------------------------------------- |
| `git config --global user.name "[name]"`           | Sets the name you want to attached to your commmit transactions |
| `git config --global user.email "[email address]"` | Sets the email you want attached to your commit transactions    |
| `git config --global color.ui true`                | Enables helpful colorization of command line output             |

## History

Browse and inspect the evolution of project files:

| Command                                     | Description                                                  |
| ------------------------------------------- | ------------------------------------------------------------ |
| `git log`                                   | Lists version history for the current branch                 |
| `git log --follow [file]`                   | Lists version history for a file, including renames          |
| `git diff [first-branch]...[second-branch]` | Shows content differences between two branches               |
| `git show [commit]`                         | Outputs metadata and content changes of the specified commit |

## REDO COMMITS

Erase mistakes and craft replacement history
| Command                     | Description                                                   |
| --------------------------- | ------------------------------------------------------------- |
| `git reset [commit]`        | Undoes all commits after [commit], preserving changes locally |
| `git reset --hard [commit]` | Discards all history and changes back to the specified commit |