>>1. git command  
`refer url "http://stormzhang.com/github/2016/05/30/learn-github-from-zero3/"`  
>>>> git init //init github repository  
>>>> git status //check git status  
>>>> git add <file> //add <file> into cache  
>>>> git rm --cached <file> //remove <file> from cache  
>>>> git commit -m "commit info" // commit with commit info  
>>>> git log //to check commit log  
>>>> git push origin master // to push local code to remote master branch  
>>>> git pull origin master // to update local code with remote branch. We usually first pull the remote code to local before push.  
>> branch function: to make different feature develop independent.  
>>>>- git branch <branch name> // to create a new branch named <branch name>  
>>>>- git checkout <branch name> // to switch to branch <branch name>  
>>>>- git checkout -b <branch name> // to renew a branch <branch name> and auto-switch to it.  
>>2. merge switch branch to master branch step  
>>>>- git checkout master // first switch branch to master  
>>>>- git merge <branch name> // second merge <branch name> to master  
>>>>- git branch -d <branch name> // to delete branch <branch name>  
>>>>- git branch -D <branch name> // to force delete branch <branch name>  
>>3. tag function: to traceback errors.  
>>>>- git tag // to show tags  
>>>>- git tag <tag name> // to renew a tag named <tag name>  
>>>>- git checkout <tag name> // to switch the tag to <tag name>  
>>4. to login github and submit code to github  
`"refer url:http://stormzhang.com/github/2016/06/04/learn-github-from-zero4/"`  
