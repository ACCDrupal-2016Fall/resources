# Git Cheat Sheet

**HEAD** - The currently active Branch on *your* local repository. Whether on Branch ```master```, ```slave```, or ```poodle```, the HEAD is the state of your file-set frozen at the point of the most recent Commit. Resetting to ```HEAD``` will simply undo all changes that have not been committed.

**Remote** - This is the non-local 'copy' of your files. Typically this is GitHub, though other Remote locations can be added.

**Local** - This is your local 'copy' of your files. Typically this is a directory on your computer where Git Bash is opened to, for tracking changes.

## Common Git Commands

### Configuration
> This must be done when first initializing Git and will probably require reference should you ever need it again....

| Task  | Command   |
| :--- | :--- |
| **Configuring the Local machine**  |  |
| Define the author name for all commits by current user  | ``` git config --global user.name <name> ``` |
| Define the author email for all commits by current user  | ``` git config --global user.email <name> ``` |
| Set the Text Editor to be used when commands require text editing  | ``` git config --system core.editor atom.exe ``` |
| Open the global configuration file for editing (if you got something wrong)  | ``` git config --global --edit ``` |
| **Configuring Remotes**  |  |
| View Remotes  | ```git remote -v``` |
| Add a Remote  | ```git remote add <local-name-for-remote> <remote-url>``` |
| Delete a Remote  | ```git remote rm <local-name-for-remote>``` |

> **Note** - Not adding ```--global``` to the command will mean the Author information is only applied locally. This is useful if you are using someone else's login to make changes, though rarely recommended.


### Create a New, Local Repository
| Task  | Command   |
| :--- | :--- |
| Clone an existing repository  | ``` git clone https://github.com/ACCDrupal-2016Fall/resources.git ``` |
| Create a completely new repository  | ```git init```  |

> **Note** - I think I have used ```git init``` three or four times **total** since truly learning Git. Most times it is not only more efficient, but also *easier* to let the companies hosting online repositories do the work of configuring remotes, adding access, etc. Instead, simply create a new repository via github.com/ and use ```git clone```.

### Branching
| Task  | Command   |
| :--- | :--- |
| View All Branches  | ``` git branch -av ``` |
| Switch to a Branch  | ``` git checkout <branch-new> ``` |
| Add a New Branch  | ```git branch <new-branch-name>```  |
| Checkout a Branch  | ```git checkout <branch-name>```  |
| Delete a Local Branch  | ```git -d <branch-name>```  |
| Delete a Local **Unmerged** Branch  | ```git -D <branch-name>```  |

> **Note** - Branching is covered by basics and in relation to usage with Pantheon.io's MultiDev environment primarily within this course. Students are encouraged to explore the power of Git Branches beyond the scope of the course as they are the foundation of the Git VCS.
> For example, a useful trick to creating a Branch and switching to it is to simply use the command ```git checkout -b <new-branch-name>```.

### Tracking, Adding, and Committing *Local* Changes
| Task  | Command   |
| :--- | :--- |
| Review file changes within a repository  | ``` git status ``` |
| Add all changes in all edited files to the next commit  | ```git add . OR git add *```  |
| **Commit Local Changes**  |   |
| All Changes  | ```git commit -a -m "<add text here>"```  |
| Previously Staged Changes  | ```git commit -m "<add text here>"```  |
> Note, you must be at or below the root of the Git repository.

> The ```-m``` tag is rarely included in most instructions, but should always be included because Git requires comments for every commit made.

### Resetting Changes
| Task  | Command   |
| :--- | :--- |
| Unstage all Staged changes since last commit  | ``` git reset ``` |
| Unstage all Staged changes and revert files to last commit  | ```git reset --HARD```  |


### Applying Changes To / From Server

| Task  | Nickname  | Command   |
| :--- | :--- | :--- |
| Adding Remote changes to Local Repository  | **Fetching**  | ``` git fetch <remote> <branch> ``` |
| Applying Remote changes to Local Repository   | **Pulling**  | ```git pull <remote> <branch>```  |
| Apply Local changes to Remote Repository   | **Pushing**  | ```git push <remote> <branch>```  |

**Example - Pulling:**
```
git fetch origin master
git pull origin master

git fetch GitHub 7.x-0.x
git pull GitHub 7.x-0.x
```
> **Note** - Often, ```git fetch``` is unnecessary, but can sometimes be required when attempting to pull in a *different* Branch from the Server and apply it to the current HEAD.

> **Second Note** - Sometimes (often, on large teams) ```git pull``` simply does not work. Instead, ```git merge``` is required. Merging is out of scope for this course, however, because the focus is local development. See below for additional references, if interested.

**Example - Pushing:**
```
git push origin master

git push GitHub 7.x-0.x
```

## Further Reading
 * [Git-Tower = Git Cheat Sheet](https://www.git-tower.com/blog/git-cheat-sheet/ "Git-Tower = Git Cheat Sheet")
 * [GitHub = Git Cheat Sheet](https://services.github.com/kit/downloads/github-git-cheat-sheet.pdf "GitHub = Git Cheat Sheet")
 * [Atlassian = Git Cheat Sheet](https://www.atlassian.com/dms/wac/images/.../git/atlassian_git_cheatsheet.pdf "Atlassian = Git Cheat Sheet")  
