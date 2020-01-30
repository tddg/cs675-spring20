---
layout: page
title: "GitLab Setup for CS 675 Labs"
permalink: /gitlab_setup.html
---

## Introduction

The following instructions describe how to create a Git source code
repository in the student.cs computing environment.

We will be using Mason GitLab for the rest of our CS 675 labs (i.e., [Lab 1](https://git.gmu.edu/cs675-spring20-labs/lab1) and Lab 2). 

## Step 1: Create a GitLab Repo

First, you will need to login to <a
href="https://git.gmu.edu/users/sign_in">GitLab</a> by clicking
`Sign in with: GMU Login`. Username and Password never work
for some reason.

**Important:**
For both Lab 1 and Lab 2, make sure you fork
the original project GitLab repositories and then change the permission
of the project to **Private**.



## Step 2: Clone Your Private GitLab Repo

Before cloning your GitLab repo to your student.cs computing environment,
you will need to first create an RSA SSH key by typing:

```
% ssh-keygen -t rsa -C "your_email_addr"
```

Or you can simply follow 
<a href="https://git.gmu.edu/help/ssh/README#generating-a-new-ssh-key-pair">this tutorial</a>.

Then, add an SSH key to your GitLab account by following 
<a href="https://git.gmu.edu/help/ssh/README#adding-an-ssh-key-to-your-gitlab-account">these instructions</a>.

<a href="https://git.gmu.edu/help/ssh/README#adding-an-ssh-key-to-your-gitlab-account">Test</a> if
the SSH-based access has been successfully set. 

Click on the **Clone** button at the right-top corner of your GitLab repo's webpage,
copy the string under **Clone with SSH** to clipboard.
Then, create a new directory called <tt>cs675-spring20-labs</tt> under your `$HOME` directory
(of your Linux machine, Zeus, or an EC2 virtual machine box, or whatever you have), 
`cd` to your working directory where you are supposed to put your os161 source code,
and clone your created GitLab repo on to your server:

```
% mkdir $HOME/cs675-spring20-labs
% cd $HOME/cs675-spring20-labs 
% git clone git@git.gmu.edu:cs675-spring20-labs/lab1.git
```


## Step 3: Check in Your Updates

Now, check in the source code which you have already modified:

```
% git add *
% git commit -m "[some meaning message]" 
% git push  
```

If you are checking in for the first time on an empty repo (which is your case here),
you should run:

```
% git push -u origin master
```

Instead of

```
% git push
```



