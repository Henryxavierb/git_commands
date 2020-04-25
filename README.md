## Git Commands
For most developers starting with git, sometimes it's difficult to write the various commands that the library has. So, i decided share some scripts that may help you on your everyday lite.

### To start a git file:
   ```shell
   git init
   ```

### Show difference in file:
  - Simple changes.
      ```shell
      git diff
      ```

  - Show changes that was selected in stage that will go in next commit.
      ```shell
      git diff --staged
      ```

### To add files in git repository:
  - To a specific file with changes.
      ```shell
      git add name_file
      ```

  - To adding all files with changes.
      ```shell
      git add .
      ```

  - Adding similar files.
      ```shell
      git add *.js
      ```

  - Adding files by folder, analysing the differences.
      ```shell
      git add -P
      ```

    OBS: To divide changes by modifications: Answer: Y

### To give a message to commit:
   ```shell
      git commit -m '...'
   ```

### To update repository:
   ```shell
      git pull origin branch_name
   ```

### To send changes to repository:
   ```shell
      git push origin branch_name
   ```

### To rename the last commit:
   ```shell
      git commit -m '...' --amend
   ```

### To undo last modifications before push:
  - Delete all changes and commit before push. 
   ```shell
      git reset --hard
   ```
  
  - Only delete commits without undo changes. The number is the total commits that you need to undo.  
   ```shell
      git reset --soft HEAD~1
   ```

### To remove a file in "git add .":
  - To remove a only file.
   ```shell
      git reset HEAD -- file_name
   ```

  - To remove all:
   ```shell
      git reset --
   ```

### To show number of commits by users:
   ```shell
      git shortlog -sn
   ```
