
# Git Commands Reference

## 1. Basic Setup

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
