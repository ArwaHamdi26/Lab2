Git & GitHub Lab 2
This lab covers the basic Git and GitHub workflow, including repository creation, remote connection, branch management, merging, stashing, and tagging.

1. Create a Repository
Initialize a Git repository, add the files, and create the first commit.

git init
git add.
git commit -m "first commit"
2. Connect to a Remote Repository
Connect the local repository to the GitHub remote repository.

git remote add origin git@github.com:ArwaHamdi26/Lab2.git
3. Push to the Remote Repository
Push the main branch to GitHub and set the upstream branch.

git push -u origin main
4. Create Two Branches and Push Them to the Remote Repository
Create the dev and test Branches
git branch dev
git branch test
Add a File to the dev Branch
Switch to the dev branch, create a file manually, add the changes, commit them, and push the branch to GitHub.

git checkout dev
"create a file manually"
git add .
git commit -m "second commit"
git push -u origin dev
Add a File to the test Branch
Switch to the test branch, create a file manually, add the changes, commit them, and push the branch to GitHub.

git checkout test
"create a file manually"
git add .
git commit -m "third commit"
git push -u origin test
5. Merge the Two Branches into main
Switch to the main branch, merge the dev and test branches, and push the changes to GitHub.

git checkout main
git merge dev
git merge test
git push
6. Delete Branches Locally and Remotely
Delete the dev branch from the local repository and the remote repository.

git branch -d dev
git push origin --delete dev
7. Switch Branches Without Committing Changes
Use Git stash to temporarily save uncommitted changes, list the saved stashes, switch between branches, and restore the changes.

git stash
git stash list
git switch test
git switch main
git stash pop
8. Create an Annotated Tag
Create an annotated tag named v1.7 with a message describing the version.

git tag -a v1.7 -m "version 1.7"
9. Push the Tag to the Remote Repository
Push the v1.7 tag to GitHub.

git push origin v1.7
10. List All Tags
Display all tags available in the local repository.

git tag
11. Delete a Tag Locally and Remotely
Delete the v1.7 tag from the local repository and the remote repository.

Delete the local tag:

git tag -d v1.7
Delete the remote tag:

git push origin --delete v1.7

12. Add an Image
Add an image to the README file using Markdown syntax.

!sunset sky

Conclusion
This lab demonstrates essential Git and GitHub operations, including:

Initializing a repository and creating commits.
Connecting a local repository to GitHub.
Creating, managing, and deleting branches.
Pushing branches and changes to a remote repository.
Merging branches into main.
Temporarily saving and restoring uncommitted changes using Git stash.
Creating, pushing, listing, and deleting annotated tags.
Adding and displaying an image in the README file using Markdown syntax.