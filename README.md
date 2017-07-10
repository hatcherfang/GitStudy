>>1. git command  
`refer url "http://stormzhang.com/github/2016/05/30/learn-github-from-zero3/"`  
>>>>- git init //init github repository  
>>>>- git status //check git status  
>>>>- git add <file> //add <file> into cache  
>>>>- git rm --cached <file> //remove <file> from cache  
>>>>- git commit -m "commit info" // commit with commit info  
>>>>- git log //to check commit log  
>>2. branch function: to make different feature develop independent.  
>>>>- git branch <branch name> // to create a new branch named <branch name>  
>>>>- git checkout <branch name> // to switch to branch <branch name>  
>>>>- git checkout -b <branch name> // to renew a branch <branch name> and auto-switch to it.  
>>3. merge switch branch to master branch step  
>>>>- git checkout master // first switch branch to master  
>>>>- git merge <branch name> // second merge <branch name> to master  
>>>>- git branch -d <branch name> // to delete branch <branch name>  
>>>>- git branch -D <branch name> // to force delete branch <branch name>  
>>4. tag function: to traceback errors.  
>>>>- git tag // to show tags  
>>>>- git tag <tag name> // to renew a tag named <tag name>  
>>>>- git checkout <tag name> // to switch the tag to <tag name>  
>>5. to login github and submit code to github  
>>>> to set the authentication refer `http://stormzhang.com/github/2016/06/04/learn-github-from-zero4/`  
>>>>- git clone git@github.com:<username>/<repository>.git  // to get the remote repository  
>>>>- git remote add origin git@github.com:<username>/<repository>.git //to attach local repository with remote's  
>>>>- git remote -v // to show the remote repository name  
>>>>- git push origin master // to push local code to remote master branch  
>>>>- git pull origin master // to update local code with remote branch. We usually first pull the remote code to local before push.  
>>6. to set the git username and email which will be shown on commit info  
>>>>- git config —global user.name "hatcherfang"  
>>>>- git config —global user.email "hatcherfang@163.com"  
>>7. git code update  
>>>>- git fetch git@github.com:<username>/<repository>.git  // to update the local repository  
>>>>- git diff <filename> // to diff the file <filename> with updated   
>>>>- git rm <filename> // to remove the file from repository  
>>>>- git mv <filename1> <filename2> // to rename the <filename1> to <filename2>  
>>8. git workflow  
![workflow](https://github.com/hatcherfang/git-study/blob/master/workflow.jpg)  
