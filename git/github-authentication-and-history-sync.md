

# GitHub Authentication and History Sync

## 1. Problem 
    Git requested a login and a token after each push. The goal to cofigure GitHub auth. so that a token did not need to entered manually every time.

## 2. GitHub CLI Authetication 
### 2.1 Install GithHub CLI 
        sudo apt update 
        sudo apt install gh
### 2.2 Login
        gh auth login --hostname github.com --git-protocol https (Entered by a web browser in an other machine) 
Authenticates GitHub CLI with GitHub.com and selects HTTPS for Git operaitions 
### 2.3 Configure Git
        gh auth setup-git
Configures Git to Use GitHub CLI for retrieving auth credentials 
## 3. Checking Repo Status 
        git status -sb
Displays a short status (-s), including the current branch (-b) and its relationship with the tracked remote branch. 
## 4. Synchronizing History
        git pull --rebase
Fetches remote changes and replays local commits
## 5. Resolving a Conflict
### 5.1 Check the conflicting files
        git status
### 5.2 Edit each conflicting file and remove the conflict markers after selecting the correct finak content.
### 5.3 Mark the resolve file as prepared
        git add <filename>
### 5.4 Continue the rebase
        git rebase --continue
## 6. Pushing and Veryfying
        git push 
        git status -sb         
