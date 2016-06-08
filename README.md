# Git Smart

An introduction to Git and GitHub. Hosted by Women Who Code LA and
Carbon Five.

## Before you arrive

* You will need to bring a laptop device to be able to run these
  examples on your own!
* Sign up for an account on http://www.github.com.
* Be sure to download the GitHub Desktop client (Windows or Mac): https://desktop.github.com/

## Why Git?

Git powers much of software development today - it enables users to keep
track of changes to software from many different locations. It is
decentralized enough to allow users to work on software from anywhere in
the world.

GitHub is a cloud service that hosts Git repositories. Its strength is
in the ease in which it allows you to view and edit files, and share
your changes with other people. It also allows you to keep a full
history of changes to that repository - meaning that at any point in
time you can see what files changed, how they changed, and if you want,
you can restore changes from the past.

Think back to the last time you worked on a group project at school.
Maybe you had to work on a report or a presentation. How did you all
manage to work on the document? Did you email it around, or send it
around on a USB stick, CD-ROM, floppy? Do you remember how much work it
took to make sure everybody had the same document?

Then - some of you may understand this analogy - do you remember how the
game changed when you learned how to use a cloud document service, like
Google Docs? Suddenly, everybody had one place to go to. Changes were
propogated and trackable. You could rest easy knowing that people's
changes could be rolled back.

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

### Git & Repositories

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

These snapshots are called *commit* s.

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

#### A very important aside on commits

Remember, commits are records of changes you've made to the repository
at any point in time.

They are always accompanied by SHA values. Say it like "shaw". SHA is a
cryptographic algorithm that ensures a unique value for your change
across all values in the universe. Amazing, huh?!

Just remember this for now: when you make a commit, you get a new SHA.
This SHA value is the unique record of your change - every character that was added, or removed, is uniquely compressed into a scalar value.

### 4) Adding files

Create a new file in the `git-poems` folder on your computer. You
can create a text file with Microsoft Word, or with TextEdit, or with a
code editor of your choice. Call it 'the-road-not-taken.txt'.

```
TWO roads diverged in a yellow wood,
And sorry I could not travel both
And be one traveler, long I stood
And looked down one as far as I could
To where it bent in the undergrowth;

Then took the other, as just as fair,
And having perhaps the better claim,
Because it was grassy and wanted wear;
Though as for that the passing there
Had worn them really about the same,

And both that morning equally lay
In leaves no step had trodden black.
Oh, I kept the first for another day!
Yet knowing how way leads on to way,
I doubted if I should ever come back.

I shall be telling this with a sigh
Somewhere ages and ages hence:
Two roads diverged in a wood, and I—
I took the one less traveled by,
And that has made all the difference.
```

OK, saved it?

Now go open GitHub Desktop again. You should see a new file available
for adding. You will want to be on the "1 Uncommitted Change" tab,
viewing changes.

Select the checkbox next to the new file. Enter a description of what
you are doing in the "Summary" field - in this case, "Adding Robert
Frost poem" could be a good summary message. The description field is
optional.

Click "Commit to master". Now flip back to the "History" tab. Click on
the last change we just made.

Show your partner. Compare your SHAs. You got another one! Why are your SHAs different?
Discuss.

## Part 2: Moving to the Cloud

Oh boy! We just made changes to our repository on our computer. Really,
we've just made changes to files on our local repository. However, we
want to get our changes up to GitHub. Why? The code needs to live
somewhere where it's shareable. GitHub is the place to share or store
the code.

We do this by making a "push". Open GitHub Desktop and click "Sync" in
the upper-right hand corner. What is happening here is that your desktop
software is comparing differences between your repository and the
original repository in GitHub. It's pushing up your changes (the fixed
typo and the new file), then it's saving them in the cloud. Then it's
checking if there's anything new on the cloud, and downloading them to
your computer.

Go check your repository URL. It should be at
[http://github.com/<your-github-username>/git-poems](http://github.com/<your-github-username>/git-poems). 
Do you see your fixed typo and new poem?




## Get in touch

Andrew Hao
andrew@carbonfive.com
