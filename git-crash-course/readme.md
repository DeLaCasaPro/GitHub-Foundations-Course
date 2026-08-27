## Following a youtube freecodecamp teacher

```sh
https://www.youtube.com/watch?v=Jdc0i7RcBv8&t=4206s
```

## Git Hidden Folder

There is an hidden folder called `.git` wich tells you that our folder is a git repo.

If we want to create a git repo in a new project we ' createthe folder and the initialize that repo using `git init`


```sh
mkdir /workspaces/tmp/new-project
cd /workspaces/tmp/new-project
git init
touch Readme.md
code Readme.md
git status
git add .
# makes changes to readme.md
git commit -a-m "add readme file"
```

## Cloning

We can clone three ways: HTTPS, SSH Github CLI

Since we are using Github Codespaces we'll create a temporary directory in our workspace

```sh
mkdir /worspaces/tmp/
cd /workspaces/tmp
```

### HTTPS
```sh
git clone https://github.com/DeLaCasaPro/GitHub-Foundations-Course.git
```
### SSH

### Github CLI

## Commits

When we want to commit code we can write git commit which will open up the commit edit message in the editor of choice

```sh
git commit
```

Set the global editor
```sh
git config --global core.editor emacs
git config --list --show-origin
git config --list --show-origin --show-scope
```

## Branches

## Remotes

## Stashing

## Merging

## Add

git add <file> d3c07185b8580561eaba65d0e5b948a24874f1f6

When we want to stage changes that will be included in the commit We can use the . to add all possible files.

```sh
git add Readme.md
git add .
```

## Reset

Reset allows you to move Staged changes to be unstaged
This is useful when you want to revert all files not to be not commited
```sh
git add .
git reset
```

> git reste will revert a git add .

## Status

git status shows you what files will or will not be commited.

```sh
git status
```

## Gitconfig file

The gitconfig file is what stores your global confogurations for git suchm as email, name, editor and more.

Showing the content of our .gitconfig file
```sh
git config --list
```

When you first setup git on a machine you are suppose to set up your name and email`

```sh
$ git config --global user.name "John Doe"
$ git config --global user.email johndoe@example.com
```