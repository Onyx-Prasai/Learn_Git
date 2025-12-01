# Fork
Forking is basically just copying a repo to our local file and keeping it in our repository as a rough copy. If we are creating a project and someone who is not a colobrate wants to contribute to our repo then the person can fork the project then work, contribute then send a pr to the main user or you can use it for your independent development.

There process to fork a repo is shown below:
1. First go to the project repository of the project that you want to fork.
2. Then you should see something like fork at right side from the project name
<br>
<img src="../Images/Fork.png" width=400px>
<br>

3. Now click on that fork button and then you will see a create a fork optoion
4. Now click on create a new fork and hence your forked copy is ready.
</br>

There is also another method to fork a file using a command in terminal
ie.
```bash
gh repo fork <owner>/<repository-name>
```
In place of owner you should keep the name of the github user whose fork you are going to make and in place of repository-name you should write the name of the repository you want to fork.

To fork a repo into a specific repo you can also use this command:
```bash
    gh repo fork <owner>/<repository-name> --org "my-organization"
```   
To automatically clone the forked file in your local machine you can use this command:
```bash
    gh repo fork <owner>/<repository-name> --clone
```
Now after this you have learned to fork a file for yourself.

[<<Back to Previous Page](./Merge&MergeConflict.md)  <div align="right">[Continue to Next Page >>](./SpecialGithubFiles.md) </div>


