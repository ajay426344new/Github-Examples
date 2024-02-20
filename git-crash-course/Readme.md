## Git Hidden Folder

There is a hidden folder called '.git', which tells that our project is in a git intialised repo.

```sh
mkdir /Desktop/Git Projects/git-crash-course

git init
```

## Commits

When we want to commit code or save the changes that we did in the code then we can use "git commit", which will open up the commit edit message in the editor 

```
git commit -a "Messge"
```
## Merging

## Remotes

We can add remote but often you will just add remote via upstream, when adding a new branch and pushing it from local to repo.
```sh
git remote add ...
git branch -u origin new-branch-name
```
## Branches

```sh
git branch
git branch -a
git checkout branch-name
```
## Stashing

```sh
git stash list
git stash
git stash save name-of-the-stash
git stash apply
git stash pop
```

## Statging

## Cloning
    We can clone three ways: HTTPS, SSH, Github CLI

    Well make a temp directory to clone the codebase. 

```sh
    cd /Git Projects/git-crash-course
```
### HTTPS
```sh
        git clone https://github.com/ajay426344sec/Github-Examples.git
```
> You'll need to generate a personal access token(PAT) in order to push from local dev env.
>https://github.com/settings/token

## SSH

```sh
git clone git@github.com:ajay426344sec/Github-Examples.git
```
## Testing

## Add

When we want to stage changes that will be included in the commit
We can use the . to add all possible file to the staging phase.
```sh
git add Readme.md
```
## Reset

Reset allows you to move Staged changes to unstaged.
This is useful when you want to revert the changes without commiting.
```sh
git add .
git reset
```
>git reset will rrevert a git add

## Status

Git status shows you what files will or will not be commited.

```sh
git status
```

## Git Config file

The git config file is what stores your global configurations for git such as email, name editor and more.
Shoeking the contents of our .gitconfig file.
```
git cofig --list
```

 When you install Git on a machine, you're supposed to setup your name and email.

```sh
git config --global user.name "John Doe"
git config --global user.email johndoe@example.com
```

##edited using ssh methods