# **GIT & GITHUB**

<!-- ![image](https://user-images.githubusercontent.com/15100077/208880325-73824c43-81e1-4be7-b363-b46c6e18567c.png)
<img src="https://user-images.githubusercontent.com/15100077/208880325-73824c43-81e1-4be7-b363-b46c6e18567c.png" width="300" height="200"> -->

![image](https://user-images.githubusercontent.com/15100077/208984391-c45a0f71-2e44-433c-8500-8a3797cd3102.png)

# **GIT** 
  GIT is a version control system that helps developers track and manage changes to their code. A version control system helps developers store every change they make   to a file at different stages so they and their teammates can retrieve those changes at a later time. 

# **GitHub** 
   GitHub is a web interface where you store your Git repositories and track and manage your changes effectively. It gives access to the code to various
   developers working on the same project. You can make your own changes to a project at the same time as other developers are making theirs.

   If you accidentally mess up some code in your project while making changes, you can easily go back to the previous stage where the mess has not occurred yet.
   
   ![image](https://user-images.githubusercontent.com/15100077/208984601-6fb89bf1-cf0b-45d7-be62-23d215d4fb98.png)


# **Version control**

   There are three types of version control systems, which are:

- **Local Version Control Systems:** This is a type of version control system that is very common and simple to use. But this method is quite prone to errors and
    attacks because the files are being stored in your local system.
    This means that you might lose the system file or accidentally forget the directory/folder of the file you are working (and then write in another directory).
- **Centralized Version Control Systems:** In this type of version control, a server act as a repository that stores each version of the code. The CVCS helps different     developers collaborate together.
    
    Despite the helpful collaboration and communication between developers, if a server goes down for few seconds or gets corrupted, there's the chance you'll lose
    your work. Unfortunately, this is a very big problem with the CVCS.
    
    In CVCS, only a few developers can work together on a project.
- **stributed Version Control Systems:** This is the latest and most commonly used type of version control system these days.

     In a DVCS all developers have a full back up (clone) of all the data in the server. This means that whenever the server is down or faulty, you can still work on
     your project and you can copy or back up your repositories to the server to restore them.

     When you're using a DVCS, many developers can work together on a project. One popular DVCS is Git, which we'll talk about more now.


# How to start (if you have already git installed and if you have already a github account)
1. When you have already a Github repository and you want to update a version of the file on the Github
    - Create a repository on GitHub.
    - Next clone the repository in your system, by using command
        ```
        git clone "Github HTTP clone link like https://github.com/username/XYZ.git"
        ```
    - Then open VSCODE editor and find "Open folder option" and go to the folder where you have cloned the github repository. When you are inside the Github repository   
      local folder, you can now create any file and push it to online GitHub repository. When you clone your repository to your local respository, you also get a file    `.git`, which connects your local repository to the online Github repository. 
    - After creating your file (let's say, you have created a file named `mycode.py`), check git status, by
      ```
      git status
      ```
      In output, you will find list of the files changed into your local repository. Now you need to `add` it to the staging area to track the changed that you make.
      Everytime you make a change in the file, it will create a local id. By this id, you can track the changes in future.
    - Use following command it add it to the staging area:
      ```
      git add .
      ```
      If you want to just add a specific file, then use:
      ```
      git add "your file with extension"
      ```
    - After this, you need to commit the staged changes to the repository by
      ```
      git commit -m "Commit message" -m "Commit message description"
      ```
    - Now it's time to push the commited files to the github repository.
      ```
      git push
      ```
      or to push a specific file, use
      ```
      git push "file name with extension"
      ```

2. When you first create file locally and you want to upload and update the file to a Github repository
    - Follow following steps.
    - First create a local repository. For example lets create a local repository, named "demo-repo" and create a local file inside the local repository 
      (let's the creted file is "index.py"). Then go the the created repository via the VSCODE terminal. Now you need to change the created local repository "demo-repo" 
      into a git repostory, you need to initiat first. To do this, use following command
      ```
      git init
      ```
    - Now you can check the status of the newly created local git repository by
      ```
      git status
      ```
    - Now you need to add the newly created "index.py" file to the stagging area. To do this
      ```
      git add index.py
      ```
    - After this, you need to commit the changes. 
      ```
      git commit -m "message" -m "description on the message"
      ```
    - Next when you try to push the locally created git repository to GitHub, it will show a error like 
      ```fatal: origin doesnot appear to be repository 
      fatal: couldnot read from remote repository

      Please make sure that you have the correct access rights and the repository exists.
      ```
    - So to get the acess rights, first create a empty repository on the GitHub website. Now copy the quick setup HTTPs link (something like 
       https://github.com/username/XYZ.git) for the newly created GitHub repsotory. Next go to the VSCODE terminal, where you where working and creating the
       local repository and in the terminal type
       ```
       git remote add origin https://github.com/username/XYZ.git
       ```
       here remote is used to add a reference to the remote repository "origin" on GitHub via the https link.
    - Now you can check the added reference to the remote repository to the github by
      ```
      git remote -v
      ```
    - Now to push the local commits to the Github by using upstream command
      ```
      git push -u origin master
      ```
      here sometimes named as main. 
      
---
> **What is repository:** A repository contains a directory named `.git`, where git keeps all of its metadata for the repository. The content of the `.git` directory is private to git.
---

Now, if you don't have git installed in your system and you don't have a github account, then go ahead to the next section.

# Let's start with installing Git and creating a GitHub account

  a). Create a GitHub account and make a repository at github
  
  b). Next install Git and configure it.

## **Create GitHub account:**
   - Visit [official GitHub website](https://github.com/) and create account
      
     ![image](https://user-images.githubusercontent.com/15100077/208905059-2565eb30-95a2-44cd-b6a4-944d7927b0f8.png)
     
   - Enter your email id 
       
      ![image](https://user-images.githubusercontent.com/15100077/208906231-10b1d922-6520-4ab4-a5a0-57d01105d190.png)
    
      here, follow the steps on display and create your account.
   - During the account creation, it may be asked about specific features, you are interested in as
    
      ![image](https://user-images.githubusercontent.com/15100077/208907825-282e183f-d20c-41c5-8316-515f50d57869.png) 
      
      then choose whichever is suitable for you. For a starter, you should choose collaborative coding.
   - Next choose "Continue for free" option, if you just want to learn as a bigginer.
   - You will be taken to your home dashboard. 
    
     ![image](https://user-images.githubusercontent.com/15100077/208909141-53088dc0-abb3-4235-a058-2d12a6000e7b.png)

   - Now, there are two options two create a repository: First one is just click on "_create repository_" and second one is by clicking "*New repository*", which is
     inside the `+` symbol at the top right corner.
   - Now enter the repository name and let other options as it is and then click "_Create repository_"

      ![image](https://user-images.githubusercontent.com/15100077/208909817-f73ad2b4-bee5-4478-b96a-abd0c4a4ab4f.png)

   - Next you will have following view of your own repository on GitHub:
    
      ![image](https://user-images.githubusercontent.com/15100077/208910659-112748fc-a665-4c1c-8af2-ae9cb7124fb1.png)

   - You can start with your repository now. To create a file, click on 'Create a new file'.
       

    
# **Starting with GIT**

Here are some steps to follow to get started:

1. **Instalation:** Install Git on your computer. You can download the latest version of Git from the [official website](https://git-scm.com/downloads).

    - **Installing on Linux**
     If you want to install the basic Git tools on Linux via a binary installer, you can generally do so through the package management tool that comes with your
     distribution. If you’re on Fedora (or any closely-related RPM-based distribution, such as RHEL or CentOS), you can use dnf:
       ```
       sudo dnf install git-all
       ```

      If you’re on a Debian-based distribution, such as Ubuntu, try apt:
       ```
       sudo apt install git-all
       ```

    - **Installing on macOS**

      There are several options for installing Git on macOS. 
      - Homebrew:
        If you don't have homebrew on your mac, install it using:
      
        ```  
        Install homebrew
        ```

        Next use

        ```
        brew install git
        ```
           
      - MacPorts: Install MacPorts if you don't already have it, then 
        ```
        sudo port install git
        ```
      
      - Xcode 

         Apple ships a binary package of Git with [Xcode](https://developer.apple.com/xcode/).
  
     - **Installing on Windows:** 
     
         Follow the links and steps given at [offical git windows website](https://git-scm.com/download/win) 
    

2. **Configuration:** 
    Set up your Git configuration. This includes setting your username and email address, which will be associated with your commits. You can do this by running the
    following commands:
     ```
     git config --global user.name "Your Name"
     ```
     ```
     git config --global user.email "your_email@example.com"
     ``` 
    Git comes with a default branch with name "master", so I changed it to be called the main branch by using the 
     ```
     git config --global init.default branch main
     ```
    command.

3. **Create a new Git repository**
    A repository is a directory that holds all the files related to a project, as well as all the commits made to those files. To create a new repository, navigate to
    the directory where you want to store your project and run the following command:
     ```
     git init
     ```
4. **Add files to the repository:** You can start adding files to your repository by running the following command:
     ```
     git add <filename>
     ```
    You can also add all the files in a directory by running `git add ..`

5. **Commit your changes** Once you've added files to your repository, you can commit your changes by running the following command:
    ```
    git commit -m "Commit message" -m "Commit message description"
    ```
    The commit message should briefly describe the changes you made.



These are the basic steps for getting started with Git. To learn more about Git and how to use it effectively, you can refer to the official documentation (https://git-scm.com/doc) or take an online course or tutorial. There are also many resources available online, such as blogs and forums, where you can ask questions and get help with specific issues.

**Practice using Git:** The best way to learn Git is to use it. Create a new repository on GitHub and try out some of the Git commands you've learned. You can also try working through some of the interactive Git tutorials available on the GitHub Learning Lab (https://lab.github.com/).


# Summary 

## Set up

`git config --global user.name "User Name"` (Here your user name)

`git config --global user.email "email@email.com"` (Here provide your GitHub user email id)

## Create a New Project:
- Open your terminal 
- `mkdir XYZ` (Create a directory to work on a project named 'XYZ')
- `cd XYZ` (After creting the directory, go to the directory)
- `git init` (initialise empty git repo in my folder (based on path) aka .git folder)
- `ls -la` (check my folder)

## Check status:

- `git status` (To check the current status. Here all the message on the modification of the code will appear.)
- `git help <command>` Help for each command, for example if want to know about 'commit', just type: `git help commit`.

## Add files

- `git add .` = add all on current branch. Basically modifications done in all files will be added to your current branch. For branches, this also works.
- `git add -p <param=file>` = add part of file to staging area, ask for each change (if no param => all files) so we have more control and cleaner commits. 
    After any `git add`, we need a `git commit`, either a file or a pattern (e.g. *.txt)

## Delete a file

- `git rm <filename>` = deletes a file, updates git and then commit!

- `git rm --cached <filename>"` = delete a previously tracked file

## Move a file

- `git mv <old path> <new path>` should be followed by:
- `git rm <old path>`
- `git add <new path>`

## Check difference

- `git diff` = displays what will be added if i `git add .`, so what changed in the folder and hasn't been updated yet
- `git diff <filename>` = displays the alterations of a file (the modified and the commited versions of it)
- `git diff --staged` = displays what has already been added and thus what changed will be recorded
- `git diff HEAD` = displays changes since last commit

## Display history

- `git-log` = displays the history, the chronologival order of commits (based on their IDs), who did them, what was their description
- `git show <id>` = displays what the commit did = git log + git diff

## Make an alias

- `git config --global alias.<aliasname> "command(s)"`
- for example:
  `it config --global alias.lg "log --color --graph --pretty=format: '%(red%h%(green(%cr)%((bold blue)<%an>%(reset' --abbrev -commit"`
  `it config --list`- displays our aliases
  
## Make archive

- `git archive --format=zip -o latest.zip HEAD`

## Revert to old commit

- `git log`
- `git checkout <commit hex id>`

## Cancel not staged changes

- `git checkout` = it copies staging area (usually last commit) to out working copy

## Reset
- `git reset` - remove all that exists in my staging area by copying them from the most recent commit (basically undoes git add)

## Copy a commit to another branch

- `git cherry-pick <commit>` = we copy a commit from a point of the graph, we put it on active branch (therefore creating a copy of the selected commit) - new ID, same changes and description!

## Copy changes to new commit

- `git revert <commit>` = inverted add/deletes etc. It cancels the commit that has already happened.

## Tags

-  `git tag -a <tag>` = adds tag to last commit of current branch
-  `git tag -a <tag> <commit>` = add tag to selected commit
-  `git tag` = shows all tags in repo
-  `git tag -d <tag>` = deletes a tag

## Publish tags

- `git push <remote> <tag>` = publishes tag in remote git fetch --tags <remote> = brings all tags from remote

## Serial list of changes
  - `git reflog` = all the changes
  - `git reflog <branch>` = changes on our branch
  - `git reflog --date=relative` = displays changes relative to time


  
# **Important commands**
  
  Here is a list of some important Git commands that you might find useful when working with Git:
  
  | Command        | Explanation                                                                           |
  |----------------|---------------------------------------------------------------------------------------|
  | `git init`     | Initializes a new Git repository in the current directory                             |
  | `git clone`    | Clones an existing Git repository                                                     |
  | `git add`      | Adds one or more files to the staging area                                            |
  | `git commit`   | Commits the staged changes to the repository                                          |
  | `git push`     | Pushes the local commits to a remote repository                                       |
  | `git pull`     | Pulls updates from a remote repository and merges them into the local repository      |
  | `git branch`   | Lists, creates, or deletes branches                                                   |
  | `git checkout` | Switches to a different branch                                                        |
  | `git merge`    | Merges changes from one branch into another                                           |
  | `git log`      | Shows the commit history for the current branch                                       |
  | `git status`   | Shows the status of the repository, including the staging area and the current branch |
  | `git diff`     | Shows the differences between the staging area and the most recent commit             |
  
  
# **Find additional resources:** 

  There are many resources available for learning Git, including books, online courses, and videos. As you become more comfortable with Git, you can explore these resources to learn more advanced concepts and techniques.

1. [GitHub Training](https://githubtraining.github.io/training-manual/#/02_getting_started)
2. [Github documentation](https://docs.github.com/en)
3. [A video reference](https://youtube.com/watch?v=RGOj5yH7evk&feature=shares)
4. [Git commands](https://gist.github.com/ZapDos7/9d2d536da77ad1448ab88511034ca672)
5. [Basic writing and formatting syntax](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax#links)



