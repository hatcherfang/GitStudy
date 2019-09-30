## Git command  
`refer url http://stormzhang.com/github/2016/05/30/learn-github-from-zero3/`  
- git init //init github repository  
- git status //check git status  
- git add <file> //add <file> into cache  
- git rm --cached <file> //remove <file> from cache  
- git commit -m "commit info" // commit with commit info  
- git log //to check commit log  
## Branch function: to make different feature develop independent.  
- git branch <branch name> // to create a new branch named <branch name>  
- git checkout <branch name> // to switch to branch <branch name>  
- git checkout -b <branch name> // to renew a branch <branch name> and auto-switch to it.  
## [Get remote branch into local](https://www.cnblogs.com/fuyanwen/archive/2012/12/29/2838676.html)  
- list all of the branch  
`git branch -a`  
- fetch remote branch to local, if branchname not exist in local, it will be created    
`git fetch origin "remote-branchname":"local-branchname"`   
- checkout remote branch to local and switch to the branch   
`git checkout origin/"remote-branchname" -b "local-branchname"`  

## Merge switch branch to master branch step  
- git checkout master // first switch branch to master  
- git merge <branch name> // second merge <branch name> to master  
- git branch -d <branch name> // to delete branch <branch name>  
- git branch -D <branch name> // to force delete branch <branch name>  
## Tag function: to traceback errors.  
- git tag // to show tags  
- git tag <tag name> // to renew a tag named <tag name>  
- git checkout <tag name> // to switch the tag to <tag name>  
- git tag -a <tag name> -m "comment"  // to add annotated tag with comment  
- git tag -d <tag name>  // delete local tag  
- git push origin :refs/tags/<tag name> // delete remote tag   
- git push origin <tag name>  // to commit tag   
## Login github and submit code to github  
 `to set the authentication refer http://stormzhang.com/github/2016/06/04/learn-github-from-zero4/`  
- git clone git@github.com:<username>/<repository>.git  // to get the remote repository  
- git remote add origin git@github.com:<username>/<repository>.git //to attach local repository with remote's  
- git remote -v // to show the remote repository name  
- git push origin master // to push local code to remote master branch  
- git pull origin master // to update local code with remote branch. We usually first pull the remote code to local before push.  
## Set the git username and email which will be shown on commit info  
- git config --global user.name "hatcherfang"  
- git config --global user.email "hatcherfang@163.com"  
- to check the config file `vim .git/config`
## Git code update  
- git fetch git@github.com:<username>/<repository>.git  // to update the local repository  
- git diff <filename> // to diff the file <filename> with updated   
- git rm <filename> // to remove the file from repository  
- git mv <filename1> <filename2> // to rename the <filename1> to <filename2>  
## [Git SSH configure](https://help.github.com/articles/adding-a-new-ssh-key-to-your-github-account/)    
1. Checked for existing SSH keys  
`ls ~/.ssh/`  
If id_rsa.pub not exists, go to step 2.

2. Generated a new SSH key and added it to the ssh-agent   
- `ssh-keygen -t rsa -b 4096 -C "your_email@example.com"`  
- `ssh-add ~/.ssh/id_rsa`  
3. copy SSH key `id_rsa.pub`(~/.ssh/id_rsa.pub) to your github account   
4. try to use git clone `repo path` to download code  


## Git workflow  
![workflow](https://github.com/hatcherfang/git-study/blob/master/workflow.jpg)  
## [Git create remote branch](https://blog.csdn.net/github_38395241/article/details/77198673)  
git checkout -b my-test  //create local branch my-test under current branch  
git push origin my-test  //push my-test branch to remote   
git branch --set-upstream-to=origin/my-test //将本地分支my-test关联到远程分支my-test上   
git branch -a // to check remote branch  
