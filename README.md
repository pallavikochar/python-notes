# Start date:Dec-21
# PYTHON:
Python is a high level programming language which is easy to understand by its code. It is widely used by software developers, programmers, etc. The language is named after the BBC show “Monty Python’s Flying Circus” and has nothing to do with reptiles. Python is simple to use, but it is a real programming language, offering much more structure and support for large programs than shell scripts or batch files can offer. On the other hand, Python also offers much more error checking than C, and, being a very-high-level language, it has high-level data types built in, such as flexible arrays and dictionaries. Because of its more general data types Python is applicable to a much larger problem domain than Awk or even Perl, yet many things are at least as easy in Python as in those languages. Python allows you to split your program into modules that can be reused in other Python programs. It comes with a large collection of standard modules that you can use as the basis of your programs — or as examples to start learning to program in Python. Some of these modules provide things like file I/O, system calls, sockets, and even interfaces to graphical user interface toolkits like Tk. Python is an interpreted language, which can save you considerable time during program development because no compilation and linking is necessary. The interpreter can be used interactively, which makes it easy to experiment with features of the language, to write throw-away programs, or to test functions during bottom-up program development. It is also a handy desk calculator. Python enables programs to be written compactly and readably. Programs written in Python are typically much shorter than equivalent C, C++, or Java programs, for several reasons: 1. the high-level data types allow you to express complex operations in a single statement; 2. statement grouping is done by indentation instead of beginning and ending brackets; 3. no variable or argument declarations are necessary. Python is extensible!!

###### Encoding is the process of putting a sequence of character s (letters, numbers, punctuation, and certain symbols) into a specialized format for efficient transmission or storage. Decoding is the opposite process -- the conversion of an encoded format back into the original sequence of characters.
###### UTF-8 can represent any character in the Unicode standard. UTF-8 is backwards compatible with ASCII. By default, Python source files are treated as encoded in UTF-8. 

## 1. An Informal Introduction to Python
1. Using Python as a Calculator  
  1.1. Numbers 
  1.2. Strings 
  1.3. Lists
2. First Steps Towards Programming

#### NOTE: 
1. a/b  # classic division returns a float
2. a//b  # floor division discards the fractional part
3. a%b  # the % operator returns the remainder of the division
4. a** b  # a powered b
5. Python supports numbers of type int, float, Decimal and Fraction
6. Has built-in support for complex numbers, and uses the j or J suffix to indicate the imaginary part (a+bj).
7. 'doesn\'t'  # use \' to escape the single quote..."doesn't"
8.  print('C:\some\name')  # here \n means newline!...C:\some
9.  print(r'C:\some\name')  # note the r before the quote...C:\some\name (raw strings)
10. s[:i] + s[i:] is always equal to s:
11. The while loop executes as long as the condition remains true.
12. The keyword argument end can be used to avoid the newline after the output
13. In interactive mode, the last printed expression is assigned to the variable _. This means that when you are using Python as a desk calculator, it is somewhat easier to continue calculations 
14. Python also has built-in support for complex numbers, and uses the j or J suffix to indicate the imaginary part (e.g. 3+5j).
15. String literals can span multiple lines. One way is using triple-quotes: """...""" or '''...'''. End of lines are automatically included in the string, but it’s possible to prevent this by adding a \ at the end of the line.
16. Strings can be concatenated (glued together) with the + operator, and repeated with *:
17. Two or more string literals (i.e. the ones enclosed between quotes) next to each other are automatically concatenated. >>> 'Py' 'thon' --> 'Python'. This only works with two literals though, not with variables or expressions.
18. If you want to concatenate variables or a variable and a literal, use +.
19. Python strings cannot be changed — they are immutable. Therefore, assigning to an indexed position in the string results in an error: 'str' object does not support item assignment.
20. The built-in function len() returns the length of a string.
21. Lists might contain items of different types, but usually the items all have the same type.
22. Unlike strings, which are immutable, lists are a mutable type, i.e. it is possible to change their content.
23. You can also add new items at the end of the list, by using the append() method.
24. It is possible to nest lists (create lists containing other lists).

## 2. More Control Flow Tools
1. if Statements
2. for Statements
3. The range() Function
4. break and continue Statements, and else Clauses on Loops
5. pass Statements
6. Defining Functions
7. More on Defining Functions 
  7.1. Default Argument Values
  7.2. Keyword Arguments 
  7.3. Special parameters
    7.3.1. Positional-or-Keyword Arguments
    7.3.2. Positional-Only Parameters
    7.3.3. Keyword-Only Arguments
    7.3.4. Function Examples
    7.3.5. Recap
  7.4. Arbitrary Argument Lists
  7.5. Unpacking Argument Lists
  7.6. Lambda Expressions
  7.7. Documentation Strings
  7.8. Function Annotations
