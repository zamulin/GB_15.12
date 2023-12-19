# Hint for working with Git

### What is Git?

[Git][1] is a distributed version control system that tracks changes in any set of computer files, used for coordinating work among programmers who are collaboratively developing source code during software developmen.

![markdown logo](https://cdn.iconscout.com/icon/free/png-256/free-git-18-1175219.png)


## [The beginning of the way][2]


The first thing you should do after installing Git is to provide a name and email address. This is important because every commit in Git contains this information, and it is included in the commits you push.
        
>To set the username in the repository, enter the **git config --global user.name "name"** command.

> To configure the mail used by the repository, enter the **git config --global user.email your mail** command.

### Change of editor
You can change the text editor to a more convenient one using the **git config --global core.editor your instal editor** command.

### Colors in Git

Git fully supports colored terminal output, which greatly aids in visually parsing command output quickly and easily.

>To enable automatic highlighting of part of your output, enter the **git config --global color.ui auto** 

>To cancel automatic text selection, enter the **git config --global color.ui false** command.


## Working with data


### Preparing the repository
First, let's create a repository, you need to run the [git init][3.1] command
in the folder with the repository and you will have a repository created
(a hidden folder will appear .git).

### Git add
To add changes to a commit, use the [git add][3.2] command. 
To use the this command write **git add filename"**.

### View repository status
To view the status of the repository, use the [git status][3.3] command. To do this, you need to write git status in the folder with the repository, and you will see whether there were changes in the files or there were none.

### Making commits
In order to create a commit (save), you must execute the appropriate command [git commit][3.4]. It is done like this: **git commit -m "commit"**.

### View commit history
To view commits that have already been made, you will need to be able to see what has already been done using the commit history. To do this, enter [git log][3.5].

> To see the commit log with visualization, enter the **git log --graph** command.


## Working with files


### Show information about files in the index

This command merges the file listing in the index with the actual working directory list, and shows different combinations of the two. To use this command, enter [ls][4.1].

> To see what links are present on the server, enter the **git ls-remote URL** command.

## Move or rename a file

  To rename a file, directory or symbolic link you can use the [git mv current name future name][4.2] command.

## Remove files from the working tree

To remove files at a specified path from the index or from the working tree and index, issue the [git rm name file][4.3] command.

### Looking at the contents of the file
Using the [cat filename][4.4] command you can get information about the content, type and size of objects from a Git repository.

You can determine the type of object in the *objects catalog* automatically and display the result in the appropriate form using the AKU command. **git cat-file -p filename** command.

### Other

* **mkdir "name new directory"** - 
    make directory

* **toch "name new file"** - 
    make empty file

* **cp "name of the copied file" "name new file"** - 
    сopying a file

* **сd "your directory"/** - 
    change way directory

        ~ - start
        .. - on a higher level    


## Working with repositories 


### Cloning a Repository

To clone a remote repository to your local machine, enter the [git clone URL][5.1] command.

### Adding a Remote Repository

 To add a new remote repository, enter the [git remote add name URL][5.2] command.

### Removing and Renaming Remote Repositories

To delete a remote repository, enter the **git remote remove name** command.
To rename a remote repository, enter the **git remote rename old_name new_name** command.

### Information about Remote Repositories:

To display both fetch and push URLs for all remote repositories, issue the **git remote -v** command.
### Find branch

To find out which branches are available and what the name of the current branch is, run [git branch][5.3]. If **--list** is given or no arguments, the current branch will be highlighted in green and marked with a ( * ) sign, the rest will be highlighted in blue and marked with a ( + ) sign.

> To delete another branch, enter the **git branch -d branch_name** command.

> To create another branch, enter the **git branch branch_name** command.

> To show remote branches, enter the **git branch -r** command

> To set up tracking for the current local branch, enter the **git branch --set-upstream-to=remote/branch** command.

### Switch branches

Updates files in the working tree to match the version in the index or specified tree. If no path specification is provided, [git checkout][5.4]  will also update the specified head branch as the current one.

> To move to another branch, enter the **git checkout branch_name** command.

> **git checkout master** will help you check out your local branch.

> To create a local branch that tracks a remote branch, issue the **git checkout -b new_branch remote/branch** command.

### Join two or more development histories together

To include changes from named commits (from the moment their history deviated from the current branch) into the current branch, use the [git merge branch_name][5.5] command.

### Fetching Changes from a Remote Repository

 To retrieve all changes from the specified remote repository, issue the [git fetch name][5.6] command.

 To fetch changes and merge them into the current branch, issue the [git pull name branch][5.7] command.

### Pushing Changes to a Remote Repository

To push changes to a remote repository, issue the [git push <name> <branch>][5.8] command.

> To undo the last push, overwriting the history, enter the **git push <name> --force** command.

### Show changes
To display the difference between any two Git trees, files, or indexes, you can use the [git-diff][5.9] command.

When working with a third-party utility, use the [git-difftool][5.10] command.


# Content
[Introduction](#what-is-git)

[The beginning of the way](#the-beginning-of-the-way)

[Working with data](#working-with-data)

[Working with files](#working-with-files)

[Working with repositories](#working-with-repositories)



 [1]: (https://en.wikipedia.org/wiki/Git)
 [2]: (https://git-scm.com/book/sv/v2/Customizing-Git-Git-Configuration)
 [3.1]: (https://git-scm.com/docs/git-init)
 [3.2]: (https://git-scm.com/docs/git-add)
 [3.3]: (https://git-scm.com/docs/git-status)
 [3.4]: (https://git-scm.com/docs/git-commit)
 [3.5]: (https://git-scm.com/docs/git-log)
 [4.1]: (https://git-scm.com/docs/git-ls-files)
 [4.2]: (https://git-scm.com/docs/git-mv)
 [4.3]: (https://git-scm.com/docs/git-rm)
 [4.4]: (https://git-scm.com/docs/git-cat-file)
 [5.1]: (https://git-scm.com/docs/git-clone)
 [5.2]: (https://git-scm.com/docs/git-remote)
 [5.3]: (https://git-scm.com/docs/git-branch)
 [5.4]: (https://git-scm.com/docs/git-checkout)
 [5.5]: (https://git-scm.com/docs/git-merge)
 [5.6]: (https://git-scm.com/docs/git-fetch)
 [5.7]: (https://git-scm.com/docs/git-pull)
 [5.8]: (https://git-scm.com/docs/git-push)
 [5.9]: (https://git-scm.com/docs/git-diff)
 [5.10]: (https://git-scm.com/docs/git-difftool)
