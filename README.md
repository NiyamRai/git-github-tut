## Git

## Github

### Version Control

### Commands:

- clone->(from hosting to local machine)
- add->(track Files and changes)
- commit->(Save in git)
- push->(Upload to gitHub)
- pull-> (Download changes from remote repo)

#### To add Project First Time:

```sh
git init
git add .
git commit -m "initial commit" -m "description"
git remote add origin https://github.com/YOUR-ID/YOUR-REPOSITORY
git branch -M main
git push -u origin main
git push origin main(recomended)
(-u to make it default)
```

#### Initialising a git

```sh
git init
```

#### Staging the files

- to add all the files

```sh
git add .
```

- to add only selected file

```sh
git add <"file name">
```

- Alternate: to add all the files

```sh
git add --all
```

#### To bring back the data same to the last commit :

```sh
git checkout -f

OR

git checkout <"file names">
```

#### To see all the commits:

```sh
git log
git log -p -1
```

#### To get the status of git:

```sh
git status
```

#### To Remove A file from staging area (if added by mistake):

```sh
git rm --cached <"file name">
```

# Branching

- #### To create a new branch:

```sh
git branch dev1
```

- #### Moving to other branch:

```sh
git checkout dev1
```

- #### alternate way:

```sh
git checkout -b dev1
```

- #### To merge branch with the main brasnch:

```sh
git merge dev1
```

- #### To delete the Branch:

```sh
git branch -d dev1
```

- #### To push into the new branch:

```sh
git push -u origin dev1

git push origin dev1(Recomended)
```

## CLONE

```sh
git clone <"url of git repo">
```

#### To remove existing git data

```sh
rmdir -Force -Recurse .git
```

#### To chnage the origin (url) of the repo

```sh
git remote set-url origin <https-url>
```

## STASH

#### Adding stash

```sh
git stash
```

#### Getting previous stashed state

```sh
git stash apply
```

#### Listing All the Stash

```sh
git stash list
```

#### Getting stashed state from stash index

```sh
git stash apply 1
```

```sh
git stash apply <"stash index">
```

#### Adding stash

```sh
git stash push -m "initial stash"
```

#### To remove a stash

```sh
git stash drop 1
```

```sh
git stash drop <"stash index">
```

#### To bring back stash to normal flow

```sh
git stash pop 1
```

```sh
git stash pop <"stash index">
```

###### then we can use normal staging and commit

## Switching to another account

```sh
git config --global user.name "name"
```

```sh
git config --global user.email "email@example.com"
```

- then go to manage window credentials and remove all github creadentials
