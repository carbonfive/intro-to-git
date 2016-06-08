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

## Intro

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

Today, we are literary researchers building up a poem
catalog. Our job is to look at the existing poems in our repository and
correct them for typos and missing parts.

Additionally, we have a couple of new poems we want to add.

## Part 1: Making changes with git

### Pair up!

Find a partner somewhere in the room. You'll be working together for much of tonight. Try to make pairs with somebody of a different Git skill level from you, so you can teach and learn from each other.

OK, got your group? Now pick one person whose computer you work on. We'll this person the *"host"* for the purposes of this next part. The partner we'll call the *"collaborator"*.

We are going to simulate a real software project, complete with a GitHub git repository in the cloud, and two (or more) collaborator working on the project at a time.

### 1) Fork the repository from our workshop to your host's personal GitHub account.

*Forking* is the action of copying the repository from one organizational user to
the other. You are essentially copying the repository from the `carbonfive` account to
yours.

1. Make sure you are signed in on Github.com.
2. Visit https://github.com/carbonfive/git-poems.
3. Click the "Fork" button.
4. (Optional) You may be presented with an account to copy to. Choose
   your preferred GitHub account to clone to.
5. You're done - you should now have your own 'git-poems' repository at
   your URL: https://github.com/your-github-username/git-poems

### 2a) Create a directory on your host's computer to store repositories.

You will want to find a directory on your computer where you want to
store this downloaded *repository* - remember, that's just a *folder*.

As a pair, use your operating system's file explorer to create a new, empty directory for your code to live. Code repositories will be checked out as nested folders within this folder.

**Tip**: Choose a directory on your file system where you keep all your
repositories. I keep a folder called **workspace** under my Home folder.
Many people have a folder called *Sites*, or *Projects*. If you don't really care, you can also use the default `Documents` folder on your computer.

### 2b) Clone the repository to the host's computer.

The first concept we want to learn is the concept of the repository.
Remember how I said the repository was a folder? You will want to
*clone* the repository, which basically means *download*.

Once you clone this repository, it will show up as a folder named
downloaded repository. So my repository now shows up in
*workspace/intro-to-git*.

As a pair on your host's computer, open up the GitHub Desktop client software. Find the "clone" button in the upper-left hand corner, find the "git-poems" repository and choose the folder you want to clone into. Click "clone" and you're on your way:

