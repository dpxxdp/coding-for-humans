#There is No Magic Here

###A Slightly More Complex Tip-Calc

I'm going to write a program for you and you're going to figure out how it works.  It's not going to be easy, but please please PLEASE, do not forget this fact: There is No Magic Here.  None.  There *is* an explanation for every piece of code.  Every outcome in computers happens for some reason.  You *can* understand all of it if you take enough time to figure it out.  

```python
#this code will calculate your tips for you
greeting = "Thanks for using Tip-Calc"
bill = raw_input('How much was your meal in dollars?\n')

generousTip = bill * 0.30
goodTip = bill * 0.20
mediocreTip = bill * 0.15
badTip = bill * 0.10

print greeting
print "A generous tip: $" + generousTip
print "A good tip    : $" + goodTip
print "A mediocre tip: $" + mediocreTip
print "A bad tip     : $" + badTip
```

Copy that code into your tip-calc.py file and run it.  Play around with it.  Edit away, try breaking it in different ways.  Challenge yourself to figure out what is happening one step at a time before moving on to the explanations below.

<hr>

###Line by Line

The best way to understand a program is to read it line by line.  After all, this *is* the way the computer reads it.

```python
#this code will calculate your tips for you
```

It's somewhat ironic that we start with this line- that's because the python interpreter is ignoring it.  Any line that starts with `#` is completely ignored, making it the perfect place to write human-readable comments.  We add comments to note the author, describe confusing code, outline what job the program is meant to perform, etc.

```python
greeting = "Thanks for using Tip-Calc"
```

This is a variable assignment. A variable is a box (here, called `greeting`). It's a piece of memory in the computer's RAM that holds onto whatever value you choose to assign it.

In python we create variables and assign their values using the "=" sign. Here we assigned a **string** of letters: `"Welcome To Tip-Calc"` to the variable: `greeting`. Now, every time we use `greeting` in the rest of our code, the python interpreter retrieves the value being stored inside.

Variables can hold strings of letters, numbers, lists, dictionaries, dates, and a whole range of other types of information. We'll cover those in more depth after this.

```python
bill = raw_input('How much did your meal cost?\n')
```

Another variable assignment.  We created a new variable, called `bill`.  But on the right side of the assignment we find something that's pretty unique.  `raw_input( )` is a very special command in python.  It allows us to take user input from the command line.  This is HUGE.  Allowing a user to interact with the program is the first step in doing anything useful on a computer.  So even though the steps behind this command are somewhat complex (but NOT magic), it's important that you learn this one right away.  If you're curious, it's called a function, but even then, it's a very special function.  We'll learn more about functions soon.

```python
generousTip = bill * 0.30
```

*Another* variable assignment.  (If you can't tell we use variables A LOT.)  This time, there is a calculation on the other side.  You've probably discovered by now that the python interpreter can do math.  You're beginning to see the power of variables, we're multiplying `0.30` by the value inside of `bill`.  In this way, we can do the math in one step no matter *what* the cost of the meal was.

```python
print greeting
```

`print` is a unique python command.  It prints whatever value you've given it to the command line.  Nice and simple.

It's also a great way to see what's going on behind the scenes of a program.  Printing variables and notifications out to the command line throughout the length of a buggy program makes it much easier to figure out where it is failing.  In this way, `print` is the most powerful debugging tool you have.

```python
print "A generous tip: " + generousTip
```

There's nothing new here.  Just note that you can use `+` to **concatenate** two strings (or in this case a string and whatever is in the variable) together into one.

<hr>

### Step Back

That was a lot to take in.  But as you continue to work through these, you will become more familiar with the language that is python.  We have only just scratched the surface of what python can do.  Remember- this language is used by NASA.  And to get you one step closer to launching space shuttles from your terminal, we're going to introduce you to the most important concept you have yet to see- Functions.

[< Previous](./python_the_holy_grail_2.md) | [Appendix](../appendix.md) | [Next >](./function_of_the_mind_4.md)

