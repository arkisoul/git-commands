# Git Basics

## Create a new git repository
`git init`

## Git config
- `git config --global --edit` edits global config file
- `git config --local --edit` edits local config file

## Git areas
- Working Area
- Staging Area
- Stash Area

## Git add
Add file(s) from working area to staging area
```
git add file
git add file1 file2 filen
git add .
git add -a
```

## Git commit
Create a commit with the staged file(s)
```
    git commit // opens an editor to write the commit message
    git commit -m "Commit Message goes here" // commit with the provided inline commit message
```

## Working with remote repository
- Create a github account if you don't have one
- Create a github repository
- Add that github repository as a remote repo to your local repo
    ```
        git remote add <remote_name> <remote_repo_url>
   ```

## Git stash
- Creates a temporary commit
- Move files from the working tree to the stash tree/area. Making working tree clean.
- Commands
    `git stash` to create a new stash
    `git stash apply [<stash_id>]` to apply the stash to the current working tree
    `git stash pop [<stash_id>]` to apply the stash to the current working tree then drop it
    `git stash show <stash_id>` to show the summary of changes/files saved in the stash
    `git stash drop <stash_id>` to drop the stash