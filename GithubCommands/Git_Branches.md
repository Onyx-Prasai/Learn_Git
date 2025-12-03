# Git Branches

Branches in Git allow developers to work on different versions of a project at the same time without affecting the main codebase.

A branch is simply a movable pointer to a commit. The default branch in most repositories is `main`.

## Why Use Branches?

- To isolate features
- To fix bugs without touching the main code
- To experiment safely
- To collaborate with teams easily
- To keep production stable while development continues

  ## Types of Git Branches

- **main** → stable production code  
- **dev** → integration of new features  
- **feature branch** → new features  
- **bugfix branch** → fixes for specific issues  
- **hotfix branch** → urgent production fixes  
- **release branch** → preparation for a release

## Creating a Branch

```bash
git branch feature-login
git checkout feature-login

# OR shortcut
git checkout -b feature-login
```
<h3>Here you have learned about branching in git and github.</h3>


[<<Back to Previous Page](./Workflow.md) <div align="right">[Continue to Next Page >>](./Pullcmd.md) </div>
