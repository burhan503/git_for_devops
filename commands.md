
# Git Commands Reference

## 1. Basic Setup This all commands is used for devops

- **Initialize a new Git repository**
  ```bash
  git init
  ```

- **Configure Git username**
  ```bash
  git config --global user.name "burhan503"
  ```

- **Configure Git email**
  ```bash
  git config --global user.email "job.khanburhan503@gmail.com"
  ```

## 2. Working with Files

- **Create a new file using Vim**
  ```bash
  vim burhan1.txt
  vim burhan2.txt
  ```

- **Add files to staging area**
  ```bash
  git add burhan1.txt burhan2.txt
  ```

## 3. Viewing Status and Logs

- **Check the status of the repository**
  ```bash
  git status
  ```

- **View commit history**
  ```bash
  git log
  ```

- **View commit history in one line**
  ```bash
  git log --oneline
  ```

## 4. Committing Changes

- **Commit changes with a message**
  ```bash
  git commit -m "Update the both file for checking this"
  ```

- **Commit new files**
  ```bash
  git add burhan3.txt/
  git commit -m "add new file"
  ```

## 5. Branch Management

- **Check current branch**
  ```bash
  git branch
  ```

- **Switch to the master branch**
  ```bash
  git checkout master
  ```

## 6. Additional Commands

- **List files in the current directory**
  ```bash
  ls
  ```

- **View Git statistics (if available)**
  ```bash
  git stats
  ```






$ git status
On branch main
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean

Administrator@DESKTOP-U27GP0N MINGW64 ~/Desktop/sh files/git_for_devops (main)
$ git push
fatal: User cancelled dialog.
error: unable to read askpass response from 'C:/Program Files/Git/mingw64/bin/gi
t-askpass.exe'
Username for 'https://github.com': burhan503
error: unable to read askpass response from 'C:/Program Files/Git/mingw64/bin/gi
t-askpass.exe'
Password for 'https://burhan503@github.com':
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 312 bytes | 312.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/burhan503/git_for_devops.git
   2081900..20de910  main -> main

Administrator@DESKTOP-U27GP0N MINGW64 ~/Desktop/sh files/git_for_devops (main)
$ ls
commands.md

Administrator@DESKTOP-U27GP0N MINGW64 ~/Desktop/sh files/git_for_devops (main)
$ vim README.md

Administrator@DESKTOP-U27GP0N MINGW64 ~/Desktop/sh files/git_for_devops (main)
$ git add .
warning: in the working copy of 'README.md', LF will be replaced by CRLF the next time Git touches it

Administrator@DESKTOP-U27GP0N MINGW64 ~/Desktop/sh files/git_for_devops (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   README.md


Administrator@DESKTOP-U27GP0N MINGW64 ~/Desktop/sh files/git_for_devops (main)
$ git commit -m "Add Readme.md file"
[main 1e549ca] Add Readme.md file
 1 file changed, 3 insertions(+)
 create mode 100644 README.md

Administrator@DESKTOP-U27GP0N MINGW64 ~/Desktop/sh files/git_for_devops (main)
$ git remote -v
origin  https://github.com/burhan503/git_for_devops.git (fetch)
origin  https://github.com/burhan503/git_for_devops.git (push)

Administrator@DESKTOP-U27GP0N MINGW64 ~/Desktop/sh files/git_for_devops (main)
$ git remote set-url https://tockenHEre@github.com/burhan503/git_for_devops.git
usage: git remote set-url [--push] <name> <newurl> [<oldurl>]
   or: git remote set-url --add <name> <newurl>
   or: git remote set-url --delete <name> <url>

    --[no-]push           manipulate push URLs
    --[no-]add            add URL
    --[no-]delete         delete URLs


Administrator@DESKTOP-U27GP0N MINGW64 ~/Desktop/sh files/git_for_devops (main)
$ git remote origin set-url https://tockenhere>X@github.com/burhan503/git_for_devops.git
error: unknown subcommand: `origin'
usage: git remote [-v | --verbose]
   or: git remote add [-t <branch>] [-m <master>] [-f] [--tags | --no-tags] [--mirror=<fetch|push>] <name> <url>
   or: git remote rename [--[no-]progress] <old> <new>
   or: git remote remove <name>
   or: git remote set-head <name> (-a | --auto | -d | --delete | <branch>)
   or: git remote [-v | --verbose] show [-n] <name>
   or: git remote prune [-n | --dry-run] <name>
   or: git remote [-v | --verbose] update [-p | --prune] [(<group> | <remote>)...]
   or: git remote set-branches [--add] <name> <branch>...
   or: git remote get-url [--push] [--all] <name>
   or: git remote set-url [--push] <name> <newurl> [<oldurl>]
   or: git remote set-url --add <name> <newurl>
   or: git remote set-url --delete <name> <url>

    -v, --[no-]verbose    be verbose; must be placed before a subcommand


Administrator@DESKTOP-U27GP0N MINGW64 ~/Desktop/sh files/git_for_devops (main)
$ git remote set-url origin https://tockenhere@github.com/burhan503/git_for_devops.git

Administrator@DESKTOP-U27GP0N MINGW64 ~/Desktop/sh files/git_for_devops (main)
$ git push
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 389 bytes | 194.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/burhan503/git_for_devops.git
   20de910..1e549ca  main -> main

Administrator@DESKTOP-U27GP0N MINGW64 ~/Desktop/sh files/git_for_devops (main)
