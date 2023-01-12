# git
Git let's you manage a repository on the local machine or on a remote location. A few basic commands to get started with:

`git init`

This initiates the current folder with the git managing and versioning it from then on. A git repository can also be copied from a remote location using the below comand.

`git clone `*`<remote-git-url>`*

Once there's a git repository with you, the current state along with the changes could be viewed by simply asking the status like so.

`git status`

If there are changes present and you'd like to track it, then go ahead and add it to git.

`git add `*`<filename>`*

or if you'd like to add everything at once, then go ahead and play with the wildcards.

`git add .`

If you're done with the changes and would like to mark everything as a checkpoint, go ahead and make a commit with a reasonable commit message.

`git commit -m "Added git.md file to the tutorial"`

If you want to push the changes to the remote git server that you're working with, then go ahead and push the commits.

`git push`

# github

github is basically a git server. It enables people to collaborate by sharing git repositories across the internet.

Once you sign up with github, it let's you create a git repository and push files it or create it with some files initially and manage it from local.

## connecting to a github

`git remote add `*`<remote name> <remote git location>`

git origin is reseved for the user's remote repository. And upstream is usually the repository getting forked from.

Managing an forked repository could be like this,

`git remote add upstream `*`<remote repository url>`*
`
`git remote delete upstream`

`git remote set-url upstream `*`<new upstream url`*

Updates on a remote upstream could be fetched by,

`git fetch upstream`

To apply the commits from the remote on the local, a good method could be.

`git rebase upstream/develop`

Or, merge the commits on top of the local with

`git merge upstream/develop`
