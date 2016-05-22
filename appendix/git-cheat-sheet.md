# Git Cheat Sheet

**HEAD** - The currently active Branch on *your* local repository. Whether on Branch ```master```, ```slave```, or ```poodle```, the HEAD is the state of your file-set frozen at the point of the most recent Commit. Resetting to ```HEAD``` will simply undo all changes that have not been committed.

## Common Git Commands

### Configuration
> This must be done when first initializing Git and will probably require reference should you ever need it again....





### Create a New, Local Repository
| Task  | Command   |
| :---: | :---: |
| Clone an existing repository  | ``` git clone https://github.com/ACCDrupal-2016Fall/resources.git ``` |



#### Create a completely new repository
```
git init
```
> **Note** - I think I have used ```git init``` three or four times **total** since truly learning Git. Most times it is not only more efficient, but also *easier* to let the companies hosting online repositories do the work of configuring remotes, adding access, etc. Instead, simply create a new repository via github.com/ and use ```git clone```.

### Tracking, Adding, and Committing *Local* Changes

#### Review file changes within a repository
```
git status
```
> Note, you must be at or below the root of the Git repository.

#### Add all changes in all edited files to the next commit
```
git add .
    OR
git add *
```

#### Commit Local Changes
```
All Changes:
git commit -a -m "<add text here>"

Previously Staged Changes (using git add):
git commit -m "<add text here>"
```
> The ```-m``` tag is rarely included in most instructions, but should always be included because Git requires comments for every commit made.

### Applying Changes To / From Server

#### Applying Changes *From* Server (Pulling)
Fetch Changes to Local Repository
```
git fetch <remote> <branch>

Example:
git fetch origin master
git fetch GitHub 7.x-0.x
```
Apply Fetched Changes to Local Repository
```

```

> **Note** - Often, ```git fetch``` is unnecessary, but can sometimes be required when attempting to pull in a *different* Branch from the Server and apply it to the current HEAD.



#### Applying Changes *To* Server (Pushing)

## Further Reading
 * [Git-Tower = Git Cheat Sheet](https://www.git-tower.com/blog/git-cheat-sheet/ "Git-Tower = Git Cheat Sheet")
 * [GitHub = Git Cheat Sheet](https://services.github.com/kit/downloads/github-git-cheat-sheet.pdf "GitHub = Git Cheat Sheet")
 * [Atlassian = Git Cheat Sheet](https://www.atlassian.com/dms/wac/images/.../git/atlassian_git_cheatsheet.pdf "Atlassian = Git Cheat Sheet")  
