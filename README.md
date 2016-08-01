# Assignment 0

Welcome to the IS program! You have a very exciting year ahead of you. This year, IS 403 will be using GitHub for assignment submissions and feedback. This assignment will show you the process of submitting an assignment through GitHub and help familiarize you with some of Git's most common features.

## What is Git?

Git is a [version control](https://en.wikipedia.org/wiki/Version_control) software. It was created to help teams work together to build large software projects. It is also very useful for individual projects and small teams because it tracks project history and helps organize files. Services like GitHub, BitBucket, or GitLab can be used to host projects that use git (called **repositories**) in the cloud so they are safely backed up accessible anywhere.

## How do I use Git?

In this assignment, you will use 5 basic git commands:

* `clone` - _Cloning_ a repository means copying it to your computer so you can make changes. Think of it like downloading a folder.
* `checkout` - The _checkout_ command lets you switch to or create a new _branch_ of a repository. Think of a branch like your personal copy of the codebase.
* `add` - The _add_ lets you pick which changes to include in your next commit.
* `commit` - A _commit_ is a snapshot of your code at a point in time. Think of it like a point on a timeline; e.g. _On September 1, Bill added support for COGS to the product_. It is a collection of many changes (included with the `add` command) bundled into 1 point in time.
* `push` - _Pushing_ your changes sends them to the remote repository so that other team members can use them.


## I'm confused.

If you're feeling confused by all those weird terms above, no worries. That is totally normal! This section will walk you through completing the assignment so you can get a feel for how this all fits together.

### Step 1 - Clone the assignment

First, you need to _clone_ (think of it like "download") the _repository_ (code) to your computer. If you're asked for a username and password, use your GitHub information. Don't worry if nothing appears on screen when you type your password - that is a security feature. Run the command below to clone the repository:

`git clone https://github.com/byu-is-403/0-up-and-running.git`

### Step 2 - Checkout your branch

Next, you will need to make a branch for yourself. The `-b` flag on the `checkout` command will create a new branch. Run the following command:

`git checkout -b [YOUR_NET_ID]`

For example, I would run `git checkout -b mocklera`

### Step 3 - Make your changes

You should create a new `.txt` file with the following name format: `lastname_firstname.txt`; e.g. `mockler_andy.txt`. It should contain your name, your group number, and an interesting fact about you.

### Step 4 - Add your changes

Run the following to add the file:

`git add lastname_firstname.txt`

> :key: - `git add .` is a shortcut to add all your changes at once.

### Step 5 - Commit your changes

To commit those changes, run the following command:

`git commit -m "Adding my student file"`

You can put anything between those double quotes - that is called a commit message. It should be a short description of your changes; e.g. `git commit -m "Updated the homepage logo"` or `git commit -m "Fixed an annoying internet explorer bug"`.

### Step 6 - Push your changes

Finally, you will _push_ your changes to GitHub with the following command, replacing `[branch_name]` with the branch name you made in step 2:

`git push origin [branch_name]`

So, to follow the previous example, I might run `git push origin mocklera`.

> :key: - Forgot your branch name? No worries! `git status` is a command that will list all kinds of information about what you are currently doing. The first line of output should say something like `On branch [branch_name]`.

### :tada: You did it! :tada:

Nice work! You've just pushed a commit to a remote repository. Now just a couple more steps and you're all set to have your assignment reviewed by a TA.

## Using GitHub

GitHub helps us use git with a nice visual interface as well as adding a few handy features. Once you have pushed your branch to GitHub, you will need to create a `Pull Request` that will be reviewed by a TA. It is easy - just follow along with these pictures:

### Create a pull request
![Create a PR](https://raw.githubusercontent.com/byu-is-403/byu-is-403.github.io/master/instructional-assets/0-up-and-running/create_pr.png)

### Submit your pull request
![Submit a PR](https://raw.githubusercontent.com/byu-is-403/byu-is-403.github.io/master/instructional-assets/0-up-and-running/submit_pr.png)
