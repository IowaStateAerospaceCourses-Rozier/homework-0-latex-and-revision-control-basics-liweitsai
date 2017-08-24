# Discussion

### Basic Git Workflow  
**Git** is a version control tool. In general, you would first have a master branch which includes all the original files. After you start to work, you could build other branches from your current branch. This process would save the current status of your current branch as a new branch. Simply type the following commands to create a new branch and move to the new branch you just made.  
```  
git branch <branchname>  
git checkout <branchname>  
```  
Also, you could use   
``` 
git branch  
```  
It would indicate all the branches you have and the current branch you are working on. As soon as you make some revisions on your original files, Git will trace those changes. You could type 
```  
git status  
```
It would show which branch you are working on, files need to be commited and files not staged for commit. In Git, you need two steps to confirm your changes and update your current branch. First, you would use 
```  
git add <filename>  
```  
to add changes to be staged for commit. Second, you would use 
```  
git commit  
```   
to commit those changes. You could also combine two branches together by using 
``` 
git merge <branchname>
```  
This would merge your current branch to your target branch. Sometimes, merge process may have some conflicts. To solve conflicts, you would have a comparison of two branches and you would need to decide which part you want to leave or cancel.  

**Github** realizes the functions of Git on the Internet. When we are working in a group, it's more convenient to have our common files on a cloud space and use a version controll tool to manage our files. Once you run through the basic steps above on your local machine and get your current branch be ready. You could use 
```  
git push <remote> <branchname>
```
to upload your current branch to your target branch on your remote repository. If your target branch doesn't exist on your remote repository, you would create a new branch on your remote repository. Since your team members would also upload their branches, you could also use 
```  
git pull <remote> <branchname>  
```  
to update your local branches. This command would pull the target branch to update your current branch. 
### The Importance of Good Documentation 
