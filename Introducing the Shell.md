# Introducing the Shell

### Questions

- What is a command shell and why would I use one?
- How can I move around on my computer?
- How can I see what files and directories I have?
- How can I specify the location of a file or directory on my computer?

### Objectives

- Describe key reasons for learning shell.

- Navigate your file system using the command line.

- Access and read help files for `bash` programs and use help files to identify useful command options.

- Demonstrate the use of tab completion, and explain its advantages.

  ## What is a shell and why should I care?

  ------

  A *shell* is a computer program that presents a command line interface which allows you to control your computer using commands entered with a keyboard instead of controlling graphical user interfaces (GUIs) with a mouse/keyboard/touchscreen combination.

  There are many reasons to learn about the shell:

  - Many bioinformatics tools can only be used through a command line interface. Many more have features and parameter options which are not available in the GUI. **BLAST** is an example. Many of the advanced functions are only accessible to users who know how to use a shell.
  - The shell makes your work less boring. In bioinformatics you often need to repeat tasks with a large number of files. With the shell, you can automate those repetitive tasks and leave you free to do more exciting things.
  - The shell makes your work less error-prone. When humans do the same thing a hundred different times (or even ten times), they’re likely to make a mistake. Your computer can do the same thing a thousand times with no mistakes.
  - The shell makes your work more reproducible. When you carry out your work in the command-line (rather than a GUI), your computer keeps a record of every step that you’ve carried out, which you can use to re-do your work when you need to. It also gives you a way to communicate unambiguously what you’ve done, so that others can inspect or apply your process to new data.
  - Many bioinformatic tasks require large amounts of computing power and can’t realistically be run on your own machine. These tasks are best performed using remote computers or cloud computing, which can only be accessed through a shell.

  In this lesson you will learn how to use the command line interface to move around in your file system.

  ## How to access the shell

  ------

  On a Mac or Linux machine, you can access a shell through a program called “Terminal”, which is already available on your computer. The Terminal is a window into which we will type commands. If you’re using Windows, you’ll need to download a separate program to access the shell.

  To save time, we are going to be working on a remote server where all the necessary data and software available. When we say a ‘remote server’, we are talking about a computer that is not the one you are working on right now. You will access the Carpentries remote server where everything is prepared for the lesson. We will learn the basics of the shell by manipulating some data files. Some of these files are very large , and would take time to download to your computer. We will also be using several bioinformatic packages in later lessons and installing all of the software would take up time even more time. A ‘ready-to-go’ server lets us focus on learning.

  

  This provides a lot of information about the remote server that you’re logging into. We’re not going to use most of this information for our workshop, so you can clear your screen using the `clear` command. 

  Type the word `clear` into the terminal and press the `Enter` key.

  This will scroll your screen down to give you a fresh screen and will make it easier to read. You haven’t lost any of the information on your screen. If you scroll up, you can see everything that has been output to your screen up until this point.

  ````bat
  $
  ````

  The dollar sign is a **prompt**, which shows us that the shell is waiting for input; your shell may use a different character as a prompt and may add information before the prompt. When typing commands, either from these lessons or from other sources, do not type the prompt, only the commands that follow it.

  Let’s find out where we are by running a command called `pwd` (which stands for “print working directory”). At any moment, our **current working directory** is our current default directory, i.e., the directory that the computer assumes we want to run commands in, unless we explicitly specify something else.

````bash
$ pwd
````

Let’s look at how our file system is organized. We can see what files and subdirectories are in this directory by running `ls`, which stands for “listing”:

````bash
$ ls
````

`ls` prints the names of the files and directories in the current directory in alphabetical order, arranged neatly into columns.

The command to change locations in our file system is `cd`, followed by a directory name to change our working directory. `cd` stands for “change directory”