
# Downlad and Installation
So, basically git is a version control system tool that helps to tract changes in a code made by the user. There are many version control system but git is popular because it it free and open source as well as fast and scalable at the same time.

First download and install Git from the website:

For windows and mac users: 
<a href="https://git-scm.com/install/" target="_blank">Download Git</a>


For UBUNT/Debian users: 
```bash 
sudo apt install git -y
```
For Fedora users: 
```bash 
sudo dnf install git -y
```
For Arch users: 
```bash 
sudo pacman -S git
```
- - - - 
Then check whether git is intalled or not
```bash
git --version
```
This command is also used to check the version of the git that is installed.
- - - -

# Configure your Git 
```bash
git config --global user.name "YourName"
``` 
In "YourName" type your github account username. This user name will be set as the author for your Git Commits.

```bash
git config --global user.email "YourEmail"
```
In "YourEmail" use your own user email. It's purpose is to set the email address that Git will include in the data when you make any changes.

```bash
git config --list
```
This command will find all the possible configures that git can use.

- - - -
After this you will be able to download, install and configure git in your device. If you have vs code installed you can also download github copilot extension there.
- - - -
[⬅️ Previous Page](../README.md) 


