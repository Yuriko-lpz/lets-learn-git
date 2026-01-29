# Let's learn Git!

This exercise will help you become familiar with the basic Git workflow expected of you in CPSC 131 projects. Reference the [GitHub Cheatsheet](https://education.github.com/git-cheat-sheet-education.pdf) as needed.

## Instructions

### Step 0 - Environment Setup

Run the following commands in your terminal:

```bash
sudo apt update -y && sudo apt upgrade -y
sudo apt install build-essential clang valgrind git -y
sudo snap install code --classic
```

This should cover most of the libraries needed for CPSC 131.

### Step 1 - Configuration

Make sure that Git is properly installed and configured on your system.

To test if Git is installed, run the following in your terminal:

```bash
git --version
```

To test if Git properly configured, run the following:

```
git config --global user.name
git config --global user.email
```

### Step 1.5 - Authentication

We'll be using the [GitHub CLI](https://cli.github.com/) for this to make our lives easier. On Ubuntu, you can authenticate with the following command and then by following the on-screen instructions. 

```bash
gh auth login
```

To verify you are authenticated, run the command:

```bash
gh auth status
```

### Step 2 - Clone

To make this project your own, you'll want to fork it first. Feel free to rename it.

Once forked, you can now clone the repository like so:

```bash
git clone <url>
```

You can find your repository's URL by clicking the **Code** button and copying the link under **HTTPS**.

### Step 3 - Making Changes

Let's practice the standard development loop.

* Task A - Edit the **README.md**. You can open a file with `code <file>`. Hello!
* Task B - Create a new file and type your name. You can create a new file with the syntax: `touch <file>`

### Step 4 - Add & Commit

Our new goal is to move changes from the workspace to the local history.

* Check Status: Run `git status`. You should see one "modified" file and one "untracked" file.
* Stage Everything: `git add .`
* Commit: `git commit -m "Add name to README and create text file"`

### Step 5 - Pushing to GitHub

Now, we will take our local history and upload it to GitHub.

This can be done by running:

```bash
git push
```

Refresh the repository page in your browser to verify that the upload was successful.

## Contributers

* [Joel](https://github.com/jjoeldaniel/)
* [Yuriko] ello!