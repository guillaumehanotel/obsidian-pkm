

#### Problem : Could not read from remote repository 
```shell
baf@baf:~/baf$ git pull
git@gitlab.com: Permission denied (publickey,keyboard-interactive).
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.
```
#### Solution : [La clé SSH n'est pas reconnue](https://stackoverflow.com/questions/4565700/how-to-specify-the-private-ssh-key-to-use-when-executing-shell-command-on-git)
```shell
baf@baf:~/baf$ cat ~/.ssh/config 
Host gitlab.com
  IdentityFile ~/.ssh/id_rsa_baf
  IdentitiesOnly yes
```