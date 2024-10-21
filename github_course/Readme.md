## Git hidden folder

`.git` folder (hidden) tells your project is a git repo.
create a git repo in new project > create folder > initalize that repo using `git init`

```
mkdir /workspaces/temp/new-project
cd /workspaces/temp/new_project
git init
touch Readme.md
open Readme.md
# make changes to Readme.md
git commit -a -m "add readme file"
```

### Cloning

Three ways : HTTPS, SSH, Github CLI

```ssh
git clone https://github.com/hiranyagarbh/Github-Examples.git
```

### SSH

```sh
git clone git@github.com:hiranyagarbh/Github-Examples.git
```

```sh
mkdir /workspace/tmp
cd  /workspace/temp
```

## Github CLI
```
brew install gh
```

```
gh login
gh repo clone hiranyagarbh/Github-Examples
```

## Commits
to commit code -> which in turn open up the commit edit message
```sh
git commit
```
make a commit and commit message without opening an editor
```sh
git commit -m "_COMMIT_MESSAGE_HERE_"
```

to set global editor
```
git config --global.editor emacs
```

## Branches
list of branches
```
git branch
```

create a new branch
```
git branch _branch_name_
```

switch/checkout the branch
```
git checkout _branch_name_
```

### To push the current branch and set the remote as upstream, use
```
git push --set-upstream origin dev
```
or
```
git push -u origin dev
```
## Stashing
```
git stash
git stash list
git stash save _instance_name_
git stash apply
git stash pop
```
## Merging

# Add
```
git add Readme.md
```
to stage changes to be included in the commit. `git add .` to add all possible files.

# Status
`git status` will show what files will or will not be commited.

# Reset

to move Staged changes to be unStaged - when you want to revert **all** staged files

```sh
git add .
git reset
```
# Gitconfig File
stores global config for git such as email, editor etc.
```sh
git config --list --show-origin
```

# Log
`git log` will show recent git commits in the git tree

# Push

to push a repo to a remote origin
```
git push
```
