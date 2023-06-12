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

**Getting Help**

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



### Git Commands We Will Use In This Session:

```
git clone https://github.com/nirajand/git-workshop.git          //Making a copy of the repo in local device(PC)
git init                                                                          //Initialize git in the git folder at local device
git status                                                                        //Show file status
git add .                                                                         //Add all the file 
git commit -m "Commit Message"                                                    //Commit the files
git remote add origin https://github.com/nirajand/git-workshop.git  //Connect your local git repo with a remote/online git repo.
git push -u origin                                                                //Push(Send) it to the repo
git pull                                                                          //Extract the contents from the repo to local device
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


**Checking the Status of Your Files**

The main tool you use to determine which files are in which state is the git status command. If you run this command directly after a clone, you should see something like this:

```
git status
```

GitHub changed the default branch name from master to main in mid-2020, and other Git hosts followed suit. So you may find that the default branch name in some newly created repositories is main and not master. In addition, the default branch name can be changed (as you have seen in Your default branch name), so you may see a different name for the default branch.

However, Git itself still uses master as the default, so we will use it throughout the learning process.


**Tracking New Files**

In order to begin tracking a new file, you use the command git add. To begin tracking the README file, you can run this:

```
git add fileName
```


**Short Status**

While the git status output is pretty comprehensive, it’s also quite wordy. Git also has a short status flag so you can see your changes in a more compact way. If you run `git status -s` or `git status --short` you get a far more simplified output from the command:

```
git status -s
```


**Committing Changes**

Now that your staging area is set up the way you want it, you can commit your changes. Remember that anything that is still unstaged — any files you have created or modified that you haven’t run `git add` on since you edited them — won’t go into this commit. They will stay as modified files on your disk. In this case, let’s say that the last time you ran `git status`, you saw that everything was staged, so you’re ready to commit your changes. The simplest way to commit is to type `git commit`:

```
git commit
```


**Removing Files**

To remove a file from Git, you have to remove it from your tracked files (more accurately, remove it from your staging area) and then commit. The `git rm` command does that, and also removes the file from your working directory so you don’t see it as an untracked file the next time around.

```
git rm fileName
```


**Moving Files**

Unlike many other VCSs, Git doesn’t explicitly track file movement. If you rename a file in Git, no metadata is stored in Git that tells it you renamed the file.

```
git mv file_from file_to
```


**Viewing the Commit History**

After you have created several commits, or if you have cloned a repository with an existing commit history, you’ll probably want to look back to see what has happened. The most basic and powerful tool to do this is the `git log` command.

```
git log
```


### Working with Remotes

To be able to collaborate on any Git project, you need to know how to manage your remote repositories. Remote repositories are versions of your project that are hosted on the Internet or network somewhere. You can have several of them, each of which generally is either read-only or read/write for you. Collaborating with others involves managing these remote repositories and
pushing and pulling data to and from them when you need to share work. Managing remote repositories includes knowing how to add remote repositories, remove remotes that are no longer valid, manage various remote branches and define them as being tracked or not, and more.


**Showing Your Remotes**

To see which remote servers you have configured, you can run the git remote command. It lists the shortnames of each remote handle you’ve specified. If you’ve cloned your repository, you should at least see origin — that is the default name Git gives to the server you cloned from:

```
$ git clone https://github.com/schacon/ticgit
Cloning into 'ticgit'...
remote: Reusing existing pack: 1857, done.
remote: Total 1857 (delta 0), reused 0 (delta 0)
Receiving objects: 100% (1857/1857), 374.35 KiB | 268.00 KiB/s, done.
Resolving deltas: 100% (772/772), done.
Checking connectivity... done.
$ cd ticgit
$ git remote
origin
```

The above code block is an example after cloning the repo called "ticgit".


You can also specify -v, which shows you the URLs that Git has stored for the shortname to be used when reading and writing to that remote:

```
$ git remote -v
origin https://github.com/schacon/ticgit (fetch)
origin https://github.com/schacon/ticgit (push)
```

Adding Remote Repositories
We’ve mentioned and given some demonstrations of how the `git clone` command implicitly adds the `origin` remote for you. Here’s how to add a new remote explicitly. To add a new remote Git repository as a shortname you can reference easily, run `git remote add <shortname> <url>`:

```
$ git remote
origin
$ git remote add pb https://github.com/paulboone/ticgit
$ git remote -v
origin https://github.com/schacon/ticgit (fetch)
origin https://github.com/schacon/ticgit (push)
pb https://github.com/paulboone/ticgit (fetch)
pb https://github.com/paulboone/ticgit (push)
```

Now you can use the string `pb` on the command line in lieu of the whole URL. For example, if you want to fetch all the information that Paul has but that you don’t yet have in your repository, you can run `git fetch pb`:

```
$ git fetch pb
remote: Counting objects: 43, done.
remote: Compressing objects: 100% (36/36), done.
remote: Total 43 (delta 10), reused 31 (delta 5)
Unpacking objects: 100% (43/43), done.
From https://github.com/paulboone/ticgit
* [new branch] master -> pb/master
* [new branch] ticgit -> pb/ticgit
```

Paul’s master branch is now accessible locally as pb/master — you can merge it into one of your branches, or you can check out a local branch at that point if you want to inspect it.

**Fetching and Pulling from Your Remotes**

As you just saw, to get data from your remote projects, you can run:

```
$ git fetch <remote>
```

The command goes out to that remote project and pulls down all the data from that remote project that you don’t have yet. After you do this, you should have references to all the branches from that remote, which you can merge in or inspect at any time.


**Pushing to Your Remotes**

When you have your project at a point that you want to share, you have to push it upstream. The command for this is simple: `git push <remote> <branch>`. If you want to push your `master` branch to your `origin` server (again, cloning generally sets up both of those names for you automatically), then you can run this to push any commits you’ve done back up to the server:

```
git push origin master
```

This command works only if you cloned from a server to which you have write access and if nobody has pushed in the meantime. If you and someone else clone at the same time and they push upstream and then you push upstream, your push will rightly be rejected. You’ll have to fetch their work first and incorporate it into yours before you’ll be allowed to push.


**Git Aliases**

A new feature in Git that can make your Git experience simpler, easier, and more familiar: aliases.

Git doesn’t automatically infer your command if you type it in partially. If you don’t want to type the entire text of each of the Git commands, you can easily set up an alias for each command using `git config`. Here are a couple of examples you may want to set up:

```
git config --global alias.co checkout
git config --global alias.br branch
git config --global alias.ci commit
git config --global alias.st status
```

This means that, for example, instead of typing `git commit`, you just need to type `git ci`. As you go on using Git, you’ll probably use other commands frequently as well; don’t hesitate to create new aliases.

This technique can also be very useful in creating commands that you think should exist. For example, to correct the usability problem you encountered with unstaging a file, you can add your own unstage alias to Git:

```
git config --global alias.unstage 'reset HEAD --'
```

This makes the following two commands equivalent:

```
$ git unstage fileA
$ git reset HEAD -- fileA
```

This seems a bit clearer. It’s also common to `add` a last command, like this:

```
$ git config --global alias.last 'log -1 HEAD'
```

This way, you can see the last commit easily:

```
$ git last
commit 66938dae3329c7aebe598c2246a8e6af90d04646
Author: Josh Goebel <dreamer3@example.com>
Date: Tue Aug 26 19:48:51 2008 +0800
Test for current head
Signed-off-by: Scott Chacon <schacon@example.com>
```

As you can tell, Git simply replaces the new command with whatever you alias it for. However, maybe you want to run an external command, rather than a Git subcommand. In that case, you start the command with a `!` character.
