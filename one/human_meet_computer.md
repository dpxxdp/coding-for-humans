#Human, Computer

###Terminal

Assuming you are reading this on a Mac, open Terminal. (Shortcut: Cmd+Space, Start typing "terminal", Hit enter.)

Terminal is a window into your computer from an unfamiliar angle.  You're probably staring a screen with a line that looks somewhat like this:

```bash
Humans-Macbook-Pro:~ human$ 
```

Terminal is a **command line tool** for navigating your computer and executing programs. Its only user interface (UI) consists of text, and it only accepts keyboard strikes as user input.

Soon enough, you'll be writing programs of your own that anyone can execute through their Terminal.  For now, let's start with a few built-in commands.

Terminal is state-based.  When Terminal shows the command prompt: `$`, Terminal is giving you, the user, access to a specific **file directory** inside your computer. Let's look at the current prompt again:

```bash
Humans-Macbook-Pro:~ human$ 
```

Each of those components, defined:

```bash
Computer-Name:current_directory current_user$ 
```

The `~` represents the home directory of the current user, usually this is /Users/<your_username>

###The File System

You already know file directories as "Folders".  The combination of all folders on your computer makes up the **file system**, its a map of all the allocated memory on the computer's hard drive.  This is how Terminal allows you, the human, to understand everything written in the memory of the computer.  The File System has a tree-like structure.  Inside any given directory, you can put any number of files (think, leaves), and any number of "child" directories (branches to other leaves and branches).


The Terminal command for "peaking" inside your current directory is: `ls`.  Try this now.





The command line gives you access to the current directory.  Type `ls`, and hit enter.
