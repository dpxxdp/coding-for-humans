##Python

While we're looking at coding in terms of giving the computer instructions, here's how python works:

The python package that comes pre-installed on Mac OS X is a whole bunch of software that converts human-readable text into **machine code** (binary code that the computer understands).  Python uses an **interpreter** (as opposed to a **compiler**, we'll talk about that later) to "interpret" each line of text, and then execute the command that it produces in machine code.  If the intrepeter doesn't recognize the given text as a valid command, it will throw an error, and the code will not be run.  The collection of all the valid text that we can give the python interpreter *is* the language we call Python.

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

## Running python on your computer

There are a few different ways to get the python interpreter to read your text and execute their commands:

###python in the terminal
In Terminal, run:

```bash
python
```

When you execute this, your terminal prompt will probably turn into a blinking `>`.  This means the python interpreter is running directly in your terminal.  Now give it some text, `print "hello, world"` and hit enter. You will see that it interprets and runs the commands immediately.**

Likewise, try running `printToScreen "hello, world"`.  What happens?

Obviously `printToScreen` is not part of the python language.  The python interpreter doesn't recognize it, so it threw an error.  A good error always gives you details about what went wrong.  Figuring out how to read errors is one of the most important parts of learning to code.  See if you can tell what's going on with the error code it gave you.

Play around with the interpreter, give it some of the statements listed above.  More example python code, run these and see if you can figure out what's going on:

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
x = 2
y = 3
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

Once you're done with the python interpreter, type `quit()` and hit enter.  This closes the interpreter.  You should be left with the terminal again wherever you left off.

###python using scripts

Running python in the terminal was cool, and it is great for running quick calculations and testing little bits of code, but you can see where that might not be entirely useful for building a large program.  There's another way the python interpreter works its magic: on scripts.

I've created a file called hello-world.py.  Inside, there is one line of text: `print "hello, world`.

In Terminal, while you're in the same directory as that file, run `python hello-world.py`.  Works pretty much like you'd expect it to...

When you run `python <any-python-script>.py` the interpreter runs all of the python in that file.  Try creating a new file, call it `tip-calc.py` and save it in this directory.  Inside just put two lines of code:

```python
cost = 30
tip = cost * .20
print tip
```

Now save the file and run `python tip-calc.py`.  Everything go as expected?


**It is somewhat [tradition](http://en.wikipedia.org/wiki/%22Hello,_world!%22_program) for the first program you write in any language to make the computer say "hello, world".
