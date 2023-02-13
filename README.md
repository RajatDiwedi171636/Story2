Git, Git Hub and Version COntrol:

1. "git init" :- it initialise the git and make a hidden repository ".git/" you can see that "ls -a" 

2. "git status" : it is used to check which files are not added in the staging area so that after added to the staging area 
we can commit the changes. it shows all the files which are added or not added yet.

3. "git add <File-Name>" : it is used to add the file in staging area.

Ex: git add cahpter1.txt    
Now you can check again by "git status" it will show that chapter1.txt is added in the staging area and ready to be commited.

4. "git commit": it is used to commit all the changes and if you want to add message in your commit so that you can track what 
commit you have made then use 'git commit -m "Chapter1 completed"'

5. "git log": To check the logs of commit. it will show the commit details, time, message and a hash for that commit.

6. "git add ." : by this we can add multiple files in the staging area

Note: So now the flow is (WorkingDirectory ----git_add---> Staging_Area ---git_commit---> Local_Repository)
# So now what is the use of Staging Area. 
it usefull when we want to go back to the previous changes.

Ex: if we change something in chapter1.txt
 First:
7. "git diff <File-Name>" : to check the difference b/w previous and present changes.
  Ex: git diff chapter1.txt
 Then:
8.  "git checkout <File-Name>" : To roll back the changes from staging area. Ex: "git checkout chapter1.txt"

9. To add your code on git hub 
   st1.)First make a git hub repository copy the http address of it
   st2.)Now we need to create the remote repository by using: git remote add origin <Paste the Remote Directory address> 
   st3.)Now to push local repository to remote: git push -u origin master (here "origin" is remote repo and "master" is the branch)
   st4.)you can see your branch graph in network under insights. 

Note: .git is the local repo and github is the remote repo

10. To remove everything from the staging area: "git rm --cached -r ."
now you can check again by "git status"  
   
11. .gitignore: by the help of this file we can ignore the files that we don't want to add on git hub ex secret.txt file where 
we kept all the secret keys and confidential data.
-> In .gitignore file we can simply write the file name that we want to ignore
-> we can write comment in .gitignore file by using "#" 
-> *.txt means the files which have .txt extension will be ignored  

12. git clone <URL of the remote repo>: to clone the remote github repo

13. git branch <branch name> : to add a new branch Ex: git branch alien-plot
14. git branch : to see the no of branches

15. now to work on the branch that you have made you have to swith the branch: git checkout <branchName>
Ex: git checkout alien-plot
now make some changes and commit them
then come back to the master branch by git checkout master you can see there is no changes on the master branch 
now do some changes on master branch and commit them
 
16. Now to merge the alient-plot branch with master branch first you have to go to master branch then
git merge <branchName>: Ex: git merge alienPlot
and then type ":q!" to quit
now you can again push the changes to the git hub by : git push origin master -u

17. If you want to contribute to someone's repo on git hub you have to first "Fort" that repo which is to make copy of someone's 
repo to your own github repo
Now After make the changes on the repo that you copied to merge them you have to make the pull request from the github and 
add the message for ex what you have done to improve the code.
After that the Owner the repo that you have copied from will take tha action and see your pullrequest under pull request section
and compare the changes and give review to you. If he found that changes to be worth then he merge the pull request.
That's how you contribute on the git hub
 

 

