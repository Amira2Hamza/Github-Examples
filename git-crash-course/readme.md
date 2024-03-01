## Git Hidden Folder

There is a hidden folder called `.git` which tells you that our project is a git repo.

If we want to create a new git rep in a new project we'd create the folder and then initialize that repo using `git init`

```
mkdir /workspaces/tmp/new-project
cd /workspaces/tmp/new-project
git init
touch Readme.md
code Readme.md
git status
git add Readme.md
# make changes to readme.md
git commit -m "add readme file"
```


## Cloning

We can clone three ways: HTTPS, SSH, Github CLI

Since we're using Gtihub Codespaces we'll create a temporary directory in our workspace

```sh
mkdir /workspace/tmp
cd /workspace/tm[]
```

### HTTPS

```sh
git clone https://github.com/Amira2Hamza/Github-Examples.git
cd Github-Examples
```

## Commits

When we want to commit code we can write git commit which will open up the commit edit message in the editor of choice.

```sh
git commit
```

Set the global editor
```
git config --global core.editor emacs
```

## Branches

## Remotes 

## Stashing

## Merging

## Add

When we want to stage changes that will be included in the commit we can use the . to add all possible files.

```
git add readme.md
git add .
```

## Reset

Reset allows you to move staged changes to be unsaved. 
This is useful when you revert all files not to be commited

```
git add .
git reset
```

> git reset will revert a git add.

## Status

Git status shows you whta files will owr will not be commited. 

```
git status
```

## Gitconfig file

The gitconfig file is what stores your global configuration for git such as email, name, editor and more.

Showing the contents of our .gitconfig file
```
git config --list
```

When you first install git on a machine you ar esupposed to set up your name and email

```sh
$ git config --global user.name "John Doe"
$ git config --global user.email johndoe@example.com
```