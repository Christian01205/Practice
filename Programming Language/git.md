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