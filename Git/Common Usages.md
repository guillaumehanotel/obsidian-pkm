## [Merger la branche dev dans master](https://stackoverflow.com/questions/14168677/merge-development-branch-with-master)

```shell
#(on branch development)
git merge master
# (resolve any merge conflicts if there are any)
git checkout master
git merge --no-ff develop #(there won't be any conflicts now)
```

## Ajouter du contenu au dernier commit
```shell
git commit --amend
git push -f
```

## [Throw away local commits in Git](https://stackoverflow.com/questions/5097456/throw-away-local-commits-in-git)
```shell
git reset --hard origin/<branch_name>
```