8. Intermezzo: Coding Style

### NOTE:
1. x = int(input(" "))
2. if x < 0: [note the colon]
3. The keyword ‘elif’ is short for ‘else if’
4. Python’s for statement iterates over the items of any sequence (a list or a string)
5. range(5)  0, 1, 2, 3, 4
6. range(5, 10)  5, 6, 7, 8, 9
7. range(0, 10, 3)  0, 3, 6, 9
8. sum(range(4))  # 0 + 1 + 2 + 3 = 6
9. list(range(4))  [0, 1, 2, 3]
10. The break statement breaks out of the innermost enclosing for or while loop.
11. Loop statements may have an else clause i.e. the else clause belongs to the for loop, not the if statement
12. The pass can be used when a statement is required syntactically but the program requires no action.
13. The keyword def introduces a function definition
14. The return statement returns with a value from a function
15. The statement result.append(a) calls a method of the list object result
16. A method is a function that ‘belongs’ to an object and is named obj.methodname
17. The method append() adds a new element at the end of the list
18. Functions can also be called using keyword arguments of the form kwarg=value
19. When a final formal parameter of the form **name is present, it receives a dictionary (see Mapping Types — dict) containing all keyword arguments except for those corresponding to a formal parameter
20. write the function call with the *-operator to unpack the arguments out of a list or tuple
21. list(range(3, 6))     # normal call with separate arguments [3, 4, 5]
22. args = [3, 6] >>> list(range(*args))   # call with arguments unpacked from a list [3, 4, 5]
23. Small anonymous functions can be created with the lambda keyword #lambda a, b: a+b
24. Another use of lambda is to pass a small function as an argument
25. Annotations are stored in the __annotations__ attribute of the function as a dictionary and have no effect on any other part of the function

## 3. Data Structures
1. More on Lists
  1.1. Using Lists as Stacks
  1.2. Using Lists as Queues
  1.3. List Comprehensions
  1.4. Nested List Comprehensions
2. The del statement
3. Tuples and Sequences
4. Sets
5. Dictionaries
6. Looping Techniques
7. More on Conditions
8. Comparing Sequences and Other Types

### NOTE:
1. list.append(x) Add an item to the end of the list. Equivalent to a[len(a):] = [x].
2. list.extend(iterable) Extend the list by appending all the items from the iterable. Equivalent to a[len(a):] = iterable
3. ist.insert(i, x) Insert an item at a given position. The first argument is the index of the element before which to insert, so a.insert(0, x) inserts at the front of the list, and a.insert(len(a), x) is equivalent to a.append(x).
4. list.remove(x) Remove the first item from the list whose value is equal to x. It raises a ValueError if there is no such item.
5. list.pop([i]) Remove the item at the given position in the list, and return it. If no index is specified, a.pop() removes and returns the last item in the list. 
6. list.clear() Remove all items from the list. Equivalent to del a[:].
7. list.index(x[, start[, end]]) Return zero-based index in the list of the first item whose value is equal to x. Raises a ValueError if there is no such item.
8. list.count(x) Return the number of times x appears in the list.
9. list.sort(key=None, reverse=False) Sort the items of the list in place 
10. list.reverse() Reverse the elements of the list in place.
11. list.copy() Return a shallow copy of the list. Equivalent to a[:].
12. The list methods make it very easy to use a list as a stack, (“last-in, first-out”)
13. To implement a queue, use collections.deque which was designed to have fast appends and pops from both ends...  from collections import deque
14. List comprehensions provide a concise way to create lists
15. squares = list(map(lambda x: x**2, range(10))) or = [x**2 for x in range(10)]
16. 


## 4. Input and Output
1. Fancier Output Formatting
  1.1. Formatted String Literals
  1.2. The String format() Method
  1.3. Manual String Formatting
  1.4. Old string formatting
2. Reading and Writing Files
  2.1. Methods of File Objects
  2.2. Saving structured data with json

### NOTE:

## 5. Errors and Exceptions
1. Syntax Errors
2. Exceptions
3. Handling Exceptions
4. Raising Exceptions
5. User-defined Exceptions
6. Defining Clean-up Actions
7. Predefined Clean-up Actions

### NOTE:

## 6. Classes
1. A Word About Names and Objects
2. Python Scopes and Namespaces 
  2.1. Scopes and Namespaces Example
3. A First Look at Classes 
  3.1. Class Definition Syntax 
  3.2. Class Objects 
  3.3. Instance Objects 
  3.4. Method Objects 
  3.5. Class and Instance Variables
4. Random Remarks
5. Inheritance
  5.1. Multiple Inheritance
6. Private Variables
7. Odds and Ends
8. Iterators
9. Generators
10. Generator Expressions
##### References: https://docs.python.org/3/tutorial/ , https://www.learnpython.org/

