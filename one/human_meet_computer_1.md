#Human, Computer

###Terminal

Assuming you are reading this on a Mac, open Terminal. (Shortcut: Cmd+Space, Start typing "terminal", Hit enter.)

Terminal is a window into your computer from an unfamiliar angle.  You're probably staring a screen with a line that looks somewhat like this:

```bash
Humans-Macbook-Pro:~ human$ 
```

Terminal is a **command line tool** for navigating your computer and executing programs. Its only user interface (UI) consists of text, and it only accepts keyboard strikes as user input.

Soon enough, you'll be writing programs of your own that anyone can execute through their Terminal.  For now, let's start with a few built-in commands.

Terminal is state-based.  When Terminal shows the command prompt: `$`, Terminal is giving you, the user, access to a specific **directory** inside your computer. Let's look at the current prompt again:

```bash
Humans-Macbook-Pro:~ human$ 
```

Each of those components, defined:

```bash
Computer-Name:current_directory current_user$ 
```

The `~` represents the home directory of the current user, usually this is /Users/username

<hr>

###The File System

You already know directories as "Folders".  The combination of all folders on your computer makes up the **file system**, it is a map of all the allocated memory on the computer's hard drive.  In this way, Terminal allows you, the human, to understand everything written inside the memory of the computer.  The File System has a tree-like structure.  Inside any given directory, you can put any number of files (think: leaves), and any number of **child directories** (branches that lead to other leaves and branches).

Your computer has a single "root" directory, represented by the `/`.  When listing memory addresses, directory names are seperated by the `/` as well.  A location in memory, then, is listed like this: `/Users/matthew/Documents/homework.docx` .  This should seem familiar to you.  'homework.docx' is a piece of memory (a file), the directions to get to that memory (the address) start at the root and follow each branch: "/Users/matthew/Documents".

<hr>

Type `ls` and hit enter.

`ls` is the Terminal command for listing files and child directories inside your current directory.

`cd <directory_name>` will allow you to change your "current directory".  A few examples:

```bash
cd Documents
cd /Users/mattbro/Downloads
cd ~
cd ~/Downloads
cd usr/bin
cd ..
cd ../..
cd somefile.txt
cd
```

Try experimenting with changing directories. Keep an eye on the current directory displayed in the prompt to keep track of where you are, and use `ls` to see everything around you.  What does `cd ..` do?  Does `cd .` do anything?  What directory do you think `.` represents?

<hr>

###Touching Memory

Think of the memory as a neighborhood.  If a directory is the address of a piece of memory, the file itself is the property located at that address.

With `cd` and `ls` you can navigate and view properties, but we haven't actually learned to make new properties or build anything on existing ones.  Let's do that now.

Change into the `~` directory and run `ls`.  You should see a directory called 'Developer'.  Change into that directory.  If you don't have one, you can create this directory by running `mkdir Developer`.

Now that you're in the '~/Developer' directory, Run `mkdir cfp`.  You've created a new directory called 'cfp'.  Change into 'cfp'.  This is the directory we're going to be using to store everything related to this course.

While you're in `~/Developer/cfp`, run `touch test.txt`.  Run `ls`.  You can see you've created a new file.

Run `cat test.txt`.  This will show you the contents of the file.  Right now, it's probably empty, but there are a number of ways to edit the file.  You can use a text editor, for example, TextEdit.  You can use a sweet Integrated Developers Environment (IDE)- more in [Chapter 2]().  For now let's use nano, a super simple text editor built into Terminal.

Run `nano test.txt`.  Your file is now open, edit away!  When you're done, save with Ctrl+O and then Enter. Close nano with Ctrl+X.

Run `cat test.txt` again.  You'll see the contents of the file printed in the Terminal.

Now play around with a few more commands:

`cp test.txt copy_of_test.txt` will make a copy of your file.

`rm test.txt` will delete your file.

To recap, a list of commands we've learned:

+ `ls` list subdirectories and files
+ `cd <directory>` change directory
+ `mkdir <directory_name>` make new directory
+ `touch <file_name>` make new file
+ `rm <file_name>` remove file
+ `rm -r <directory_name>` remove directory (CAREFUL- it will remove everything inside it!!!)
+ `nano <file_name>` run simple text editor
+ `cp <source_file> <target_file>` copy a source file to a target file 
+ (use like this for copying around different directories: `cp ~/Developer/cfp/test.txt ~/Documents/test.txt`)
+ `cp -r <source_directory_name> <target_directory_name>` copy an entire directory to another directory

Continue to play around in Terminal as long as you'd like.  [Here](https://github.com/0nn0/terminal-mac-cheatsheet/wiki/Terminal-Cheatsheet-for-Mac-%28-basics-%29) is a cheat sheet for basic terminal commands.  [Here](http://www.techradar.com/us/news/computing/apple/top-25-os-x-terminal-commands-696443) are some cool Terminal tricks you might enjoy playing around with.

<hr>

###Terminal Notes

Two concepts that you should know about when navigating the world of Terminal: command structure and "sudo".

Every Terminal command has a structure as follows:

```bash
command -options <arguments>
```

Depending on the command, you don't need to supply any options or arguments.  Usually if you run `<command> -help` or `man <command>` (as in "manual"), it will display text telling you how to use the command.

When an important command is issued, such as installing a new program or deleting a locked file, the computer will not allow you to do that unless you prove you are the admin.  Therefore, the user must issue the command as a "superuser".  Do this by invoking `sudo` at the beginning of each command.  Before running, it will ask you for your password.

```bash
sudo ls
sudo touch <file_name>
sudo rm <fil_name>
```

If you ever try to run a command and you receive an error that says "access denied", try running the command using `sudo`.  But think twice about whether you actually want to run the command...

<span style="background-color:red">
WARNING: when you run commands as "sudo", there is nothing to prevent you from deleting an important system file or installing a virus.  You're in the big leagues now, a small mistake using `sudo` can seriously mess up your computer.
</span>

[< Previous](../README.md) | [Appendix](../appendix.md) | [Next >](./python_the_holy_grail_2.md)

----------------
#####Answers
----------------
What does `cd ..` do?  
Changes to the **parent** of the current directory.

oes `cd .` do anything? 
"Changes" to the same directory.

What directory do you think `.` represents?
`.` represents the current directory.
