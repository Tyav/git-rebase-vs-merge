# git-rebase-vs-merge
A simple demonstration on how rebase varies from merge

Rebase: 
This moves changes from a branch to another but alters the history by moving
the origin branch's starting point. It does not create a merge commit.

You should rebase in a target branch when there are changes in it. Pull and rebase

Rebasing is better to streamline a complex history, you are able to change the commit history by interactive rebase. 
You can remove undesired commits, squash two or more commits into one or edit the commit message.
Rebase will present conflicts one commit at a time whereas merge will present them all at once.

```sh
git pull origin feature --rebase # for pulling into the local repos branch

git rebase <incoming-branch> # for bringing in updates from the incoming branch while in target branch
```

Merge: 
This moves changes from a branch to another and creates a merge commit. It preserves the history.

You should use merge if the target branch has no changes.

```sh
git pull origin feature # by default the --merge flag is used

git merge target-branch # This means that there are no changes in the current branch
```



