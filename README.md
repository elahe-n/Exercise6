# Questions

## Introduction
Use this document as a starting point for the Class 6 exercise. Please note that these questions will test your knowledge of both the Git CLI and the command line in general.

## Instructions
- Start by creating a new folder and initializing it as a Git repository.
- Copy this file and its contents into your new repository and commit. The copied file should also be named `README.md`.
- Answer the questions below. Introduce each answer as a separate commit.
- Push the resulting repository to your personal GitHub account.
- See the class page for additional submission instructions.

## Questions
1. Assuming that you aren't sure whether you're currently inside of a Git repository, write the command (or commands) that will give you this information.
A:ls -a (If we're currently inside of a Git repository folder, there should be a hidden folder named .git)
B:git status (If we're currently inside of a folder which itself or one of its parents is git repository by running git commad with any sub commands except help, we will get a related and meaninnful response like "On branch master. nothing to commit, working tree clean". Otherwise, we will face to this response: "fatal: not a git repository (or any of the parent directories): .git")


2. Assuming that you are currently within a Git repository, write the command (or commands) that will create a new file named 'hello-world.txt' then stage and commit it.
touch hello-world.txt
git add hello-world.txt
git commit hello-world.txt -m "hello-world.txt file has been created" 
Or 
git commit -m "hello-world.txt file has been created" (Since we stageed just hello-world.txt file, so there is no need to mention the name of the file)


3. Assuming that you are currently within a Git repository that contains a file named 'README.md', write the command (or commands) that will display any uncommitted changes made to this file.
git diff README.md 

4. Assuming that you are currently within a Git repository that includes several commits, write the command (or commands) that will display the changes from the commit with the ID of abc123.
git show abc123 

5. Assuming that you are currently within a Git repository that includes multiple commits, write the command (or commands) that will display the IDs and commit messages for the 3 most recent commits.
git log -n 3 --oneline