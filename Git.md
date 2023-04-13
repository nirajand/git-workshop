## Getting Started With Git


**Source Control**

Source control, or version control, is a way of tracking your files progress over time.

It is usually saved in a series of snapshots and branches, which you can move back and forth between.

**What you can do**

- Distribute your file changes
- over time
- Prevent against data
- loss/damage by creating
- backup snapshots
- Manage complex project
- structures

**About Git**

Git is a source control software, which is similar to any other version control system. It was developed by Linux creator Linus Torvalds for code maintainence written by many programmers to control workflow and merge conflicts with the code.


**Creating GitHub Account**

If you are reading this on the browser, you are likely reading from GitHub. To create a GitHub acount, go to [https://github.com/login](https://github.com/login) and sign up. After following the procedure, you need to log in into GitHub. Then we set GitHub Desktop Application. 

**What is GitHub Desktop?**

GitHub is an open-source application that lets you interact with GitHub via a Graphical User Interface (GUI) instead of relying on a command line or a web browser. GitHub Desktop incentivized you and your team to work together while employing best practices with Git and GitHub.

So, to sum it up, Git is a VCS that helps you manage your code and keep track of it, and GitHub is a cloud-based hosting platform that enables developers to manage their Git repositories. GitHub Desktop is an application that lets users interact better with GitHub through a GUI.

**Setting Up GitHub Desktop**

If you are reading here, you have perhaps downloaded GitHub Desktop Application and installed on your computer. If you haven't, download and install the application. The links are provided earlier on this Readme.

Sign in to GitHub: Once the installation is complete, launch GitHub Desktop. If you have a GitHub account, sign in with your username and password. If you don't have a GitHub account, you can create one by clicking the "Sign up for GitHub" link.

Configure GitHub Desktop: After signing in, you will be prompted to configure GitHub Desktop. You can choose to set your name and email, the default text editor, and other preferences.


### First Time Git Setup

Now that you have Git on your system, you’ll want to do a few things to customize your Git environment.

The first thing you should do when you install Git is to set your user name and email address. This is important because every Git commit uses this information, and it’s immutably baked into the commits you start creating:

```
git config --global user.name "John Doe"
git config --global user.email johndoe@example.com
```

"John Doe" is a username passed into git and "johndoe@example.com" is the mailing address passed into git so as to setup your identity. Please be cautious that the `user.email` should have the same email address as the one used to sign in into GitHub.

**Your default branch name**
By default Git will create a branch called master when you create a new repository with git init. From Git version 2.28 onwards, you can set a different name for the initial branch.

To set main as the default branch name do:

```
git config --global init.defaultBranch main
```

**Checking Your Settings**

If you want to check your configuration settings, you can use the command to list all the settings Git can find at that point:

```
git config --list
```

***Getting Help***

If you ever need help while using Git, there are three equivalent ways to get the comprehensive manual page (manpage) help for any of the Git commands:

```
git help <verb>
git <verb> --help
man git-<verb>
```

For example, you can get the manpage help for the git config command by running this:

```
git help config
```

These commands are nice because you can access them anywhere, even offline.

If you don’t need the full-blown manpage help, but just need a quick refresher on the available options for a Git command, you can ask for the more concise “help” output with the `-h` option, as in:

```
git add -h
```


**Getting a Git Repository**

You typically obtain a Git repository in one of two ways:

1. You can take a local directory that is currently not under version control, and turn it into a Git
repository, or
2. You can clone an existing Git repository from elsewhere.

In either case, you end up with a Git repository on your local machine, ready for work.


**Initializing a Repository in an Existing Directory**

If you have a project directory that is currently not under version control and you want to start
controlling it with Git, you first need to go to that project’s directory.

Use command `cd` and reach to the directory you want to work your project to be kept. The commands are well-documented at the README.md file. Please find the command, and reach to the directory and type the command:

```
git init
```

This creates a new subdirectory named `.git` that contains all of your necessary repository files — a Git repository skeleton. At this point, nothing in your project is tracked yet.

If you want to start version-controlling existing files (as opposed to an empty directory), you should
probably begin tracking those files and do an initial commit. You can accomplish that with a few `git add` 
commands that specify the files you want to track, followed by a `git commit`:

```
git add *.c
git add LICENSE
git commit -m 'Initial project version'
```

**Cloning A Repository**

If you want to get a copy of an existing Git repository — for example, a project you’d like to
contribute to — the command you need is `git clone`.

To clone a repository, follow the command:

```
git clone <url>
```

`<url>` Has value in either https or ssh you can copy from and has the url ending with `.git`.
