# HRI-20069: Introduction to S/W developmental tools & perception technologies 

Linux Laptop required!!!

## Week 2: Git (Version Control)

### Install git & sign up for github.com
In Ubuntu 16.04, git is already included, but for the other OS please refer to https://git-scm.com

  * References:
    * https://git-scm.com/book/en/v2
    * https://opentutorials.org/course/2708

### First-Time Git Setup
  * Configure the git
    ** Your Identity
    ```
    $ git config --global user.email "you@example.com”  
    $ git config --global user.name "Your Name"
    ```   
    ** Your Editor
    ```
    $ git config --global push.default simple
    $ git config --global core.editor vi           # Using vi editor for git
    ``` 
    ** Checking Your Settings
    ```
    $ git config -l
    user.name=John Doe
    user.email=johndoe@example.com
    color.status=auto
    color.branch=auto
    color.interactive=auto
    color.diff=auto
    ...
    ```

### Git Basics
Git has three main states that your files can reside in: committed, modified, and staged:

    * Committed means that the data is safely stored in your local database.

    * Modified means that you have changed the file but have not committed it to your database yet.

    * Staged means that you have marked a modified file in its current version to go into your next commit snapshot.

This leads us to the three main sections of a Git project: the Git directory, the working tree, and the staging area.

![pic-W2-001](./assets/images/areas.png)

You typically obtain a Git repository in one of two ways:
  1. Initializing a repository in an existing directory, or
  2. Cloning an existing Git repository from elsewhere.
In either case, you end up with a Git repository on your local machine, ready for work.

#### Initializing a Repository in an Existing Directory

  * First, make a folder (a git repository)
  ```
    $ mkdir hri-20069-git
  ```

  * Initialize the repository,
  ```
    $ cd hri-20069-git
    $ git init
  ```

  * Let's make several files as
  ``` 
    $ echo "test1: v01" > test1.txt
    $ echo "test2: v01" > test2.txt
  ```
  
  * Add all files to git stage
  ```
    $ git add .
  ```
  
  * Commit the staged files
  ```
    $ git commit -m 'v01'
  ```

#### Cloning an Existing Repository
You clone a repository with git clone <url>. For example, if you want to clone the Git for this class called HRI-20069 , you can do so like this:
 
  ```
    $ git clone https://github.com/cjs0818/HRI-20069
  ```
If you want to clone the repository into a directory named something other than HRI-20069, you can specify that as the next command-line option:

  ```
    $ git clone https://github.com/cjs0818/HRI-20069 myHRI
  ```

#### Recording Changes to the Repository
As you edit files, Git sees them as modified, because you’ve changed them since your last commit. As you work, you selectively stage these modified files and then commit all those staged changes, and the cycle repeats.

![pic-W2-002](./assets/images/lifecycle.png)

#### Checking the Status of Your Files
  ```
    $ git status
    On branch master
    Your branch is up-to-date with 'origin/master'.
    nothing to commit, working directory clean
  ```

### Git Branching

### Git on the Server

### Distributed Git

### GitHub

### Git Tools

### Version control for Dockerfile using git
  * ros-kinetic-core
  * ros-kinetic-base
  * ...
  * ros-kinetic-desktop-full
