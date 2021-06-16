### Install Ubantu

```bash
sudo apt-get install git -y
```
### Check Version

```bash
git --version
```

### Set Globaly
```bash
git config --global user.name AhmadAliCodility
git config --global user.email ahmed.ali@codilitysolutions.com

git config --list
    user.email=ahmed.ali@codilitysolutions.com
    user.name=AhmadAliCodility

```
### Initialize GIT

```bash
git init
```
### Show all hidden folders
```
ls -lart
total 16
drwxr-xr-x 3 lap-066 lap-066 4096 جون    16 10:45  ..
-rw-rw-r-- 1 lap-066 lap-066  383 جون    16 10:57 'git commands.md'
drwxrwxr-x 3 lap-066 lap-066 4096 جون    16 10:58  .
drwxrwxr-x 7 lap-066 lap-066 4096 جون    16 10:58  .git

```
### Git Status

```bash
git status

On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
	git commands.md
	index.html

nothing added to commit but untracked files present (use "git add" to track)

```

![Screenshot](screenshot.png)

### Add to staging Area and check Status

```bash
git add index.html

git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
	new file:   index.html

Untracked files:
  (use "git add <file>..." to include in what will be committed)
	git commands.md
	screenshot.png

```

### Commit
```bash
git commit -m "First commit"
```

### Checkout 
1. if some one change your file by mistake then this commandd will help you to recover your code back it  match with last commited file
1. I change on the index file and save it now i run this command to back my code

```bash
git checkout index.html
```
3. If Someone change all of your files and in Git status you found all files modified  then this command will help you to back to your last commit

Match with your previous commit and recover your file
```bash
git checkout -f
```