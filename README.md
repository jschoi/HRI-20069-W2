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
You typically obtain a Git repository in one of two ways:
  1. You can take a local directory that is currently not under version control, and turn it into a Git repository, or
  2. You can clone an existing Git repository from elsewhere.
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



### Version control for Dockerfile using git
  * ros-kinetic-core
  * ros-kinetic-base
  * ...
  * ros-kinetic-desktop-full
