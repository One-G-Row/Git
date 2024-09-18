# Git Commands Guide

## To initialize git

```
git init
```

## Stage file

```
git add <filename>
```

## To check status of the file

```
git status
```

## To remove staged file/unstage file

```
git rm –cached <file name>
```

## To check commit history logs

```
git log
```

## To escape git log

Press `q`

## To condense logs to one line

```
git log –oneline
```

## To checkout a commit

1. Run `git log –oneline`
2. Copy the code for the specific commit you want to go to
3. Enter:

```
git checkout <commitcode>
```

## To go back to the last commit/last update

```
git checkout main
```

## To undo a commit/remove a file safely

1. Check history by running `git log –oneline`
2. Copy code of the commit you want to revert
3. Run:

```
git revert <commitcode>
```

## To create a branch

```
git branch <filename>
```

## To check all available branches and which one you are working on

```
git branch -a
```

## To create a branch and checkout to the branch at the same time

```
git checkout -b <filename>
```

## To switch to another branch

```
git checkout <filename>
```

## To delete a branch

```
git branch -D <filename>
```

## To merge branches to main

1. Checkout to `main`:

```
git checkout main
```

2. Merge branch:

```
git merge <branchname>
```

## To push files to remote repo

```
git push <repo url> main
```

## To give repo url an alias

1. Add remote origin:

```
git remote add origin <repo url>
```

2. Push using alias:

```
git push origin main
```

## To pull unrelated histories created separately

```
git pull <repo name> –allow-unrelated-histories
```

## Collaborating with others

### If there are changes in the remote repo and you want to pull to the local repo:

```
git pull origin main
```

### To push changes to remote repo

#### Option 1 (while working on a feature/alternative branch):

1. Add changes:

```
git add .
```

2. Commit changes:

```
git commit -m "changes text"
```

3. Push to branch:

```
git push origin <branch name>
```

4. On GitHub, click the "Compare & Pull Request" popup.
5. Create a pull request.
6. If there are conflicts, resolve them.
7. Merge the pull request.
8. Confirm merge.
9. Optionally, delete the branch.

#### Option 2 (while working on a feature/alternative branch):

1. Add changes:

```
git add .
```

2. Commit changes:

```
git commit -m "changes made text"
```

3. Push to branch:

```
git push origin <feature branch name>
```

4. Checkout to `main`:

```
git checkout main
```

5. Merge the feature branch:

```
git merge <feature branch name>
```

6. Resolve conflicts.
7. Push changes to main:

```
git push origin main
```

## To work on something else

1. Checkout to `main`:

```
git checkout main
```

2. Pull changes from `main`:

```
git pull origin main
```

3. Optionally, create a new branch:

```
git checkout <branch name>
```

4. Add changes:

```
git add .
```

5. Commit changes:

```
git commit -m "commit message"
```

6. Push to branch:

```
git push origin <branch name>
```

7. Compare and pull.
8. Merge pull request.
9. Confirm merge.
