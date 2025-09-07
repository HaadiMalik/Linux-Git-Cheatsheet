# Linux Commands

- "$ cat [file_name]"
    - opens [file_name] to view contents in the terminal
    - can be modified to join, copy, append and create files among other things

<br>

- "$ cd [path/to/dir]"
    - change directories to [path/to/dir]

<br>

- "$ ls"
    - list all the files (not hidden) within the current directory

<br>

- "$ mkdir [new_folder]"
    - create [new_folder] in the current directory


<br>

- "$ mv [file_name] [destination_name]"
    - move [file_name] location to [destination_name]
    - can replace [file_name] with [folder_name]

<br>

- "$ pwd"
    - print working (current) directory

<br>

- "$ rm [flags] [file_name]"
    - remove [file_name] or [folder_name] ([folder_name] must be empty first)
    - use "$ rm -r [folder_name]" to remove [folder_name] and all contents within


<br>

- "$ touch [file_name(s)]"
    - create empty file(s). can do multiple files at once, with a space between each file name
    - if [file_name] already exists, updates access and modification timestamps. no other data is changed

<br>

# Git Commands


- "$ git add [file(s)]"
    - add [file(s)] to the stage, ready forr a commit
    - use "$ git add ." to add all new/changed files in the current directory to the stage

<br>


- "$ git branch [branch_name]"
    - use without [branch_name] for a list of branches. the active branch will be marked with *
    - use with [branch_name] to create a new branch at the current name
    - closely related to "$ git checkout -b [branch_name]" and "$ git switch -c [branch_name]"

<br>

- "$ git clone [online_repo_url]"
    - clone an online repository for local use

<br>

- "$ git commit -m 'message' "
    - commit stage content with a message (don't have to push immediately, now a part of commit history)
    - entering just "$ git commiit" opens a text editor for the user to write a commit message
    - can use single or double quotes for message

<br>

- "$ git init"
    - initialize an existing local directory as a git repository

<br>

- "$ git merge [branch_name]"
    - finds the latest common commit between the current branch and [branch_name]
    - if there are no conflicts, it merges the two and creates a merge commit
    - with conflicts, a text eeditor is opened for you to resolve

<br>

- "$ git pull"
    - take the changes made to the latest version of the online repository and pull to the local level
    - only applies to current branch. needs to be done seperately for each branch

<br>

- "$ git push"
    - push all commits in the local repository branch to the online repository branch
    - for the first commit for each branch in a local development environment, "$ git push -u origin [branch_name]" is needed
        - all subsequent commits only need "$ git push", whether or not branches are switched