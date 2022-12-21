# **GIT & GITHUB**

This repository contains the step by step for learning GIT and updating GITHUB.

<!-- ![image](https://user-images.githubusercontent.com/15100077/208880325-73824c43-81e1-4be7-b363-b46c6e18567c.png) -->

<img src="https://user-images.githubusercontent.com/15100077/208880325-73824c43-81e1-4be7-b363-b46c6e18567c.png" width="300" height="250">

# **GIT:** GIT is a version control system that helps developers track and manage changes to their code. A version control system helps developers store every change they make to a file at different stages so they and their teammates can retrieve those changes at a later time. 
# **GitHub:** GitHub is a web interface where you store your Git repositories and track and manage your changes effectively. It gives access to the code to various
     developers working on the same project. You can make your own changes to a project at the same time as other developers are making theirs.

     If you accidentally mess up some code in your project while making changes, you can easily go back to the previous stage where the mess has not occurred yet.

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


Here are some steps to follow to get started:

1. Install Git on your computer. You can download the latest version of Git from the [official website](https://git-scm.com/downloads).

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
    

2. Set up your Git configuration. This includes setting your username and email address, which will be associated with your commits. You can do this by running the following commands:

git config --global user.name "Your Name"
git config --global user.email "your_email@example.com"


3. Create a new Git repository. A repository is a directory that holds all the files related to a project, as well as all the commits made to those files. To create a new repository, navigate to the directory where you want to store your project and run the following command:

git init

4. Add files to the repository. You can start adding files to your repository by running the following command:

git add <filename>

You can also add all the files in a directory by running git add ..

5. Commit your changes. Once you've added files to your repository, you can commit your changes by running the following command:

git commit -m "Commit message"

The commit message should briefly describe the changes you made.

These are the basic steps for getting started with Git. To learn more about Git and how to use it effectively, you can refer to the official documentation (https://git-scm.com/doc) or take an online course or tutorial. There are also many resources available online, such as blogs and forums, where you can ask questions and get help with specific issues

