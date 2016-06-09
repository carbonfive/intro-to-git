class: middle

# Git Smart: An Introduction to Git and GitHub

#### Women Who Code LA 🌟 Carbon Five

*June 8, 2016*

---

class: middle

# Hi!

Sue Anna ([@sueannayeh](http://twitter.com/sueannayeh)), Andrew ([@andrewhao](http://twitter.com/andrewhao)), and Greg ([@thebucknerlife](http://twitter.com/thebucknerlife))

--

#### Many thanks to the mentors among us!

---

class: background-image-contain middle center background-color-white

![Carbon Five](http://www.carbonfive.com/images/c5-logo-vertical.png)

---

### Git Smart: Setup

1. Connect to wifi: `carbonfive-guest` / `guestpassword`
1. Download and install GitHub Desktop: https://desktop.github.com/
1. Create a GitHub account for yourself.
1. Download and install a text editor: [Sublime Text](https://www.sublimetext.com/) or [Atom](https://atom.io/) suggested.
1. Open up the project instructions: http://carbonfive.github.io/intro-to-git

---

## Our evening in two parts:

#### 1. Working in a repository on your computer

--

#### 2. Working with a remote repository in the cloud (GitHub)

---

class: middle

## Introductions 👩🏻👨😸

---

### Find a pair

Find another partner to pair up with.

Try to mix and match Git abilities - find someone with different level
of Git experience as you!

Choose someone to be the "host", the other is the "collaborator"

Sit down together.

---

class: middle

## What's Git?

---

## 📖 Definition!

#### Version control software

*Software that tracks changes to a set of files and folders.*

---

## 📖 Definition!

#### Repository

*A collection of files and folders, where changes are tracked.*

--

"A folder with special powers"

---

## 📖 Definition!

#### GitHub

*An online cloud-based service that stores repositories.*

--

(Remember that GitHub is not the same as Git!)

---

class: middle

## Why Git?

---

# 📁💻

--

# 📁☁️

--

# 📁📱

--

# 📁☁️

---

## Tonight: We are git poets!

We are literary archivists, amassing a large collection of the world's poems.

---

### ⚡️ Step 1: Fork the `git-poems` repository to your GitHub account.

1. Visit http://www.github.com/carbonfive/git-poems
2. Click the "Fork" button
3. That repository is now copied to your GitHub account!

![Fork button](http://i.imgur.com/l5GNCpb.png)

---

### ⚡️ Step 1: Fork the `git-poems` repository to your GitHub account.

View it in your browser at:

http://www.github.com/your-github-username/git-poems.

---

## 📖 Definition!

#### Fork

The act of copying a repository from one account to another.

Implies a change of ownership.

---

### ⚡️ Step 2a: create a folder to store your code in

It's a good idea to have a folder on your computer to store your repositories in!

Make a new folder called `"Code"` within your `"Home"` folder or `"Documents"` folder.

#### Help your partner when you're finished.

---

### ⚡️ Step 2b: Clone your repository from GitHub Desktop

Now, we are about to do an action called "cloning", which is the act of copying a repository from the cloud down to your computer.


#### Help your partner when you're finished.

---

![Clone](http://i.giphy.com/l0K42xwweWNlhUmvS.gif)

---

## Done cloning?

Take a look around: welcome to GitHub Desktop.

---

### Step 3: Fix a typo

Uh oh, there's a typo here in one of these poems. Can you find it?

--

 When you've found it, fix it in your text editor. Save the file.

---

### ⚡️ Step 3: Change an existing file

Now how do we store the change? By "staging" the change and then committing it to the repository. Open GitHub Desktop and click the checkmark next to the changed file.

Note how the change is highlighted.

Now type a message about the change you made, describing why you made it. Click "Commit to master"

---

![Make a commit](http://i.giphy.com/l0K4oGnTSuCuml1Hq.gif)

---

### 📖 Definition!

#### Commit

Contains a record of the changes to files in a repository.

--

Contains a reference to the commit that preceded it.

--

Other metadata, like a summary, a description, and date.

--

It only stores enough information about the "change" to a file, instead
of the entire file itself!

--

*This is a core concept in Git- don't miss it!*

---

### 📖 Definition!

#### SHA (aka hash)

A cryptographic function that assigns a unique ID to the unique change in the file contents and creates a "hash", or cryptographic ID, to give it.

---

### 📖 More on commits

A repository can be thought of as the sum of its commits.

| | Time | SHA  | Action     | Snapshot |
|-|------|------|------------|----------|
|🔵| 1    | d2cf | add 'A'    | 'A'      |
|🔵| 2    | 4f52 | append 'B' | 'AB'     |
|🔵| 3    | e2ac | append 'C' | 'ABC'    |
|🔵| 4    | 340e | delete 'B' | 'AC'    |

---

### ⚡️ Step 3: Change an existing file

Observe now that you've committed, that your new change has been added to the History view in GitHub Desktop.

Can you find the SHA value of your commit?

Can you browse forward and backwards through the History view, from commit to commit in time?

#### Help your partner when you're finished.

---

### ⚡️ Step 4: Add a file

1. In your text editor, create a new file, "the-road-not-taken.txt"
1. Copy and paste Robert Frost's famous poem into it.
1. Save it.
1. Commit it with GitHub Desktop.

#### Help your partner when you're finished.

---

class: middle

# Part 2: Moving to the ⛅️ (GitHub)

---

### Step 5: Learning about pushes

Hosts: push your local repository to GitHub by clicking the "Sync"
button.

---

### Step 6: Getting everybody on the project

Host: Time to add everybody to the project!

Visit GitHub and click on "Settings", then on "Collaborators"

Enter your collaborator(s)' GitHub usernames.

---

class: background-color-white

![Add your partner as a collaborator](http://i.imgur.com/F2zTYlY.gif)

---

### Step 6 cont'd

Collaborators: Confirm your account by email or by visiting the repository web page.

---

### Step 7: Collaborator cloning

#### Collaborators: clone

Collaborators: Open GitHub desktop, and clone the `git-poems` repository for
yourself.

#### Everybody: take some time to commit new poems.

Push to GitHub with "Sync", and have the other person "Sync" the changes back. Then switch roles.

---

### 📖 Definition!

#### Branch

A stream of commits that may diverge from another branch.

--

Useful for keeping work separate from other people's work.

---

class: center middle

![Branches](http://i.imgur.com/GzBmrJY.gif)

---

### Step 8: create a local branch

Collaborator: create a local branch on your computer with GitHub
Desktop. Click on the "Add a branch" button and name your branch `more-poetry`.

![Create a GitHub Desktop Branch](http://i.imgur.com/4sC74j1.png")

---

### Step 8 cont'd

Fill out the rest of the Emily Dickinson poem.

Commit your changes to the `more-poems` branch.

---

### Comparing branches

<img src="http://i.giphy.com/26BRBoSBcgGbccvJu.gif" class="img-responsive" />

---

## Compare your branches

Now you've got a new commit on a branch. Browse around to see all the
new, different changes!

--

Also notice that if you flip back to the `master` branch view, you won't
see your commit show up there.

---

### Step 9: Publish your branch

Click "Publish" in the upper-right hand corner of the GitHub desktop UI.

This pushes your branch to the GitHub.com cloud repository.

Visit your GitHub cloud repository to view your new branch.


---

### 📖 Definition!

#### Pull Request

Pull Requests are places to faciliate the approval of code changes from
one branch back into another.

Often used for code review.

---

### Step 10: Review changes with Pull Requests

Open a Pull Request from the GitHub UI:

---

![Pull Requests](http://i.giphy.com/l41YoufJiqXz5Nkze.gif)

---

### Review and merge the PR on GitHub

Discuss the changes with your partner. Do you agree they are correct?

Practice making comments on the pull request.

Click the big green "Merge" button when you're done!

#### Everybody sync to your local computer.

---

## Make conflicts


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
