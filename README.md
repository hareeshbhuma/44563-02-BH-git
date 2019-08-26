# Basic Python Control flow Tools

![Image](https://www.python.org/static/img/python-logo@2x.png)

Python knows the usual control flow statements known from other languages, with some twists.

## Overview

Here are the items that will be briefly covered in this exploration of basic Python Control flow Tools.

1.if Statement
2.for Statement
3.break and continue Statements, and else Clauses on Loops
4.pass Statements

## if Statement

- There can be zero or more elif parts, and the else part is optional. The keyword ‘elif’ is short for ‘else if’, and is useful to avoid   excessive indentation. 
- An if … elif … elif … sequence is a substitute for the switch or case statements found in other languages.

```
>>> x = int(input("Please enter an integer: "))
Please enter an integer: 42
>>> if x < 0:
...     x = 0
...     print('Negative changed to zero')
... elif x == 0:
...     print('Zero')
... elif x == 1:
...     print('Single')
... else:
...     print('More')
...
More
```
## for Statement
The for statement in Python differs a bit from what you may be used to in C or Pascal. Rather than always iterating over an arithmetic progression of numbers (like in Pascal), or giving the user the ability to define both the iteration step and halting condition (as C), Python’s for statement iterates over the items of any sequence (a list or a string), in the order that they appear in the sequence. For example (no pun intended):

```
>>> # Measure some strings:
... words = ['cat', 'window', 'defenestrate']
>>> for w in words:
...     print(w, len(w))
...
cat 3
window 6
defenestrate 12
```
## Break and continue Statements, and else Clauses on Loops¶
- The break statement, like in C, breaks out of the innermost enclosing for or while loop.
- Loop statements may have an else clause; it is executed when the loop terminates through exhaustion of the list (with for) or when the   condition becomes false (with while), but not when the loop is terminated by a break statement. This is exemplified by the following     loop, which searches for prime numbers:

```
>>> for n in range(2, 10):
...     for x in range(2, n):
...         if n % x == 0:
...             print(n, 'equals', x, '*', n//x)
...             break
...     else:
...         # loop fell through without finding a factor
...         print(n, 'is a prime number')
...
2 is a prime number
3 is a prime number
4 equals 2 * 2
5 is a prime number
6 equals 2 * 3
7 is a prime number
8 equals 2 * 4
9 equals 3 * 3
```
## pass Statements
- The pass statement does nothing. It can be used when a statement is required syntactically but the program requires no action. For       example

```
>>> class MyEmptyClass:
...     pass

```
![http://www.letustweak.com/wp-content/uploads/2015/12/conti.png](src)

## References 

[https://python.swaroopch.com/control_flow.html](url)

[https://fresh2refresh.com/python-tutorial/python-control-statements-or-control-flow/](url)

[http://net-informations.com/python/flow/default.htm](url)
