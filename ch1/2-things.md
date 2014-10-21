##Things

Now you know *you* can give computers instructions.  And in time, you will learn a whole range of new instructions that you can give.  But coding is an art.  And just as important as knowing the **syntax** is being able to visualize and conceptualize everything we work on.

One *extremely* useful method for visualizing code and the ways it works is by picturing **things** in the real world.  Think of bits of code as objects.  In fact many times, that's what we're trying to represent.  A "window" on your monitor.  A "character" in a game.  A "bank account" on a website.  All of these are *things* that you might find in the real world.  We have a few different ways of representing Things in python.

###Variables
This is the most basic.  A variable is a box.  It's a piece of memory in the computer's RAM that holds a **value**.

```python
user = "matt"
```

In python we create variables and assign their values using the "=" sign.  Here we assigned the value `"matt"` to the variable `user`.  Variables can hold strings of letters, numbers, lists, dictionaries, dates, and a whole range of other types of information.  We'll cover those in more depth after this.

###Functions
This is slightly more complex.  A function is a box with an input tray and an output tray.  It is a machine that runs the same way every time.  You give the function an input, it does *something*, and it **returns** an output.

```python
def add(x,y):
  sum = x + y
  return sum
```

```python
def getMattInfo():
  return "Age = 16, Hair = brown, Height = tall"
```

```python
def printmeTwice( someString ):
  print someString
  print someString
  return
```

```python
def printGreeting():
  print "hello, world"
  return
```

As you can see, defining a function is a bit more complicated than defining a variable.  But there are three things to look at here: 

`def myFunction()`: def is short for "define", this creates a function in the computer's RAM with the name: "myFunction".

`def myFunction( parameters )`: Inside the parentheses you put the **parameters** of the function.  These are variables that represent the "inputs" to the function.  These are optional.  You can have a function that does the same thing every time, without any inputs.

`return "some output value"`  This is where the function ends and *returns* an "output". Note that a return value is optional.  A `return` followed by nothing will end the function without any outputs.

Once you **define** the function, you can use it anywhere in your code: `myFunction(inputs)`.  When the interpreter gets to this, it will run the function with the inputs that you gave it, and it will replace the function with any outputs that the function may return.

```python
magicNumber = add(5,2)
print magicNumber
```

Here we've already combined variables and functions.  See how useful they can be? We ran the function `add(x,y)` with 5 and 2.  It did it's thing, returned a value, 7 and saved it to the variable, `magicNumber`.  Likewise, we'll call a function with no return variable:
```
printMeTwice("hello")
```
info = GetMattInfo()
print info

And here we call a function that takes no inputs *and* returns no outputs:
```
print "start"
printGreeting()
print "end"
```

###Objects

Objects are complex.  They are boxes full of boxes.  A single object can contain many variables and many functions.  We're not going to get into Objects yet, but it's an extremely powerful concept and I want to give you a taste that there are more exciting Things to come.


