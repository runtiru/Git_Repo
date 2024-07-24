# Commands on git..?

* Basic commands

1. git init     --> initializes a new git repo
2. git status   --> it display the status of the repository, including any changes that need to be committed.
3. git add .    --> Stages all changes in the current directory and subdirectorues.
4. git commit -m "message" --> Commits changes with a meaningful message.
5. git log      --> Displays a log of all commits made to the repository
6. git log      --oneline -> Display a lof of all commits on short view.
7. git push     --> push the all changes after  commit local repo to remode repository.
8. git push -u origin master
9. git push -f -u origin master 
10. git pull    --> pull the all changes from remote repository to local repository.

---
* Git Configuration:

1. git config --global user.name "[name]" : Sets the global username.
2. git config --global user.email "[email]" : Sets the global email address.
3. git config --global core.editor "[editor]" : Sets the default editor for git commands.

---
* Branching and merging

1. git branch <branch name>     --> Create a new branch
2. git checkout <branch name>   --> change current branch to what you give.
3. git merge <branch name>      --> merge changes form another branch into the current branch.
4. git branch -d <branch name>  --> delete a branch
5. git remote add origin <url> 

---
* Git Status:

1. git status   --> it display the status of the repository, including any changes that need to be
committed.
2. git diff     --> Displays differences between files. it display the difference between the current branch and the branch you want to merge.
3. git diff --cached --> Displays differences between files that have been staged.

---
* Stashing and cherry-picking:

1. git stash        --> Stash all changes in the working directory and index.
2. git stash pop    --> Apply the most recent stash and remove it from the stash list.
3. git stash list   --> List all stashes.
4. git stash apply  --> Apply the most recent stash without removing it from the stash list.
5. git stash drop   -->Remove the most recent stash from the stash list.
6. git stash clear  --> Remove all stashes from the stash list.
7. git cherry-pick <commit hash> : Apply the changes from a specific commit to the
current branch.

---
* Rebasing and rewriting history:

1. git rebase <branch name> : Rebase the current branch on top of the specified
branch.
2. git rebase --interactive <commit hash> : Rewrite history by editing the specified commit.
3. git rebase --continue : Continue a rebase after resolving conflicts.
4. git rebase --abort : Abort a rebase and return to the previous state.


