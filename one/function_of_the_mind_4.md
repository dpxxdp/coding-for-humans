#Functions
When we looked at variables, we compared a variable to a box.  It was a box of memory that could store a single value.  Here we're going to introduce another type of box, only slightly more complex. In fact it's more like a box with a machine inside.  A **function** is a box with an input tray and an output tray.  It is a machine that runs the same way every time.  You give the function an input, it does *something*, and it **returns** an output.

Here are a few sample **function definitions**. Look them over before carrying on.  Note that if you run these, you will be creating new functions to be stored in memory, but you won't see any output yet- you haven't actually *used* the functions.

```python
def add(x,y):
  sum = x + y
  return sum
```

```python
def getMattInfo():
  return "Age = 17, Hair = brown, Height = tall"
```

```python
def printMeTwice( someString ):
  print someString
  print someString
  return
```

```python
def printGreeting():
  print "hello, world"
  return
```

As you can see, defining a function is a bit more complicated than defining a variable.

```python
def myFunction( parameters ):
  #do a whole bunch of stuff
  return "some output value"
```

There are three things to look at here:

`def myFunction():`: def is short for "define", this creates a function in the computer's RAM with the name: "myFunction".

`def myFunction( parameters ):`: Inside the parentheses you put the **parameters** of the function.  These are variables that represent the "inputs" to the function.  These are optional, it is possible to have functions without any inputs (the parentheses remain though).

`return "some output value"`  This is where the function ends and **returns** an output. Note that a return value is optional.  A `return` followed by nothing will end the function without any outputs.

Two Notes: The function name ends with `:`.  Everything in the function definition is indented.

Once you **define** the function, you can use it anywhere in your code by calling it's name and passing it any needed inputs: `myFunction(inputs)`.  When the interpreter gets to this, it will run the function with the inputs that you gave it, and it will "replace" the function call with any outputs that the function may return.

Copy and paste this into the python prompt or run it as a script from a file.

```python
def add(x,y):
  sum = x + y
  return sum

print add(5,2)
```

Step by step.  First we defined a function: `add(x,y)`.  Once it's been defined, you can use the function as many times as you want.  We ran the function with 5 and 2 as inputs.  After the function did it's thing, it should have returned the value 7.  We chose to print the value to the console, but you could have done anything you wanted with the return value.

Likewise, we'll call a function with no return value:
```python
def printMeTwice( someString ):
  print someString
  print someString
  return

printMeTwice("hello")
```

This function takes no inputs, but returns a value:

```python
def getMattInfo():
  return "Age = 17, Hair = brown, Height = tall"

info = GetMattInfo()
print info
```

And here we call a function that takes no inputs *and* returns no outputs:

```python
def printGreeting():
  print "hello, world"
  return

print "start"
printGreeting()
print "end"
```

Experiment with these.  Change them around and try to break them.  Can you see why functions might be useful?


Functions are hugely important in programming.  They allow us to write a bit of code once and not have to repeat ourselves again after that.  They also make it easier to break long code up into manageable pieces.

<hr>

Variables and Functions are our two basic building blocks for everything else we need to know.  Lets build something bigger to cap off the first chapter.

[< Previous](./no_magic_here_3.md) | [Appendix](../appendix.md) | [Next >]()
