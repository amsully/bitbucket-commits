# bitbucket-commits
Don't let private bitbucket repos ruin your github streak! Create your own github 'bitbucket' repo and record any bitbucket commit on github without committing the code... with one command! 

## Reqs'
Developed and tested: Ubuntu 14.04

Tested: OSX

## Set-Up

### Fork this repository...

 such that you have your own instance (eg: Mine is https://github.com/amsully/bitbucket-commits)

### Clone your newly forked repository onto your local machine

Example:

```
git clone https://github.com/<github name here>/bitbucket-commits.git
```

### Move repo into /etc/

```
sudo mv /path/to/bitbucket-commits /etc/
```

### Navigate into bitbucket commits

```
cd /etc/bitbucket-commits
```

### Copy git-commit-bitbucket into /usr/bin/

```
sudo cp git-commit-bitbucket /usr/bin/
```

Notes: The new version requires less configuration but will always push to your bitbucket-commits repo.

## Use

Now we want to push to our bitbucket repo but also let github know we are coding up a storm!

### Add changes

In the bitbucket repository you are working on simply add changes as normal.

```
git add *
```

### Commit/Push to Bitbucket/ Push to Github

Now we call one command to do everything for us.

```
git commit-bitbucket -m "My streak is alive and I pushed to bitbucket!"
```

##TODO:
- Implement error handling (currently very much only a script)
- ~~Test on Mac~~
- Append commit messages to file rather than overwrite
- Simple formatting (date/bitbucket repo title) within auto commits
- Man pages















