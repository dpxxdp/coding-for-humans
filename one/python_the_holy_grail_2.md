#Python: The Holy Grail

###Introduction

Let's not waste any time.  First and foremost, this course is about manipulating computers to do the human's bidding.  We may as well jump right into writing code.

Computers are powerful for two reasons:

* they do fast calculations and remember large amounts of data
* they do exactly what the human tells them

The human's job, then, is to give the computer instructions in clever ways, taking advantage of its speed and memory.  Computer instructions come in many forms, in fact you were just giving plenty of instructions through the command terminal.  A **programming language** is the principle way for humans to write complex instruction manuals for the computer.  For this course, we will use Python, a programming language specifically designed to be easy for humans to read.  Python is a hugely popular language, and it's no joke either.  Python is used by Google, NASA, IBM, and [countless other organizations](https://wiki.python.org/moin/OrganizationsUsingPython).  You'll be learning a programming language that is used in Web Development, Gaming, Science Research, Theoretical Computing, Finance... in fact pretty much any field you can think of.

Python is powerful to the you, though, for the same reason every programming language is powerful: it's a language that both the human and the computer can understand.

<hr>

###Python Works... How?

While we're looking at coding in terms of giving the computer instructions, here's how python works:

Python is a software package that comes pre-installed on Mac OS X. It is a very powerful and cleverly written algorithm that converts human-readable text into **machine code** (binary code that the computer understands).  Python uses an **interpreter** to "interpret" each line of text, and then execute the command that it produces in machine code.  If the intrepeter doesn't recognize the given text as a valid command, it will throw an error, and the code will not be run.  The collection of all the valid text that we can give the python interpreter *is* the language we call Python.

A taste of python code:

```python
print "hello, world"
```

```python
user = "Jim"
print "Hi " + user + "!"
```

```python
user = "Tommy"
userAge = 17
if userAge > 16:
  print user + ": You can legally drive!"
```

<hr>

###Running Python On Your Computer

There are a few different ways to get the python interpreter to read your text and execute its commands:

#####python in the terminal
In Terminal, run:

```bash
python
```

When you execute this, your terminal prompt will probably turn into a blinking `>`.  This means the python interpreter is running directly in your terminal.  Now give it some text: `print "hello, world"` and hit enter. You will see that it interprets and runs the commands immediately.**

Likewise, try running `printToScreen "hello, world"`.  What happens?

Obviously `printToScreen` is not part of the python language.  The python interpreter doesn't recognize it, so it throws an error.  A good error always gives you details about what went wrong.  Figuring out how to read error codes is one of the most important parts of learning to program.  See if you can tell what's going on with the error code it gave you.

Play around with the interpreter, give it some of the statements listed above.  Below is some basic python code, run these and see if you can figure out what's going on:

```python
x = 3
y = 2
print x
print y
print x + y
print x * y
print x**y
```

```python
x = 5
y = 8
print "x" + y
print "x" + "y"
x = x + 1
print x
y = y * x
print y
```

```python
name = "matt"
id = "12321"
print "Name: " + name
print "Id: " + id
```

```python
name = "dan"
number = 2
print name + number
```

Once you're done with the python interpreter, type `quit()` and hit enter.  This closes the interpreter.  You should be left with the Terminal again wherever you left off.  NOTE: When you were running all of those python scripts, you were not really doing it through the Terminal prompt.  You were running it through the program, `python`, which happened to be running inside Terminal.

#####python using scripts

Running python in the terminal was cool, and it is great for running quick calculations and testing little bits of code, but you can see where that might not be entirely useful for building a large program.  There's another way the python interpreter works its magic: on scripts.

Using terminal, create a file called hello-world.py (remember: `touch hello-world.py`).

Run `nano hello-world.py` and edit the file with one line of text: `print "hello, world`.

Save with Ctrl+O and Enter, then close nano with Ctrl+X.  (Remember, you could have used any text editor to do this.  But nano is the quick and dirty way if there isn't much going in the file.)

Now in Terminal, run `python hello-world.py`.  Works pretty much like you'd expect it to...

When you run `python <any-python-script>.py` the interpreter runs all of the python that happens to be in that file.

Play around with creating new python scripts and adding as much python code as you'd like inside.  Run the scripts you create and see how they work.  Use any errors you get to trace down bugs that might be in your code.

<hr>

###Our First Textbook (read: Boring) Program

This is a classic introductory program.  Create a new file, call it `tip-calc.py` and save it in the `~/Developer/cfp` directory.  Inside just put three lines of code:

```python
cost = 30
tip = cost * .20
print tip
```

Now save the file and run `python tip-calc.py`.  Everything go as expected?

Let's go a little further with tip-calc, before we move on to bigger and better programs.

[<- Previous Lesson]() | [Next Lesson ->]()

----------------------------
**It is somewhat [tradition](http://en.wikipedia.org/wiki/%22Hello,_world!%22_program) for the first program you write in any language to make the computer say "hello, world".
