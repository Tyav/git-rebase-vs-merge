# git-rebase-vs-merge
A simple demonstration on how rebase varies from merge

Rebase: 
This moves changes from a branch to another but alters the history by moving
the origin branch's starting point. It does not create a merge commit.

You should rebase in a feature branch when there are changes in it. Pull and rebase

```sh
git pull origin feature --rebase # for pulling into the local repos branch

git rebase <incoming-branch> # for bringing in updates from the incoming branch
```


