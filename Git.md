# My Git Docs

### General Syntax :

```
git clone <repo-link> // to copy repo from remot repo [Github,GitLab ...] to your local repo

git status // to show untracked files

git add <file-name> // to add the specific file to stage area

git add . // to add all file to staged area

git reset head <file-name> // to return the specific file to untracked files

git commit -m "Write your description about what you did" // to transport files from staged to local repo

git branch // to diplay all branches

git remote -v // to display all remotes

git push -u origin master   // -u . pull + push

git pull origin main // "fetch and merge "  to pull repo from remote and merge it with the local repo

```
### Configuration :
```
git config -l // show config

git help config

git config --global user.name "souf-devs"

git config --global --unset user.name 

```
### SSH Github Connection :

```
ssh-keygen -t ed25519 -C "ahmedsiradj9@gmail.com"

eval "$(ssh-agent -s)"

ssh-add ~/.ssh/id_ed25519

git clone <ssh-link>

```
```
ssh-add -l // display all keys
ssh-add -D // delete all cached keys

```

### Stach :

```
git stach // to hide files after adding theme

git stach save "message" // hide the file and save it with the message

git stach list

git stach pop // to call the last hidden file and remove it from the stach list

git stach apply // to call the last hidden file and do not remove it from the stach list

git stach pop stach@{4} // to call the specific hidden file
```
### Handle Github Repo from CLI :

***First of all you need to install `gh` packages to interact with github using cli***
> sudo apt-get install gh

##### For Create a repo :

```
gh repo create <repo-name> --private --clone --add-readme --description "your repo description" 

git pull origin main

git branch -m main

< add your changing here ... >

git push -u -f origin main 

```
##### For delete a repo :
***You Need to auth your self before start deleting :***
*Run this command*
> gh auth refresh -s delete_repo

*To delete the repo run this :*
> gh repo delete <repo-name> --confirm






















