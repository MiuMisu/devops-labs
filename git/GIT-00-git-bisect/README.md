# GIT-00 - Git Bisect

## Objective 

Learn how to use git bisect to identify the commit that introduced a bug.

## Enviroment

- OS; Ubuntu Linux
- VCS: Git
- Shell: Bash

## Task 

Create a test repository with several commits, introduce an intentional bug, and use Git Bisect to find the first commit containing the bug.

## Repository Initialization

Created a temp. rep. for the experiment to avoid modifying the main lab rep

    mkdir -p /tmp/git-bisect-lab
    cd /tmp/git-bisect-lab
    git init -b main

### Commands:

| Command | Description |
|---------|-------------|
| mkdir -p | Creates the directory, including parent dir. if necesary.|
| cd | Changes the current working dir.|
| git init -b main | Init a new Git rep and sets its initial branch name to main.|

## Git Bisect Commands

| Command | Description |
|---------|-------------|
| git bisect start | Start the bisect session |
| git bisect good | Mark the current commit as good |
| git bisect bad | Mark the current commit as bad |
| git bisect good <commit> | Mark a specific commit as good |
| git bisect bad <commit> | Mark a specific commit as bad |
| git bisect reset | End the bisect session and return to the original position |

Git Bisect uses binary search to narrow down the range of commits and identify the first commit that introduced a bug.

## Practical Work

1. Initialized a temp. Git rep.
2. Created a Bash script that classifies numbers.
3. Added input validation and separate handling for zero.
4. Created several commits to build project histroty.
5. Introduced an intentional bug. 
6. Started a Git Bisect session.
7. Marked the initial commit as good and the current commit as bad.
8. Tested intermediate commits and marked.
9. Identified the first bad commit.
10. Used **git bisect reset** to return to the orig. branch position.

## Result

Git Bisect successfully identified the first commit that introduced the bug.

## Key Takeaways

- Git Bisect doesn't rewrite ot delete commit history.
- During the process, Git may entered a detached HEAD state.

## Conclusion

Successfully completed a practical exercise in identifying a faulty commit using Git Bisect.


