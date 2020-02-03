---
layout: page
title: "Environment Setup for CS 675 Labs"
permalink: /env_setup.html
---

## Introduction

The following instructions describe how to create a Git source code
repository in the student.cs computing environment.

We will be using Mason GitLab for the rest of our CS 675 labs (i.e., [Lab 1](https://git.gmu.edu/cs675-spring20-labs/lab1) and Lab 2). 
The URL for the lab GitLab repository is [https://git.gmu.edu/cs675-spring20-labs](https://git.gmu.edu/cs675-spring20-labs). 

> **NOTE**: Don’t clone the git repo directly; instead, as described
in the GitLab Setup instructions below, first fork that repo into your own
**private** repo on our Mason GitLab server, then clone from there.
You’ll commit you changes locally and push them to your private
GitLab repo for grading.

## Step 1: Create a GitLab Repo

First, you will need to login to <a
href="https://git.gmu.edu/users/sign_in">GitLab</a> by clicking
`Sign in with: GMU Login`. Username and Password never work
for some reason.

**Important:**
For both Lab 1 and Lab 2, make sure you fork
the original project GitLab repositories and then change the permission
of the project to **Private**.
After the repository has been forked, go to your forked project, from
`Settings`, go to `General`, from there change `Visibility` level to 
`Private`.


## Step 2: Clone Your Private GitLab Repo

Before cloning your GitLab repo to your student.cs computing environment,
you will need to first create an RSA SSH key by typing:

```bash
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
Then, create a new directory called <tt>cs675-spring20-labs</tt> under `$HOME/go/src` directory
(of your Linux machine, or an EC2 virtual machine box, or whatever you have), 
`cd` to your working directory where you are supposed to put your os161 source code,
and clone your created GitLab repo on to your server:

```bash
% cd 
% mkdir -p go/src/cs675-spring20-labs
% cd go/src/cs675-spring20-labs 
% git clone git@git.gmu.edu:cs675-spring20-labs/lab1.git
```


## Step 3: Check in Your Updates

Now, check in the source code which you have already modified:
Git allows you to keep track of the changes you make to the code. For
example, if you want to checkpoint your progress, you can
**commit** your changes by running:


```bash
% git add *
% git commit -m 'partial solution to lab 1'
% git push  
```

You should do this early and often!  
If you are checking in for **the first time** on an empty repo (which is your case here),
you should run:

```bash
% git push -u origin master
```

Please let me (the instructor) know that you've gotten this far in the lab, by pushing a tag to GitLab.

```bash
$ git tag -a -m "i got git and cloned the labs" gotgit
$ git push origin gotgit
```

As you complete parts of the labs (and begin future labs), it is a
good practice to push tags. You should also be committing and pushing
your progress regularly.


## Tools related to Go

There are many commonly used tools in the Go ecosystem. The three most useful starting out are:
 <a href="https://golang.org/cmd/gofmt/">Go fmt</a> and <a
href="https://golang.org/cmd/vet/">Go vet</a>, which are built-ins,
and <a href="https://github.com/golang/lint">Golint</a>.

## Go Editors

For those of you in touch with your systems side (this *is*
Distributed Systems, after all), there are quite a few resources for
Go development in both <a
href="https://github.com/dominikh/go-mode.el">emacs</a> (additional information available 
<a href="http://dominik.honnef.co/posts/2013/03/emacs-go-1/">here</a>) and <a href="https://github.com/fatih/vim-go">vim</a> (additional resources 
<a href="http://farazdagi.com/blog/2015/vim-as-golang-ide/">here</a>).

## Go's Coding Style

All of the code you turn in for this course should have good style.
Make sure that your code has proper indentation, descriptive comments,
and a comment header at the beginning of each file, which includes
your name, userid, and a description of the file.

It is recommended to use the standard tools `gofmt` and `go vet`. 
You can also use the <a href="https://github.com/qiniu/checkstyle">Go Checkstyle</a> tool for
advice on how to improve your code's style. It would also be advisable to
produce code that complies with <a href="https://github.com/golang/lint">Golint</a> where possible. 


## Stepping into Lab 1

Now it's time to go to the [lab1](https://git.gmu.edu/cs675-spring20-labs/lab1) folder to begin your adventure!

