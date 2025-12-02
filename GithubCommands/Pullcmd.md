# Git pull
Git pull is a command used to update your local project with the latest changes from the online GitHub repository.

You can think of it like this:

- Your local folder = your copy

- GitHub remote repo = main copy

- If someone updates the main copy, your copy becomes old.

- To update your copy, you run: 

```bash
    git pull
```

This command does two things automatically:

- Fetch → downloads the latest changes from GitHub

- Merge → combines those changes with your local code

So basically:

git pull = download + update your local project.

## When to use git pull?

- Before you start coding

- When your teammate pushes new changes

- When GitHub is ahead of your local repo

- When you see "your branch is behind" message

## Quick Example

You open terminal inside your project and type:

``` bash
git pull origin main
```

This pulls the newest updates from the main branch.

[<<Back to Previous Page](./Git_Branches.md) <div align="right">[Continue to Next Page >>](./Merge&MergeConflict.md) </div>