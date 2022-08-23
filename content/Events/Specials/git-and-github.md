---
title: "Git and Github Session"
date: 21 May 2022, 06:00:00 PM IST
draft: false
description: "git and github session"
icon: "https://i.imgur.com/wdMPUpw.jpg"
background: "https://imgur.com/4fey1Kk.jpg"
---

# Event Details:

### Hosts:

#### [Saurav Pati](https://www.linkedin.com/in/oyesaurav/)

#### [Piyush Mishra](https://www.linkedin.com/in/piyushmishra965/)

#### [Shubhasai Mohapatra](https://www.linkedin.com/in/shubhasai-mohapatra/)

### Date: 21 May, 2022

## Topics Covered:

- Introduction to Git
- Hands on training on Git
- Importance of Git and its Visualization
- Introduction to GitHub
- Detailed training on GitHub
- Introduction to Open Source
- Details on "How to contribute to a project?"

## Most Used Commands in Git:

- Sets up Git with your name

  `git config --global user.name "<Your-Full-Name>"`

- Sets up Git with your email

  `git config --global user.email "<your-email-address>"`

- To create/inialize a new Git repository

  `git init `

- To know the state of our repository as seen by Git

  `git status`

- To move files from the Working Directory to the Staging Index

  `git add <file1> <file2> … <fileN>`

  To add all the files:

  `git add .`

- To saves a log message along with the commit id of the modifications made to the git repository

  `git commit –m "<your commit message>"`

- To push the contents of your local repository to the remote repository you’ve added

  `git push -u origin <branch-name>`

- To create a new branch locally

  `git branch <branch-name>`

  To take a look at the branches and check out on which branch you’re currently working:

  `git branch` or `git branch --list`

- To switch to an existing branch or to create and switch to a new one

  `git checkout <branch-name>`

- To join a branch to the parent branch

  `git merge <name-of-branch-to-merge-in>`

- To produce a local working copy of a remote repository’s source code

  `git clone https://github.com/<repo-url>`

- To fetch and integrate a remote repository with your local repository

  `git pull`

- To show all of a repository’s commits

  `git log`
