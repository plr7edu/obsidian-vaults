### What is Gitignore and How to Add it to Your Repo ?

- The `.gitignore` file is a text file that tells Git which files or folders to ignore in a project.

- A local `.gitignore` file is usually placed in the root directory of a project. 

- You can also create a global `.gitignore` file and any entries in that file will be ignored in all of your Git repositories.

- To create a local `.gitignore` file, create a text file and name it `.gitignore` (remember to include the `.` at the beginning). 

- Then edit this file as needed. Each new line should list an additional file or folder that you want Git to ignore.

The entries in this file can also follow a matching pattern.

-   `*` is used as a wildcard match
-   `/` is used to ignore pathnames relative to the `.gitignore` file
-   `#` is used to add comments to a `.gitignore` file

This is an example of what the `.gitignore` file could look like:


```text
# Ignore Mac system files
.DS_store

# Ignore node_modules folder
node_modules

# Ignore all text files
*.txt

# Ignore files related to API keys
.env

# Ignore SASS config files
.sass-cache
```

To add or change your global .gitignore file, run the following command:

```bash
git config --global core.excludesfile ~/.gitignore_global
```

- This will create the file `~/.gitignore_global`. 
- Now you can edit that file the same way as a local `.gitignore` file. 
- All of your Git repositories will ignore the files and folders listed in the global `.gitignore` file.

### How to Untrack Files Previously Committed from New Gitignore

To untrack a _single_ file, ie stop tracking the file but not delete it from the system use:

`git rm --cached filename`

To untrack _every_ file in `.gitignore`:

1. First ****commit**** any outstanding code changes, and then run:

`git rm -r --cached`

2. This removes any changed files from the index(staging area), then run:

`git add .`

3. Commit it:

`git commit -m ".gitignore is now working"`


To undo `git rm --cached filename`, use `git add filename`
