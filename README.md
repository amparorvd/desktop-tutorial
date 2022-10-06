# Welcome to my manual GitHub Desktop!

This is your README. READMEs are where you can communicate what your project is and how to use it.

Write your name on line 6, save it, and then head back to GitHub Desktop.
Git testing project


Initial Setup:

**git config --global user.name "Your name here"**

**git config --global user.email "your_email_here@a.com"**


With these commands you indicate your username (you generally use your first and last name) and email. This configuration is used so that when you make commits in the local repository, they are stored with the reference to yourself.

Two ways to work:

    Work locally, in a repository that I create on my machine.
    Clone a Github repository (or other repository hosting) to bring the complete repository to local and start working with that project.

Create working folder:
To create the files, in a common developer workflow you will use your preferred code editor: Eclipse, Sublime Text, Notepad++, Gedit, etc. As you prefer. Also, of course, you can create your file by command line and edit it if you are on Linux with the well-known Vim or any other text-only interface editor.

I create the Git repository with the "**git init**" command.

Save the files in the repository (commit)

We begin by adding the file or files to a temporary intermediate area called "Index Area" or "Staging Area", which is an area that uses Git where the files that are later going to be committed are saved.

Any file you want to send to the index zone you do it with the "add" command.

**git add filename**

**git status**

send multiple files "."

**git add .**

commit the files from the Index zone to the repository, which is called the "commit"

**git commit -m "message for the commit"**

Then you have to "push" from your local to remote repository with the commands that appear on the Github page

**git remote add origin https://github.com/here-your-repo.git**

**git push -u origin master**
**git push -u origin developer**

You can see the branch you are in at any given time with the command:
git branch


If you haven't committed your project, you'll notice that no branch has been created yet and the branch command doesn't produce any output.

More detailed description of the branches with this other command:

**git show-branch**

To move between branches we use the "git checkout" command followed by the name of the branch we want to be active.

The following command, launched from the "master" branch, allows you to merge it with the branch X
**git merge X**

You can publish a remote branch using the push command, indicating the "-u" option and the name of the branch you want to upload.
**git push -u origin X**

The process to get a branch from the remote repository
**git fetch**

Now we can access it

**git checkout my_remote_branch_downloaded**

The "fork" is one of the common operations with the work in Git and GitHub. It basically serves to create a copy of a repository in your user account. That copied repository will basically be a clone of the repository from which the fork is made, but from then on the fork will live in a different space and can evolve differently, at your own expense.

**git checkout developer**
