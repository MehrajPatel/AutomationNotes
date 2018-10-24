# GIT NOTES

git config --global user.mail "email"
git config --global user.name "hostname"

git init //initialises empty git repository in current working directory
git status
git add <filename>  //add new file to repository. use . to add all new files
git commit -m "message for commit"  //commit to repository
git remote add origin "location of remote repository" // add remote repository
git push -u origin master // push to remote repository
git log // to get logs of git commits

git branch <branchName> // create new branch
git checkout <branchName> // set default branch for local commits
git push -u origin <branchName> // push changes to given branch; it will add new branch along with all files
git merge <branchName> // merge branch to master, before that we have to checkout (set default) to master branch
git push -u orign master // push changes to master
git branch -d <branchName> //delete branch from local 
git push origin --delete <branchName> //delete from remote repository

git tag <tagname> //create new tag
git tag -a <tagname> -m "message" //create annotated tag
git tag // show list of all created tags
git show <tagname> //get all information of given tag
git tag -l "wildcard" //get all tagnames accoriding to provided wildcard character
git push origin <tagname> //push tag to remote repository
git tag -d <tagname> or git tag --delete <tagname> //delete specific tag
git push origin -d <tagnames> // delete tag from remote 
git checkout -b <branchName> <tagname> // to checkout branch with tag
git tag <tagname> <reference of commit> // create tag for past commit
git push --tags // push changes to remote repository
