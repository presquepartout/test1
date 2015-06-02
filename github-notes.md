Github for the Uninitiated
==========================

###What is git? 

* a version control system: a system that keeps track of computer files for you. 
* you have to add files to the system using: 

  > git add /path/to/file
  
* if you modify the file and want to save the modifications, use:

  > git commit /path/to/file

* all previously committed versions are saved (you are liberated from “Save As…”)
* allows you to copy code from other people (git clone <repo>)
* allows you to collaborate on code with other people (create branches, merge branches) 
 
  > e.g. git checkout - b \<branch\>

* git predates github
* git was created by Linus Torvalds as the version control system for the linux kernel 

###What is github?
* github is online, distributed git
* because github is web based and distributed, copies of repositories can exist in many places; the concept of “master” is slightly different
* In addition to the ideas of clone and branch, github introduces the concept of fork
* a forked repository is a copy of another person’s repository in your own github account
* a forked copy is similar to a clone

###What is a Repository? 
* a collection of files that you want git to control together. 
* like a folder in the git system.
* has a tree structure, with initially added and committed files as root nodes. Changed files are child nodes. 
* called repo for short
* whole repo can be branched or cloned; in github can also be forked 

###What is origin/master?
* in git, this had a meaning as the original, first repository. 
* in github, this is a bit less meaningful because repos are distributed

###What is a Fork or forked repo?
* a fork is a copy of someone else's repo in your github account

###What is a Branch? How do I create a branch? 
* a branch is a named, isolated copy of a repo. Let the original repo be called original_repo. 
* you can commit and push changes to your branch and it will not affect original_repo. 

###What is a clone, or what does it mean to clone? How do I clone? 
* a clone is a full copy of a repo. 
* a clone includes all branches. 
* typical use case is you clone one of your github repos to your desktop so you can work on it. 

###What is push?
* push is what you do if you have cloned your repo from github to your desktop, made modifications, and want to keep your modifications on your repo
* sequence of events would be:
  > fork a repo to your github
  > clone the repo to your desktop so you can work on it
  > branch the repo so that your work is isolated, doesn't break others', and others' doesn't break yours
  > git checkout -b <branch>
  > make additions, changes, commit them; to keep track, use: 
  > git status 
  > push changes to your branch on your github account:
  > git push origin branch
* push is when you update your own github branch with your own changes

###What is pull, or a pull request? 
* first you have to have already created a branch from another repo. Suppose your branch is called your_repo and the original other repo is called other_repo. 
* a pull request is a message to the owner of other_repo that you have created changes and other_repo has an option to merge the changed file(s) in your_repo with other_repo
* pull is when you update your github repo with someone else's repo changes
* a pull request is when you invite someone else to update their repo with your changes
* in github, the owner of other_repo has to be a collaborator of your_repo

