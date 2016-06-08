class: middle

# Git Smart: An Introduction to Git and GitHub

#### Women Who Code LA 🌟 Carbon Five

*June 8, 2016*

---

class: middle

# Hi!

Sue Anna (@sueannayeh) and Andrew (@andrewhao)

---

class: background-image-contain middle center background-color-white

![Carbon Five](http://www.carbonfive.com/images/c5-logo-vertical.png)

---

## Before we begin:

1. Connect to wifi: `carbonfive-guest` / `guestpassword`
1. Download and install GitHub Desktop: https://desktop.github.com/
1. Create a GitHub account for yourself.
1. Download and install a text editor: [Sublime Text](https://www.sublimetext.com/) or [Atom](https://atom.io/) are good ones.
1. Open up http://g9labs.com/intro-to-git for directions.

---

## Tonight: We are git poets!

Writing code often resembles art. So why don't we just get to it and make some art?

---

## Our evening in two parts:

#### 1. Working in a repository on your computer

--

#### 2. Working with a remote repository in the cloud

---

## ⚡️ Definition!

#### Version control software

*Software that tracks changes to a set of files and folders.*

---

## ⚡️ Definition!

#### Repository

*A collection of files and folders, where changes are tracked.*

--

"A folder with special powers"

---

## ⚡️ Definition!

#### GitHub

*An online cloud-based service that stores repositories.*

--

(Remember that GitHub is not the same as Git!)

---

### ✊🏾 Step 1: Fork the `git-poems` repository to your GitHub account.

1. Visit http://www.github.com/andrewhao/git-poems
2. Click the "Fork" button
3. That repository is now copied to your account!

![Fork button](http://i.imgur.com/l5GNCpb.png)

---

## ⚡️ Definition!

#### Fork

To fork a repository is simply to copy it to your account.

---

### ✊🏾 Step 2a: create a folder to store your code in

It's a good idea to have a folder on your computer to store your repositories in!


Make a new folder called `"Code"` within your `"Home"` folder or `"Documents"` folder.

#### Help your partner when you're finished.

---

### ✊🏾 Step 2b: ⚡️ Clone your repository from GitHub Desktop

Now, we are about to do an action called "cloning", which is the act of copying a repository from the cloud down to your computer.


#### Help your partner when you're finished.

---

![Clone](http://i.giphy.com/l0K42xwweWNlhUmvS.gif)

---

## Done cloning?

Take a look around: welcome to GitHub Desktop.

---

### Step 3: Change an existing file.

Uh oh, there's a typo here in one of these poems. Can you find it?

#### When you've found it, fix it in your text editor. Save the file.

---

### ✊🏾 Step 3: Change an existing file

Now how do we store the change? By "staging" the change and then committing it to the repository. Open GitHub Desktop and click the checkmark next to the changed file.

Note how the change is highlighted.

Now type a message about the change you made, describing why you made it. Click "Commit to master"

---

![Make a commit](http://i.giphy.com/l0K4oGnTSuCuml1Hq.gif)

---

### ⚡️ Definition!

#### Commit

A saved record of a set of changes to files in a repository.

Also known as a *"revision"*

---

### ⚡️ Definition!

#### SHA (aka hash)

A cryptographic function that assigns a unique ID to the unique change in the file contents and creates a "hash", or cryptographic ID, to give it.

---

### ✊🏾 Step 3: Change an existing file

Observe now that you've committed, that your new change has been added to the History view in GitHub Desktop.

Can you find the SHA value of your commit?

#### Help your partner when you're finished.

---

### ✊🏾 Step 4: Add a file

1. In your text editor, create a new file, "the-road-not-taken.txt"
1. Copy and paste Robert Frost's famous poem into it.
1. Save it.
1. Commit it with GitHub Desktop.

#### Help your partner when you're finished.

---

# Part 2: Moving to the ☁️ (GitHub)

---

### Hosts: push your local repository to GitHub ("Sync")

--

Everybody else: Sync your repositories right after.

---

## Make conflicts

Everybody individually modify the same line from the same poem, on your
individual computers.

--

Push and sync one at a time. What happens?

---

## Uh oh!

How do you resolve a conflict?

---

class: middle

```
<<<<<<< HEAD
The quick fox jumped
=======
The brown fox jumped
>>>>>>> origin/master
```

---

class: middle

```

The quick fox jumped

The brown fox jumped

```

---

class: middle

```
The quick brown fox jumped
```

--

#### Save it! Commit it!

---

### Push your resolved conflicts to GitHub.

Then: everybody sync.

---

### Pick someone to make a new branch.

Call it `more-poetry`

---

### Fill in the rest of the poem

Find the Emily Dickinson "Hope is a Thing With Feathers" and fill in the
rest of the poem.

Google is allowed.

--

Commit it on your computer.

---

## Publish the branch

---

## Open a PR on GitHub

---

## Publish the PR on GitHub

---

## Review and merge the PR on GitHub

---

## Extra credit: poetry share!

Add poems to our repository. Find interesting ones you'd like to share!
Commit and push them to your GitHub accounts.

--

Go around to other groups and practice merging your repositories with
each other. Who can amass the largest collection?

---

Further reading:

* https://help.github.com/articles/github-glossary/
* https://www.kernel.org/pub/software/scm/git/docs/gitglossary.html
