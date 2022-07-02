# <span style="color:#57B8FF; font-weight: bold">Git</span>

## Usefull commands

- ### Basic commands

<div style="margin-left: 15px;">

<span style="color:#57B8FF; font-style: italic; font-weight: bold; margin-left:">git clone repository-url</span>        
to clone a repository from url

<span style="color:#57B8FF; font-style: italic; font-weight: bold">git clone repository-url -b branche-name</span>    
to clone a specific repository branch from url

<span style="color:#57B8FF; font-style: italic; font-weight: bold">git fetch</span>    
to get all the updates from the remote repository

<span style="color:#57B8FF; font-style: italic; font-weight: bold">git checkout branch-name</span>    
to switch the currently working branch

<span style="color:#57B8FF; font-style: italic; font-weight: bold">git checkout -b branch-name</span>    
to create a branch and switch to it

<span style="color:#57B8FF; font-style: italic; font-weight: bold">git branch</span>    
to see all the branch and the current one

<span style="color:#57B8FF; font-style: italic; font-weight: bold">git branch new-branch-name</span>    
to create a new branch

<span style="color:#57B8FF; font-style: italic; font-weight: bold">git branch -d branch-name</span>    
to delete a local branch

<span style="color:#57B8FF; font-style: italic; font-weight: bold">git remote</span>    
to manage set of tracked repositories 

<span style="color:#57B8FF; font-style: italic; font-weight: bold">git remote -v</span>    
to see remote url after name of tracked repository

<span style="color:#57B8FF; font-style: italic; font-weight: bold">git status</span>    
to see if branche has changes

<span style="color:#57B8FF; font-style: italic; font-weight: bold">git init</span>    
to start a new repository or reinitialize an existing one in the project root

<span style="color:#57B8FF; font-style: italic; font-weight: bold">git add file-path</span>    
to stage changed files individually

<span style="color:#57B8FF; font-style: italic; font-weight: bold">git add .</span>    
to stage all changed files

<span style="color:#57B8FF; font-style: italic; font-weight: bold">git diff</span>    
to see the staged changes

<span style="color:#57B8FF; font-style: italic; font-weight: bold">git diff --staged</span>    
to see unstaged changes on the current branch

<span style="color:#57B8FF; font-style: italic; font-weight: bold">git diff branch1 branch2</span>    
to compare two branches

<span style="color:#57B8FF; font-style: italic; font-weight: bold">git commit -m 'commit message'</span>    
to save the changes done locally

<span style="color:#57B8FF; font-style: italic; font-weight: bold">git pull</span>    
to fetch all the changes from the remote repository and merge any remote changes in the current local branch

<span style="color:#57B8FF; font-style: italic; font-weight: bold">git push</span>    
to push the locally commited changes to the remote branch

<span style="color:#57B8FF; font-style: italic; font-weight: bold">git push --set-upstream remote-branch branch-name</span>    
to push the locally commited changes to the remote branch if the branch is not yet tracked

---
</div>

- ### Advanced commands

<div style="margin-left: 15px;">

<span style="color:#57B8FF; font-style: italic; font-weight: bold">git bisect <\subcommand> <\subcommand></span>        
to use binary search to find the commit that introduced a bug
</div>

---

## Push process

        git add .
        git commit -m 'commit messsage'
        git checkout main
        git pull
        git checkout my_branch
        git rebase main
        if conflicts {
            git add .
            git rebase --continue
        }
        git push

---