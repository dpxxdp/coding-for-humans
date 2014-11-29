#Battle Stations Ready

Lets be real.  Half the fun of knowing how to code is feeling like a badass.  Manipulating computers is an extremely cool passtime, and you want to feel cool while you're doing it.  That's why we're going to spend a little time up front getting the proper tools that make it fun- and efficient!- to code.

Now we all can't be like [this guy](http://imgur.com/VQBHLoT), but there *are* a few things you can do without going overboard that will make coding a little more exciting.  As we stated in the README, I'm assuming you're using a Mac OS X operating system.  As a result, your OS is already top-notch (personal opinion may vary) and most of the tools listed in this chapter are free software designed for integrating the human's life with the life of machines.

<hr>

###Homebrew

Homebrew is the go-to **package manager** for Mac users.  A package manager allows you to install software packages from the command line extremely easily.  To get Homebrew, run the following in Terminal:

```bash
ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

Homebrew keeps an enormous list of common software packages you might need [here](https://github.com/Homebrew/homebrew/tree/master/Library/Formula).  If you need software that isn't on the list, there's ways of using brew to get those too.  See the [Homebrew](http://brew.sh/) page.

Generally, to install a package, you'll want to run:
```bash
brew update
brew install <package-name>
```
First you updated brew's package list, then you installed the given package.  Very simple way to install packages.

Now that you have homebrew, installing the other packages you need is a piece of cake.

###git
Git is the **version control** software of choice for many Mac users.  Version control software allows you to track changes.  It also lets several people work on the same project (repository) without screwing up each other's work.  In fact, these tutorials were written under git version control!  Github, this very website, is a community of git users.  It's one massive collaboration on tons of different projects.  Learn how to use git and you can collaborate with thousands of other people all across the globe on software projects ranging from Bitcoin (digital currency project) to Node.js (server-side web framework used by many internet giants).

We'll learn the ins and outs of git later, but to install, let's take advantage of homebrew.

In Terminal, run:
```bash
brew update
brew install git
```

##Install pip
Another useful tool is pip.  Pip is a python-specific package manager. It's like homebrew, but handles packages related to python.  It will allow you to quickly download and install packages that are useful to many of the python projects in this course.

In Terminal, run:
```bash
curl -O https://bootstrap.pypa.io/get-pip.py
python get-pip.py
```

`curl` is a command you haven't learned yet, but it downloaded a file called get-pip.py.  But does the second command seem familiar?  That file is a python script.  It's much longer and more complicated than anything you learned in chapter one.  But try `cat get-pip.py` to see the contents of the file if you're interested.


[< Previous](../one/first_project_5.md) | [Appendix](../appendix.md) | [Next >](./github_2.md)
