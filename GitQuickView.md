# Git QuickView

- [Pro Git book](https://git-scm.com/book/en/v2)
- [Reference](https://git-scm.com/docs)
- [Git CHEAT SHEET from GitHub](/git/github-git-cheat-sheet.pdf)

Git Overview:

- ![Git Cheetsheet](/images/git_cheatsheet.png)

## Configuration

Configure user information for all local repositories:

| Command                                            | Description                                                      |
| -------------------------------------------------- | ---------------------------------------------------------------- |
| `git config --global user.name "[name]"`           | Sets the name you want to attached to your commmit transactions  |
| `git config --global user.email "[email address]"` | Sets the email you want attached to your commit transactions     |
| `git config --global color.ui true`                | Enables helpful colorization of command line output              |
| `git config --list`                                | List all the settings Git can find at that point, `~/.gitconfig` |
| `git config <key>`, e.g. `git config core.editor`  | Check a specific key’s value                                    |

## History

Browse and inspect the evolution of project files:

| Command                                        | Description                                                          |
| ---------------------------------------------- | -------------------------------------------------------------------- |
| `git log` or `git log -<n>`                    | Lists version history for the current branch                         |
| `git log --pretty=oneline`                     | Git Basics - Viewing the Commit History                              |
| `git log --pretty=format:"%h - %an, %ar : %s"` | https://git-scm.com/book/en/v2/Git-Basics-Viewing-the-Commit-History |
| `git log --follow [file]`                      | Lists version history for a file, including renames                  |
| `git diff [first-branch]...[second-branch]`    | Shows content differences between two branches                       |
| `git show [commit]`                            | Outputs metadata and content changes of the specified commit         |

## REDO COMMITS

Erase mistakes and craft replacement history
| Command                     | Description                                                   |
| --------------------------- | ------------------------------------------------------------- |
| `git reset [commit]`        | Undoes all commits after [commit], preserving changes locally |
| `git reset HEAD~<n>`        | Undoes last n commits                                         |
| `git reset --hard [commit]` | Discards all history and changes back to the specified commit |

Using `git push -f origin <your_branch>` to push it to remote branch.
