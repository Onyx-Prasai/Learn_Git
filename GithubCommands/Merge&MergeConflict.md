# Git Merge
Git merge is simply merging two branches. It integrates work from different branches into a single unified history without losing progress. For example, you can merge a feature branch into the main branch to include all recent updates. This will not alter existing commits.

## What is the importance of merge?
<li>Preserves the complete commit history of both branches.</li>
<li>Performs automatic merges unless conflicts require manual resolution.</li>
<li>Uses fast-forward merge when no diverging commits exist.</li>
<li>Creates a merge commit to combine branch histories when necessary.</li>
<li>Does not delete branches after merging.</li>

## Commands for Merge
To create a new branch:
``` bash 
git merge <branch_name> 
```
Before merging, ensure that you pull the latest changes from both branches.
``` bash
git checkout <target-branch>    
git pull origin <target-branch>  

git checkout <feature-branch>   
git pull origin <feature-branch> 
```
Now we merge the branches:
``` bash
git checkout <target-branch>   
git merge <feature-branch>  
```    
# Merge Conflicts
A merge conflict happens when Git cannot automatically combine changes from two branches because both branches changed the same part of a file.
Git basically says:
“I don’t know which version you want. Please choose.”

The best ways to handle merge conflicts is by :
<ol>Merging two branches</ol>
<ol>Deleting one of the conflicting part</ol>

[<<Back to Previous Page](./Pullcmd.md)  <div align="right">[Continue to Next Page >>](./Fork.md) </div>
