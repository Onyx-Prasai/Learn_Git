# Git Add

Suppose you have a project in your repo and you are working with that. Now when you make some changes the file and check status. Now there will be in multiple stages.
<br>
- Untracked Files: <br>
    Like, when there is a new file that git does not track then the file is known as untracked file. Suppose you create a new file in that same repo. Here you will see that the file is untracked.

    <img src="https://phoenixnap.com/kb/wp-content/uploads/2022/09/check-untracked-files.png" width=500px>
- - - -
- Modified Files:<br>
    They are the changed files where were previously in the repo.

    <img src="https://www.junosnotes.com/wp-content/uploads/2021/07/Adding-deleted-and-modified-files-only-git-add-deleted-files.png" width=500px>
- - - - 
- Staged Files: <br>
    The file is ready to be committed

    <img src="https://i.sstatic.net/9eFLZ.png" width=500px>
- - - - 
- Unmodified files: <br>
    These are unchanged files.

- - - - 

<h2>For better Understanding</h2>

<img src="https://git-scm.com/book/en/v2/images/lifecycle.png" width=750px>

<h4>So, when we change a file in our working directory we need to update it in our git at any time so in this case we use git-add command. Add helps to add new or changed files from your working directory to the git staging Area.</h4>

The command for adding your file is:
You can do add single file manually as shown in the followng code below
```bash
git add <-file name->
```
In case of <-file name-> you should be writing your file's name.

Now, It is hard to add a single file at a single time so, we can also add all the files present at the same time.
The following command adds all the file from that project.
```bash
git add .
```
# Git Commit
It is the basically just the record of changes made. 

You can use the following code to commit:
```bash
git commit -m "Type_Message_Here"
```
In place of Type_Message_Here you should type a meaningful message related to your changes or anyhing. And dont forget to use that " ".

<h3>So, after this you will be able to add and commit your files in github.</h3>

[<<Back to Previous Page](./Clone&Status.md)  <div align="right">[Continue to Next Page >>](./Init.md) </div>


