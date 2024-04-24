# chessAI
This is the initial chess AI Project with James. 

## Download
Easiest way I believe to download the repo is by using VSCode and Git Bash. Use this command in git bash:

```
   git clone https://github.com/lukezerona/chessAI.git
```

If there are problems with this, you may have to setup your git bash to connect to your github account. Follow this or a similar tutorial: https://docs.github.com/en/get-started/getting-started-with-git/set-up-git

The basic bash commands to go around the directory are: 

```
   # Go into a folder called chessAI
   cd chessAI

   # List all folders and files
   ls

   # Go back up to the parent folder
   cd ..
```

A branch allows you to create a version of the repo and make changes that you have without actually losing track of the original repo. So if you end up making a mistake, I can make comments to your branch, you can make changes, etc. Once we clear up the errors, we can merge your branch into main. Another reason we have branches is because if you find out that you have an error that was caused from 5 merges ago, we can go back in time to before you merged that branch and fix the error. 

## Branches 
To create a branch on your pc, follow the procedure below. 

```
   lukez@VENGEANCE MINGW64 ~/github
   $ cd chessAI/

   lukez@VENGEANCE MINGW64 ~/github/chessAI (main)
   $ git checkout -b intro_README
   Switched to a new branch 'intro_README'

   lukez@VENGEANCE MINGW64 ~/github/chessAI (intro_README)
   $ 
```

Notice, once you go into your cloned repo, that it says (main) next to the path. This means you are currently in a copy of the main branch of the repo. It will not let you push any changes to this branch. Then, you create and switch to a new branch - I called mine intro_README (notice the change in branch name).

**Always make a new branch when adding changes to the repo**

Now, you can use VSCode to open up your repo and make changes to your code and do whatever you want!


## Pushing Your Branch Back to Git
Once you get your changes working and you want to push your changes to your branch, follow the procedure below: 

```
   # checks what changes you added to your branch - red means not added yet, green means it was
   git status

   # adds specific file to your branch
   git add fileName

   # adds everything to your branch
   git add .

   # adds a message of what you are adding to your branch
   git commit -m "commit message"

   # if it's your first time creating this branch, this will create and push your changes to the branch on github
   git push --set-upstream origin nameOfBranch

   # push your changes to github if branch already exists
   git push
```

## Merge Request or Pull Request
Once you are finished pushing your changes to your branch on github. Go to github and create a merge or pull request. Name the merge request whatever, give it a description, assingn yourself as an assignee, add me a reviewer, and create. From here I can make comments about the code and whatnot and you can see it.

## Other git commands
```
   # switch to another branch that's already been created
   git checkout anotherBranch

   # If there is ever a desync of your branch from github and your local pc (I believe this would only happen if I made a change to your branch), you would want to pull the changes from github and realign the branches
   git pull

   # Let's say you have created a branch A and made a merge request and wanted to work on the next part, you would then create a branch off of branch A by first switching to branch A and following the commands below:
   lukez@VENGEANCE MINGW64 ~/github/chessAI (A)
   $ git checkout -b B
   Switched to a new branch 'B'
   
   # Then, let's say changes were made to branch A - branch B at this time won't contain those changes. To add those changes, go to branch B and type this command:
   $ git merge A
```

## VSCode
Optionally, there is a way to connect your vscode to git bash or github. I believe this allows you to essentially do all of these same things but all on vscode. Follow this or similar tutorial: https://code.visualstudio.com/docs/sourcecontrol/intro-to-git
