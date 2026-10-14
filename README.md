1- create a repo:
git init
git add.
git commit -m "first commit"

2-connect to remote repo:
git remote add origin git@github.com:ArwaHamdi26/Lab2.git


3-push to remote repo:
git push -u origin main


4-create two branches and add one file to each branch and push them to remote repo:
git branch dev
git branch test
git checkout dev
"create a file manually"
git add .
git commit -m "second commit"
git push -u origin dev


git checkout test
"create a file manually"
git add .
git commit -m "third commit"
git push -u origin test


5- merging the two branches on main
git checkout main
git merge dev
git merge test
git push

6- remove them locally and remotely
git branch -d dev
git push origin --delete dev

7-checkout another branch without commit changes:
git stash 
git stash list
git switch test
git switch main
git stash pop

8-create an annotated tag:
git tag -a v1.7 -m "version 1.7"

9-push the tag to the remote repo:
git push origin v1.7

10-To list all tags:
git tag

11-delete the tag locally and remotely:
git tag -d v1.7   (local)
git push origin --delete v1.7

12- 
![sunset sky](/assets/images.jpg "this is a pretty sunset sky")