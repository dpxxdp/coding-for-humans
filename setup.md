##Install homebrew

Homebrew is a **package manager**, it allows us to install software packages from the command line extremely easily.  Unfortunalety it doesn't come pre-installed, to get Homebrew, run the following in Terminal:

```bash
ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

Homebrew keeps an enormous list of common software packages you might need [here](https://github.com/Homebrew/homebrew/tree/master/Library/Formula).  If you need software that isn't on the list, there's ways of using brew to get that too.  See the [Homebrew](http://brew.sh/) page.

Generally, to install a package, you'll want to run:
```bash
brew update
```
That just updated brew's package list.
```bash
brew install <package-name>
```
Very simple install.

##Install git
Let's try it out.  First thing we're going to do is install git.  Git is **version control** software which allows us to track changes and let several people to work on the same project (repository) without screwing up each other's work.  We're going to use git for these tutorials.  Both of us are going to be making edits to the same **repository**, the one you're in right now!

In Terminal, run:
```bash
brew install git
```

##Install pip
Another useful tool is pip.  Pip is a python-specific package installer. It will allow you to quickly download and install packages that are useful when using python.

In terminal, run:
```bash
python get-pip.py
```

##Comments

Note that two of the commands you've already used are `python` and `ruby`.  Those are software packages too, but they come preinstalled on Mac OS X, so you didn't have to worry about installing them.

In the Terminal, you can execute a python script by running `python <some-file>.py` where <some-file>.py is the script you want to execute.
