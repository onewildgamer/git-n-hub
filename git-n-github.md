# git
Git let's you manage a repository on the local machine or on a remote location. A few basic commands to get started with:

<pre>git init</pre>

This initiates the current folder with the git managing and versioning it from then on. A git repository can also be copied from a remote location using the below comand.

<pre>git clone <i>&lt;remote-git-url&gt;</i></pre>

Once there's a git repository with you, the current state along with the changes could be viewed by simply asking the status like so.

<pre>git status</pre>

If there are changes present and you'd like to track it, then go ahead and add it to git.

<pre>git add <i>&lt;filename&gt;</i></pre>

or if you'd like to add everything at once, then go ahead and play with the wildcards.

<pre>git add .</pre>

If you're done with the changes and would like to mark everything as a checkpoint, go ahead and make a commit with a reasonable commit message.

<pre>git commit -m "Added git.md file to the tutorial"</pre>

If you want to push the changes to the remote git server that you're working with, then go ahead and push the commits.

<pre>git push</pre>

# github

github is basically a git server. It enables people to collaborate by sharing git repositories across the internet.

Once you sign up with github, it let's you create a git repository and push files it or create it with some files initially and manage it from local.

## connecting to a github

<pre>git remote add <i>&lt;remote name&gt; &lt;remote git location&gt;</i></pre>

git origin is reseved for the user's remote repository. And upstream is usually the repository getting forked from.

Managing an forked repository could be like this,

<pre>git remote add upstream <i>&lt;remote repository url&gt;</i></pre>
</pre>
<pre>git remote delete upstream</pre>

<pre>git remote set-url upstream <i>&lt;new upstream url&gt;</i></pre>

Updates on a remote upstream could be fetched by,

<pre>git fetch upstream</pre>

To apply the commits from the remote on the local, a good method could be.

<pre>git rebase upstream/develop</pre>

Or, merge the commits on top of the local with (prefer this method than the above until you learn git in depth)

<pre>git merge upstream/develop</pre>

Refer: [Git documentation](https://git-scm.com/docs/gittutorial)
