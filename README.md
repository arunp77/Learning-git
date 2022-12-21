# **GIT & GITHUB**

This repository contains the step by step for learning GIT and updating GITHUB.

<!-- ![image](https://user-images.githubusercontent.com/15100077/208880325-73824c43-81e1-4be7-b363-b46c6e18567c.png) -->

<img src="https://user-images.githubusercontent.com/15100077/208880325-73824c43-81e1-4be7-b363-b46c6e18567c.png" width="300" height="250">

# **GIT** 
  GIT is a version control system that helps developers track and manage changes to their code. A version control system helps developers store every change they make   to a file at different stages so they and their teammates can retrieve those changes at a later time. 

# **GitHub** 
   GitHub is a web interface where you store your Git repositories and track and manage your changes effectively. It gives access to the code to various
   developers working on the same project. You can make your own changes to a project at the same time as other developers are making theirs.

   If you accidentally mess up some code in your project while making changes, you can easily go back to the previous stage where the mess has not occurred yet.

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


# **Steps to follow**

  a). Create a GitHub account and make a repository at github
  
  b). Next install Git and configure it.

# **Create GitHub account:**
   - Visit [official GitHub website](https://github.com/) and create account
   - ![image](https://user-images.githubusercontent.com/15100077/208904536-b4efeee6-e206-4711-a399-139450e6f7b3.png)

    
# **Starting with GIT**

Here are some steps to follow to get started:

1. **Instalation:** Install Git on your computer. You can download the latest version of Git from the [official website](https://git-scm.com/downloads).

     - **Installing on Linux**
          If you want to install the basic Git tools on Linux via a binary installer, you can generally do so through the package management tool that comes with your
          distribution. If you’re on Fedora (or any closely-related RPM-based distribution, such as RHEL or CentOS), you can use dnf:
     
          `$ sudo dnf install git-all`
     
          If you’re on a Debian-based distribution, such as Ubuntu, try apt:
     
          `$ sudo apt install git-all`
     - **Installing on macOS**
          There are several options for installing Git on macOS. 
          - Homebrew:
          If you don't have homebrew on your mac, install it using:
     
          `$ Install homebrew`
     
          Next use
          
          `$ brew install git`
          - MacPorts: Install MacPorts if you don't already have it, then:
     
          `$ sudo port install git`
     
          - Xcode:
           Apple ships a binary package of Git with [Xcode](https://developer.apple.com/xcode/).
  
     - **Installing on Windows:** 
          Follow the links and steps given at [offical git windows website](https://git-scm.com/download/win) 
    

2. **Configuration:** 
  Set up your Git configuration. This includes setting your username and email address, which will be associated with your commits. You can do this by running the   
  following commands:

     `git config --global user.name "Your Name"`
  
     `git config --global user.email "your_email@example.com"`
      
   Git comes with a default branch of master, so I changed it to be called the main branch by using the 
   
     `git config --global init.default branch main`
     
   command.

3. **Create a new Git repository**
   A repository is a directory that holds all the files related to a project, as well as all the commits made to those files. To create a new repository, navigate to
   the directory where you want to store your project and run the following command:

    `git init`

4. **Add files to the repository:** You can start adding files to your repository by running the following command:

    `git add <filename>`

    You can also add all the files in a directory by running git add ..

5. **Commit your changes** Once you've added files to your repository, you can commit your changes by running the following command:

    `git commit -m "Commit message"`

    The commit message should briefly describe the changes you made.

# **Branching, pulling, and pushing**
   are important concepts in Git that allow you to work on your codebase in a flexible and efficient way. Here's a brief overview of each of these concepts:

  - Branching: Branching allows you to create a separate line of development for your codebase. This is useful when you want to work on a new feature or fix a bug
    without affecting the main branch of your codebase. To create a new branch, you can use the git branch command, followed by the name of the new branch. For
    example: 
    
    `git branch my-new-feature`

  - Pulling: Pulling is the process of retrieving updates from a remote repository and merging them into your local repository. This is useful when you want to 
     incorporate changes made by other team members into your codebase. To pull updates from a remote repository, you can use the git pull command. For example: git
     pull origin master.

  - Pushing: Pushing is the process of sending your local commits to a remote repository. This is useful when you want to share your changes with other team members or
    make them available for deployment. To push your commits to a remote repository, you can use the git push command. For example: git push origin my-new-feature.
## **Common issues with the branching, pulling and pushing**
When you try to merge two branches that have diverged from each other, Git may detect conflicts between the changes made in each branch. To resolve these conflicts, you will need to manually edit the conflicting files to decide which changes to keep and which to discard. Here's a general process for resolving conflicts in Git:

Checkout the branch you want to merge into: Use the git checkout command to switch to the branch that you want to merge the other branch into.

Attempt to merge the branches: Use the git merge command to attempt to merge the branches. If there are conflicts, Git will mark the conflicting lines in the code and will not allow the merge to be completed.

Identify the conflicting files: Use the git status command to see a list of files that contain conflicts. These files will be marked as "unmerged".

Open the conflicting files: Open the conflicting files in a text editor and look for the lines that are marked with conflict markers. These markers will indicate which changes are in conflict.

Decide which changes to keep: Review the conflicting changes and decide which ones you want to keep. You will need to edit the file to remove the conflict markers and keep only the changes that you want to keep.

Mark the conflicts as resolved: Use the git add command to mark the conflicts as resolved. This will stage the modified files for commit.

Commit the merge: Use the git commit command to commit the merge. You will need to provide a commit message to describe the changes that were made.

Push the changes: If you are working with a remote repository, use the git push command to push the merged changes to the remote repository.
# **Important commands**
  Here is a list of some important Git commands that you might find useful when working with Git:

   `git init`       : Initializes a new Git repository in the current directory.

  `git clone`       : Clones an existing Git repository.

   `git add`        : Adds one or more files to the staging area.

   `git commit`     : Commits the staged changes to the repository.

   `git push`       : Pushes the local commits to a remote repository.

   `git pull`       : Pulls updates from a remote repository and merges them into the local repository.

   `git branch`     : Lists, creates, or deletes branches.

   `git checkout`   : Switches to a different branch.

   `git merge`      : Merges changes from one branch into another.

   `git log`        : Shows the commit history for the current branch.

   `git status`     : Shows the status of the repository, including the staging area and the current branch.

   `git diff`       : Shows the differences between the staging area and the most recent commit.


These are the basic steps for getting started with Git. To learn more about Git and how to use it effectively, you can refer to the official documentation (https://git-scm.com/doc) or take an online course or tutorial. There are also many resources available online, such as blogs and forums, where you can ask questions and get help with specific issues.

**Practice using Git:** The best way to learn Git is to use it. Create a new repository on GitHub and try out some of the Git commands you've learned. You can also try working through some of the interactive Git tutorials available on the GitHub Learning Lab (https://lab.github.com/).

**Find additional resources:** There are many resources available for learning Git, including books, online courses, and videos. As you become more comfortable with Git, you can explore these resources to learn more advanced concepts and techniques.

