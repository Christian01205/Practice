# Learning Git
- Git is a distributed version control system that tracks changes in any set of computer files, usually used for coordinating work among programmers collaboratively developing source code during software development. Its goals include speed, data integrity, and support for distributed, non-linear workflows (thousands of parallel branches running on different systems).

# Basic Terms

1. Directory -> `Folder`
2. Terminal or Command Line -> `Interface for Text Commands`
3. CLI -> `Command Line Interface`
4. cd -> `Change Directory`
5. Code Editor -> `Word Processor for Writing Code`
6. Repository -> `Project, or the folder/place where  your project is kept`
7. Github -> `A website to host your repositories online`

# Git Commands

- Clone -> `Bring a repository that is hosted somewhere like Github into a folder on your local machine (i.e. VsCode)`
- add -> `Track your files and changes in Git`
- commit -> `Save your files in Git`
- push -> `Upload Git commits to a repo, like Github`
- pull -> `Download changes from remote repo to your local machine, the opposite of push`

## Additional details:
- When adding a `new file` or `creating a new repo` locally (VsCode) you have to use these `certain commands` to have your local machine know where to push the code.
  - First of all, if you have created a new repo, you have to make a file inside it to start making changes.
  - After that, you have to use the command `git init` to initialize an empty git repo which is the `.git`.
  - Now, you can make changes and use the commands written above. The problem is, when using the command `git push` the result would be `fatal` because the local machine could not read from remote repository as the repo and file is created locally.
  - The next step would be, is to create a new repo file in Github, copy the `code link` and use the `git remote add origin (link)` command. 
  - Lastly, you can now use `git push origin main` to push the repo to the remote machine. (You can use `git push -u origin main` so in the future, you only need to write `git push`.)

# Git Branching

[Git-branching-example](/Practice/Screenshot%20(1).png)

- Git branching allows the developers to create and use a separate new branch. This makes the developer able to make code changes that doesn't affect the codes in the `main(default)` branch. 
- You can call the new branches `feature branch/es`. They are used to try out new things before adding the changes in code to the `main branch`.
  -  NOTE: the changes made in `feature branch` can't be viewed or seen in the `main branch` and vice versa.
  -  The `Hot Fix Branch` in the example picture is just an `EXAMPLE` of a `new created branch`.
- After making changes to a file using the `feature branch` you CAN then `merge` it to the `main branch`.

# Commands

1. `git branch` -> used to see the list of your branches. 
```
$ git branch
* main
```
(Note: The `*` before the branch `main` is an IDENTIFIER that tells you which branch you are currently on.)
  
2. `git checkout -b (name-of-the-branch)` -> used to create a new branch.
```
$ git checkout -b test-branch
switched to a new branch 'test-branch'
```
3. `git checkout (name-of-the-branch)` -> used to switch branches. 
```
$ git checkout main
switched to a branch 'master'
```
(Tips: if you have a long branch name, for example: `test-branch-number1`. You can write `git checkout number1` and then press `TAB` it will then automatically writes the full name of the branch.)
   
   4. `git diff (name-of-the-branch)` -> used to compare the `branch` you're currently in and the `new branch` to see the changes that you made in the said `new branch`.
```
/c/git/Practice (main)

$ git diff test-branch
```
  5. `git push -u origin (name-of-the-branch)` -> used to set the remote an upstream for the `new branch` and push the changes made into the `Remote Repository`.
```
$ git push -u origin test-branch
```
(NOTE: By doing this, this command will make a pull request in the `Remote Repository`. If you are collaborating with people from your team, they will be able to review the code, add a comment, ask you to update etc.)

(Tip: After you're done. Naturally, you'll have to delete the `used branch` and start the new process over if you want to not directly make changes in the main branch.)

  6. `git merge (name-of-the-branch)` -> used to directly merge the changes made in the `new branch` to the `main branch`.

```
/c/git/Practice (main)

$ git merge test-branch
```
  7. `git branch -d (name-of-the-branch)` -> used to delete a certain `branch`.

```
$ git branch -d test-branch

Deleted branch test-branch (was ---).
```
