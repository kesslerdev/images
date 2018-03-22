# Composer Command

Create an alias
```
alias composer 'docker run --rm --interactive --tty --volume $PWD:/app --volume $SSH_AUTH_SOCK:/ssh-auth.sock --volume /etc/passwd:/etc/passwd:ro --volume /etc/group:/etc/group:ro --user (id -u):(id -g) --env SSH_AUTH_SOCK=/ssh-auth.sock kesslerdev/composer'
```
