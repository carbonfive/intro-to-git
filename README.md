# Git Smart

An introduction to Git and GitHub. Hosted by Women Who Code LA and
Carbon Five.

## Before you arrive

* You will need to bring a laptop device to be able to run these
  examples on your own!
* Sign up for an account on http://www.github.com.
* Be sure to download the GitHub Desktop client (Windows or Mac): https://desktop.github.com/

## Fundamentals

### Definitions

Git works with *repositories*.

Git is a tool in the class of software called *version control*. Version
control software is a way for you to work with text files and know how
files are changed.

**IMAGES OF CHANGES**

A *repository* is a directory of files that are under *version control*.

### History

Git is a version control system invented by Linus Torvalds.

It is a class of version control systems called "Distributed Version
Control Systems". We won't really go into this today, but the model of
source control you are about to learn is what largely helps power the
flow of software development - specifically Open Source Software
development - today.

### What is Git?

Git is powerful. 

We will be working on a folder of poems.

Repositories are also thought of as "file folders with special
powers." Everything in this folder will be synced, replicated and
managed through your Git magic monocle.

GitHub is a place to host repositories. In essence, it's a set of
folders in "the cloud" on a remote server that is also version
controlled.

When we say *remote* here, we mean "in the cloud", or "on another
server, other than this current computer".

Git is a tool you install on your computer to synchronize and download
the folders on that remote computer.

## Today's project:

Today, we are literary researchers trying to collaborate on a poem
database. Our job is to look at the existing poems in our database and
correct them for typos and missing parts.

Additionally, we have a couple of new poems we want to add.

### 1) Fork the repository from our workshop to your personal GitHub account.

*Forking* is the action of copying the repository from one organizational user to
the other. You are essentially copying the repository from my account to
yours.

1. Make sure you are signed in on Github.com.
2. Visit https://github.com/andrewhao/git-poems.
3. Click the "Fork" button.
4. (Optional) You may be presented with an account to copy to. Choose
   your preferred GitHub account to clone to.
5. You're done - you should now have your own 'git-poems' repository at
   your URL: https://github.com/<your-github-username>/git-poems

### 2) Clone the repository.

The first concept we want to learn is the concept of the repository.
Remember how I said the repository was a folder? You will want to
*clone* the repository, which basically means *download*.

You will want to find a directory on your computer where you want to
store this downloaded *repository* - remember, that's just a *folder*.

**Tip**: Choose a directory on your file system where you keep all your
repositories. I keep a folder called **workspace** under my Home folder.
Many people have a folder called *Sites*, or *Projects*.

Once you clone this repository, it will show up under your folder root +
downloaded repository. So my repository now shows up in
*workspace/intro-to-git*.

Open up your repository via Windows Explorer on a Windows computer, or
Finder on a Mac. Show your partner!

### 3) Next up: making changes.

Uh-oh. It looks like there's a typo in one of these poems. Let's start
by opening up Emily Dickinson's *Hope Is The Thing with Feathers* poem in
the `poems` directory.

Now - use your favorite text editor to fix this glaring typo. Remember
that this is just any old file on your file system. Do you see the typo?
Find the mistake, fix it, and save the file.

Now that's all fine and dandy, but we need to let Git know that a change
was made. We're basically telling Git to take a snapshot of the file
system at this point in time.

These snapshots are called *commit*s.

#### Add your files to the stage.

The git stage is the pre-planning part of your repository where you tell
Git what exactly changed. In this case, we want to "add" changed files
to the repository - we are telling Git to track this file's changes.

So what we want to do now is "add" the changed file to Git, marking them
as tracked. In GitHub Desktop client, the software notices that one of
the files has changed and auto-checks the file field for you. Having it
checked means that you want it to be added.

OK, done?

#### Add a descriptive message

Now we track this change for posterity. What exactly happened in this
session? We fixed a typo. Let's make our commit message "Fixed a typo."

Under the hood, Git is saving the "change" as the removal of the letter
"j" with the message, "Fixed a typo".

Click "Commit to master".

Flip back to the "History" view. See that there is a stacked list of
commits, going down into the past.

### 4) Adding files

..

## Get in touch

Andrew Hao
andrew@carbonfive.com
