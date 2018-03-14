# HRI-20069: Introduction to S/W developmental tools & perception technologies 

Linux Laptop required!!!

## Week 2: Git (Version Control)

### Install git & sign up for github.com
In Ubuntu 16.04, git is already included, but for the other OS please refer to https://git-scm.com

  * References:
    * https://git-scm.com/book/en/v2
    * https://opentutorials.org/course/2708

  * First, make a folder (a git repository)
```
    $ mkdir hri-20069-git
```

  * Initialize the repository,
```
    $ cd hri-20069-git
    $ git init
```

  * Configure the git
```
    $ git config --global user.email "you@example.com”  
    $ git config --global user.name "Your Name"
    
    $ git config --global push.default simple
    $ git config --global core.editor vi           # Using vi editor for git
```

### Version control for Dockerfile using git
  * ros-kinetic-core
  * ros-kinetic-base
  * ...
  * ros-kinetic-desktop-full
