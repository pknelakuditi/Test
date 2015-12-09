
## Git Development for Code Reviews :

1. Create a new remote branch from dev branch   
<code>git checkout dev</code>   
<code>git checkout -b new-branch</code>  

2. Pushing new branch to remote   
<code>git push origin new-branch</code>  

3. work on local new branch, push changes to remote   
<code>git push origin new-branch</code>   

4. when submitting for code review    
update dev and merge new-branch to dev using --no-ff option, resolve if any conflicts   
<code>git pull origin dev</code>   
<code>git checkout dev</code>   
<code>git merge --no-ff  new-branch</code>   

This merge can be used to code reviews.   
Point the merge Url for code review to see all the changes done after previous deviation from dev branch.  