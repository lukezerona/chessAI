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
To create a branch, follow the procedure below. 

```
   lukez@VENGEANCE MINGW64 ~/github
   $ cd chessAI/

   lukez@VENGEANCE MINGW64 ~/github/chessAI (main)
   $ git checkout -b intro_README
   Switched to a new branch 'intro_README'

   lukez@VENGEANCE MINGW64 ~/github/chessAI (intro_README)
   $ 
```

Notice, once you go into your cloned repo, that it says (main) next to the path. This means you are currently in a copy of the main branch of the repo. It will not let you push any changes to this branch. Then, you create and switch to a new branch - I called mine intro_README.

**Always make a new branch when adding changes to the repo**

Now, you can use VSCode to open up your repo and make changes to your code and do whatever you want!


## Pushing Your Branch Back to Git
When pushing your changes to your branch what you will do is following the procedure below:

```
   lukez@VENGEANCE MINGW64 ~/github
   $ cd chessAI/

   lukez@VENGEANCE MINGW64 ~/github/chessAI (main)
   $ git checkout -b intro_README
   Switched to a new branch 'intro_README'

   lukez@VENGEANCE MINGW64 ~/github/chessAI (intro_README)
   $ 
```

## VSCode
Optionally, there is a way to connect your vscode to git bash or github. This allows you to essentially do the same thing but all on vscode. Follow this or similar tutorial: https://code.visualstudio.com/docs/sourcecontrol/intro-to-git
