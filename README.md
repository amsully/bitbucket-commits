# bitbucket-commits
Don't let private bitbucket repos ruin your github streak! Create you github 'bitbucket' repo and any push to your bitbucket push will be recorded as a commit in this directory :)

## Reqs'
Developed and tested: Ubuntu 14.04

## Set-Up
Clone this repository

Copy git-commit-bitbucket into usr/bin

'cd' into bitbucket-commits repo and then:
```
# cp git-commit-bitbucket /usr/bin/
```

## Configure

This command sets up the github destination of the 'auto' repo.
A config file is created in /etc/.bitbucket.cfg
The repo that will be pushing to github will be created in /etc/bitbucket-commits
```
git commit-bitbucket -c "direct https link to Auto github repo"
```

## Use
When editing a project on your private bitbucket repo, configure git like one would normally (setting remote repo to bitbucket).

When you have added everything you wanted into your commit use:

```
git commit-bitbucket -m "title" -m "description" ...etc
```
This will perform git commit -m ... on your bitbucket repo as well as add the title and description to your bitbucket-commits repo **and push to the repo on github**. This means git commit-bitbucket is a push to github and a commit for your local bitbucket repo.

Finally perform git push to push the files to bitbucket.

Viola! You have committed to your bitbucket private repo AND kept your streak alive ;)

##TODO:
- Implement error handling (currently very much only a script)
- Test on Mac
- Append commit messages to file rather than overwrite
- Simple formatting (date/bitbucket repo title) within auto commits
- Man pages
- 