![Cloning](http://i.imgur.com/9SPLbig.gif)
*Cloning the git-poems repository to a local folder on your computer. Here, I save it into my "workspace" folder.*

Now you should see the commit list for your repository in the GitHub desktop view.

Open up your repository's file folder via Windows Explorer on a Windows computer, or
Finder on a Mac. Browse around to see the files that exist in this repository. Open them to read what they say. Show your partner!

### 3) Next up: making changes.

Uh-oh. It looks like there's a typo in one of these poems. Let's start
by opening up Emily Dickinson's *Hope Is The Thing with Feathers* poem.

Now - use your favorite text editor to fix this glaring typo (we like to use vim, Sublime, or Atom, but anything will suffice). Remember
that editing this file is just like changing any old file on your hard disk. Do you see the typo?
Find the mistake, fix it, and save the file.

Now we need to do some git magic. We need to inform Git that a change
was made. We're basically telling Git to take a snapshot of the file
system at this point in time.

These snapshots are called *commit* s. More on this in a bit.

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

#### 📖 A very important aside on commits 📖

> Remember, commits are records of changes you've made to the repository
at any point in time.

> They are always accompanied by SHA values. Say it like "shaw". SHA is a
cryptographic algorithm that ensures a unique value for your change
across all values in the universe. Amazing, huh?!

> Just remember this for now: when you make a commit, you get a new SHA.
This SHA value is the unique record of your change - every character that was added, or removed, is uniquely compressed into a scalar value.

> This specific commit consists of the record of removing the typoed letter `j` from the file, `hope_is_the_thing_with_feathers.txt`.

#### A note about git History

Look at your History tab. You'll see a list of commits (in this case, two or three). This is a linear history of what changed in your repository, by every person that has touched this code. As you continue to work in this repository, you will see more and more commits show up in this timeline.

### 4) Adding files

Create a new file in the `git-poems` folder on your computer. You
can create a text file with Microsoft Word, or with TextEdit, or with a
code editor of your choice. Call it `the_road_not_taken.txt` and place it in a new folder, `american` for American Poetry.

Copy and paste the contents of this excerpt into that file:

```
The Road Not Taken
Robert Frost

---

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

And save it in your text editor.

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

## Part 2: Moving to the Cloud... with just a little push.

### 5) Push your changes to the cloud with the Sync button.

Oh boy! We just made changes to our repository on our computer. Really,
we've just made changes to files on our local repository. However, we
want to get our changes up to GitHub. Why? The code needs to live
somewhere where it's shareable. GitHub is the place to share or store
the code.

We do this by making a "push".

Have your group's host synchronize the repository to the GitHub account:

Open GitHub Desktop and click "Sync" in the upper-right hand corner.

What is happening here is that your desktop
software is comparing differences between your repository and the
original repository in GitHub. It's pushing up your changes (the fixed
typo and the new file), then it's saving them in the cloud. Then it's
checking if there's anything new on the cloud, and downloading them to
your computer.

Go check your repository URL. It should be at
[http://github.com/your-github-username/git-poems](http://github.com/your-github-username/git-poems).
Do you see your fixed typo and new poem?

### 6) Add your partner as a collaborator to your account

We need to pause here to do some administrative tasks. Open the GitHub UI, surf over to the "Settings" tab and click on the "Collaborators" sub-tab. There, you can add your partner's username as a collaborator.

![Add your partner as a collaborator](http://i.imgur.com/F2zTYlY.gif)
*Here, __andrewhao__ is adding __sueyeh__ as a collaborator to his git-poems project*

Collaborators: once you've been added, you can visit your email address to confirm your account participation, or you can open your partner's GitHub repository webpage to accept your invitation.

Once collaborators have confirmed their addition to the host's GitHub repository, we can move on.

### 7) Have your group pull down new changes

Now, all the collaborators: it's your turn! Boot up your GitHub Desktop clients from your computers and *clone* your partner's repository to your local computer.

Compare the files that were downloaded. Look at the History pane. Do you see the changes that your host just recently made? Compare the SHA values. How do they compare?

#### Play with it

Take some time taking turns creating new poems and committing them to your local repositories. Click "sync" to push your changes to your repository, and have your partner "sync" your new changes back down to their local computers. Then switch roles and repeat the process the other way around.

### Introducing Branches

<img class="img-responsive" src="https://www.atlassian.com/git/images/tutorials/collaborating/using-branches/hero.svg" />

We are going to introduce a new concept called the *branch*.

Branches can be thought of as different streams of commits. A branch contains a list of commits and SHAs, as they are applied in order. Branches also have a diverging point - a specific commit at which they were created.

Branches are used when we want to *diverge* from another line of work, creating two parallel streams of work. This is commonly done when developers work on a feature of work but do not want to interrupt other developers from working on another feature. People will create their own personal "branch" on their computers, ensuring that any changes they make will not be modified (for the time being).

You may have noticed a thing called `master` when you worked with GitHub Desktop. Every repository has a default branch that is typically called `master`, and it's conventionally treated as the "source of truth" branch for any repository.

### 8) Create a local branch

Let's try this. Choose a member of your team to create a new branch and modify yet again another line from Emily Dickinson's poem.

To do this, you'll want to click the 'Add a branch' button from the GitHub Desktop UI.

<img class="img-responsive" src="http://i.imgur.com/4sC74j1.png" />

Name the branch `more-poetry` and make sure you've selected to set 'From' to be `master`.

Now you're on a branch! Fill in the rest of the Emily Dickinson poem, then create a commit.

Flip to the History view in GitHub desktop. Now go the branch dropdown and click `more-poetry` - this opens a select menu that lets you choose between the branches.

<img src="http://i.giphy.com/26BRBoSBcgGbccvJu.gif" class="img-responsive" />

What do you notice when you flip between the branches? Note that the latest commit only shows up on the `more-poetry` branch, and not the `master` branch.

### 9) Publish your branch

Clicking 'Publish' in the UI when you are in the `more-poetry` branch will synchronize your `more-poetry` branch with the GitHub branch in the cloud! See if you can find your branch on the Github.com repository for your host.

### 10) Review changes with Pull Requests

Here's the part of the evening when we start to get into the truly interesting stuff. In software, we oftentimes need to do "code reviews", which are peer reviews of software code. This code needs to be laid out in a manner which makes reviewing changes easy and obvious. This is done through Pull Requests, which we often call "PR"s.

The main goal of a GitHub Pull Request is to merge one branch into another. The secondary goal is to provide a place to view code changes and provide a place for conversations to occur.

Go to the GitHub repository web page you were working on earlier: http://www.github.com/your-host-username/git-poems

You should see a big green button that says "Create Pull Request" with your `more-poetry` branch name next to it. Click it.

Now you will see a form where you describe the changes you made. This is your chance to explain to your project team what changes you made on your branch.

Explain why you are making these changes, and why you want these changes to be pulled into the `master` branch.

<img src="http://i.gize.gif" class="img-responsive" />

Click "Create pull request"

Have everybody in the group open up the Pull Request from the Github.com interface. Have a discussion. View the code diffs. Click on a line and make some comments on the code. Suggest changes.

When you are ready, let's do the merge. Click "Merge pull request".

Everybody click "Sync" on GitHub Desktop. Observe that the changes from the branch are now pulled into your local computers!

#### An aside on merges

*Merging* is an action that takes one branch of code and attempts to reconcile all of its changes with another branch of code, effectively unifying them into the same code base.

Open the GitHub Desktop UI. Note how you can see the results of different branches and merges show up in the tree diagram.

### 11) Let's make things messy:

At this point, your entire group's computers have the same copy of the code.

Let's get even fancier now. One of Git's powers is its ability to resolve merge conflicts.

Individually, have everybody in the group change the 2nd line of the 1st stanza of Emily Dickinson's poem, "Hope is a Thing With Feathers". Add a word, completely change the sentence, remove a word. Be creative!

Everybody should commit their change on their own computers and give it a descriptive commit message.

Have the host in the group click the "Sync" button to push their revised poem up to GitHub.

Next, have the non-host click "Sync".

Uh oh. What happens?

<img class="img-responsive" src="http://i.imgur.com/ksy0PyJ.png" />

### 12) Conflicts are a part of life.

Welcome to the fun part of git. Working out conflicts between two code changes.

Here, one of our group members made this change:

```
'Hope' is the thing with feathers—
<<<<<<< HEAD
That should be perching in the soul—
=======
That! It perches in the soul—
>>>>>>> origin/master
And sings the tune without the words—
And never stops—at all—
```

OK, squint your eyes. There is one line that is conflicting here - the second line.

Look for the line between `<<<<<<<` and `=======`. That is the first change. It says `HEAD` - that means this is the change on your current repository - your computer.

Look for the line between `=======` and `>>>>>>>`. That is the second change. It says `origin/master` - which means that it is attributed to the remote repository `origin` on the `master` branch. This was likely the change the host pushed just a minute ago!

#### How to resolve conflicts, the manual way

In our world of software, this represents a real scenario where our code changes change a section of software that someone else has modified while we were working.

This usually forces us to have a dialogue with the author of the other line. What did they mean by their change? Does that change affect the system in a way that I must be aware of?

##### Decide how you want to resolve it

Discuss between you and your partner and figure out how to resolve this conflict between you two. Do you want to keep the first line of code, ignoring the second? Do you want to keep the second, discarding the first? Or do you want to settle on a hybrid of both lines?

### 📖 An aside on how to merge 📖

> Here's how we normally resolve these conflicts: In our text editor, we delete the `>>>` and `<<<` and `===` lines, merging the two lines above and below them into the code that "should" be there.

> In this example, we'll take a hybrid of both approaches, making this change on the non-host's computer.

    ```
    'Hope' is the thing with feathers—
    That! Should! be perching in the soul—
    And sings the tune without the words—
    And never stops—at all—
    ```

> Save the file.

> Go back to GitHub Desktop. Flip to the "1 Uncommitted Change" view. Make sure your newly saved file is checked, and note that the commit field has been pre-filled for you with a message: "Merge remote-tracking branch 'origin/master'". Additionally it is annotated with the message: `Conflicts: sonnets/hope_is_the_thing_with_feathers.txt`.

> Click "Commit to master". Flip to the history view:

> <img class="img-responsive" src="http://i.imgur.com/25fMRrf.png" />

Observe that the "merge commit" has been made on your local computer. Click "Sync" to push your merged conflict up to GitHub, and have everybody in your group sync again to fetch the merged changes.

### Onward (e.g. extra credit)

Collect some more poems - share some of your favorite poets.

Find another group and submit a Pull Request to their repositories from your own. Can you figure out how to make Pull Requests work across repositories?

## Further reading

* https://try.github.io
* https://www.git-tower.com/blog/git-cheat-sheet/ (see: "Best Practices" sheet)
* http://learngitbranching.js.org/

## Get in touch!

Andrew Hao (andrew@carbonfive.com, @andrewhao)
Sue Anna Yeh (sueanna@carbonfive.com, @sueannayeh)
Greg Buckner (gregb@carbonfive.com, @thebucknerlife)
