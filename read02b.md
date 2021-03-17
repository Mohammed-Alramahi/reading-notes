## Git
***
**Version control** is something we use to track down and manage the changes made to the software code over time 
If any issue or error is present with new version, 
we can go back and compare earlier versions of the code to help fix the mistake.

**Git** has a DVCS which is abbreviation for (Distributed Version Control) that gonna store the data
and it will track every change that we made.
It will also detect corrupted files which will minimize the possibility of the damage that can't be undone to files. and it has 3 states which is committed, modified and staged.
***
After we install Git we should immediately set a user name and email address so that it will be used for every Git commit.
- `$ git config --global user.name "Mohammed-Alramahi"`
- `$ git config --global user.email "vittosc1997@gmail.com"`

to set our default text editor we use:
- `$ git config --global core.editor "code --wait"`
to get our list of settings we use:
- `$ git config --list`
to get any help about some command just we type:
- `$ git help command`
while we replace command word with the command that we need help for.
***
when it comes to setting up an existing project to Git we gonna follow these steps:
1. `$ cd path`
1. `$ git init`
1. `$ git add *.c`
1. `$ git add LICENSE`
1. `$ git commit -m "message text"`

the following command will create a copy of an existing Git repository to the working directory:
- `$ git clone https://github.com/Mohammed-Alramahi/Mohammed-Alramahi`
to describe the state of files we use:
- `$ git status`
This command will commits modifications on files in the working directory:
- `$ git commit -a`
This command will push changes  from the local "locally" branch to the remote repository named "remotely"
- `$ git push remotely locally` 
will temporarily removes changes and hides them until we undo so:
- `$ git stash`
In order to show hidden changes use:
- `$ git stash apply`