# GitLab

## To remove Local Branches ->
git branch -d dev
git branch -d test


## To remove Remote Branches ->
git push origin --delete dev
git push origin --delete test


## To list tags locally ->
git tag


## To delete tag locally ->
git tag -d v1.4


## To delete tag remotely ->
git push origin --delete v1.4


## What is git rebase? Give me an example.
Git rebase can integrate the changes from one branch to another by overcoming the problems that we might have faced while using the git merge command. The changes we will do will be recorded in the form of logs which are useful to go through if any mistakes happen.

Example: if we have f1, f2 in main branch
          and f3, f4 in NewBranch branch
          Switch to NewBranch branch and rebase:
          git checkout NewBranch
          git rebase main
          Result after rebase:
          f1, f2, f3, f4 in NewBranch


## What is pull request ?
A pull request is a request to merge changes from one branch into another branch in a Git repository. Typically, pull requests are used in collaborative workflows where multiple developers work on different features or fixes in separate branches. A pull request allows the team to review and discuss the proposed changes before they are merged into the main branch.

