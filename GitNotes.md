# __Notes For Git and GitHub__

## __To Upload Project to Github from VScode__

1. First you you need to set-up the project folder as git init.  
__Type__: ```git init``` in the terminal
2. Add all the files inside the project folder that you want to upload.  
__Type__: ```git add .``` where make sure using ```pwd`` to check you are in the correct folder that you want to add the file.
3. Commit the changes with a despriatoin, where -m represent message flag.  
__Type__: ```git commit -m "Inital commit"```
4. Link the repo to the project, do not include <>.  
__Type__: ```git remote add origin <repo-url>```
5. Push the code onto the repo, if you're working a branch other than the master branch replace the 'master'. Also -u is a shorthand flag of --setup-upstream. The 'origin' is the remote repo name, and 'master' is the local branch name. After set-up once by using ```git push``` without specifying remote branch name in future. Default branch name is called ```main```  
__Type__: ```git push -u origin main```

## __Addational Notes for git push -u origin master__  

A upstream is refers to the remote repo and branch that your local repo is linked to. It's the repo that you clone from or push changes to. When you set the up-stream by using flag ```-u``` with ```git push```. It established a connection between local branch and the online remote repo.  
  
To change the branch that you pushing into, instead ```master``` branch you need to specify the branch name. For example if you want to push another branch call, ```test-ver```, you would need to use the command ```git push origin test-ver```. That makes files and chages push to that branch however it does not changes the default push. In order to change it, you have to modify by using flag ```-u```. The command looks as fellow, ```git push -u origin test-ver```. Where it switch the up-stream to ```test-ver``` branch.  

### __Check remote name__

Type: ```git remote -v```

### __Change remote name__

Type: ```git remote rename <old-name> <new-name>```  

---

## __Branches__  

### __Check current branches and avaliable branches__  

Type: ```git branch```  

### __Create a Branch__

Type: ```git branch <new-branch-name>```

### __Delete a Branch__

Type: ```git branch -d <branch-name>```  

### __Switch to a branch__  

Type: ```git checkout <branch name>```  

---

## __Push your code to remote repo__

### __Add what you to change__

Type: ```git add .```  

### __Commit the changes__

Type: ```git commit -m "your msg"```  

### __Push changes__

Type: ```git push```  

### __Un-add changes__  

Type: ```git restore --staged <file>```  

### __Un-commit chages__

Type: ```git reset HEAD~```  
This will move the branch pointer to pervious commit  

---

## __Pull from remote__

### __Pull from main branch__

Type: ```git pull origin```

### __Pull a certain Branch__

Type: ```git pull origin <branch-name>```

---

## __GitHub Emoji markdown list__  

Use the fellowing link to find emoji that you can use in the GitHub page when you use markdown: [GitHub Emoji list](https://gist.github.com/rxaviers/7360908)  

You can also use regular copy and paste emoji in markdown: 🤙[Copy and Paste](https://getemoji.com/)🤏

