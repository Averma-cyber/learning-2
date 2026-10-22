this is learning-2 created to learn git init, git add, git push, etc.


PUSH COMMAND :  push basically uploads the local repo content to the remote repo.

"git push origin main"


INIT COMMAND : used to create a new repo

"git init" --> used to initialize the git once you have created a new repo on your local
"git remote add origin <link>" --> connects your local Git repository to a remote repository- think of it as connecting the git project on your laptop to an online repo where you can store and share your code.


understanding each part - 

git : Runs Git.
remote : Manages connections to remote repos
add : adds a new remote connection.
origin: the conventional name given to that remote connections.
<link> : the url of your online repo


git remote -v : to verify remote

git branch : to check branch

git branch -M <new name> : to rename a branch

git push origin main : to push local repo to the main remote repo


git pull origin main --allow-unrelated-histories : the error non-fast-forward means your GitHub repo already contains commits that your local repo doesn't have. For example , you may have created a README.md file on GitHub when creating the repo.
Git refuses to push because doing so could overwrite changes that exists on GitHub.

the above command downloads and merges the changes from GitHub into your local main branch. the --allow-unrelated-histories flag is needed only if your local repo and GitHub repo were initialized separately.

