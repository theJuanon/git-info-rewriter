# git-info-rewriter
For those who wants to rewrite their username and email from old git commits.

## USAGE
From your terminal: Execute the next script following with your desired info in this order:

```bash
./git-info-rewrite.sh <old_email@example.com> <username> <new_email@example.com>
```
>Copy the script from above replacing the params with your actual info (omit the "<>" symbols)

## FOR REMOTE REPOS
If the commits you want to change are already in a remote repository and you want to push the changes you will need to force the push. (Because we are basically rewriting the repo's history)

```bash
git push --force --tags origin 'refs/heads/*'
```