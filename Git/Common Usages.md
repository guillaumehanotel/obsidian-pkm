

https://www.commands.dev/

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

## [Supprimer un fichier/dossier du tracking git](https://stackoverflow.com/questions/1274057/how-can-i-make-git-forget-about-a-file-that-was-tracked-but-is-now-in-gitign)
```shell
# Fichier
git rm --cached <file>
# Dossier
git rm -r --cached <folder>
```

## [Supprimer une branche en local et en remote](https://www.freecodecamp.org/news/how-to-delete-a-git-branch-both-locally-and-remotely/)
```bash
// delete branch locally
git branch -d localBranchName

// delete branch remotely
git push origin --delete remoteBranchName
```

