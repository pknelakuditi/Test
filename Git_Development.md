
# Git Development and Code Reviews :

1. Create a new remote branch from dev branch
<code>git checkout dev
git checkout -b new-branch</code>

2. Pushing new branch to remote
git push origin new-branch

3. work on local new branch, push changes to remote 
git push origin new-branch

4. when submitting for code review 
*  update dev and merge new-branch to dev using --no-ff option, resolve if any conflicts 
git pull origin dev
git checkout dev
git merge --no-ff  new-branch

this merge can be used to code reviews.

Point the merge Url for code review to see all the changes done after previous deviation from dev branch.