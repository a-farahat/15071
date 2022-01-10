.. 
   15071 Software Guide 
   created by sphinx-quickstart on Sun Dec 26 13:01:32 2021.

############
Using Python
############

<Work-in-Progress>

.. ********************
.. Stepping into Python
.. ********************

.. If you're familiar with R then the transition into Python will not be hard.
.. Both are interpreted languages (you write and execute script)
.. Two differences. 
.. First indentation.
.. Second objects.
.. zero indexing

.. indentation is Python’s way of grouping statements

.. When a compound statement is entered interactively, it must be followed by a blank line to indicate completion (since the parser cannot guess when you have typed the last line).


.. *********************
.. Arithmetic operations
.. *********************

.. 5 ** 2  # 5 squared

.. comparison ==


.. *******************
.. Variable assignment
.. *******************

.. The R <- doesn't work here'
.. Assignment doesn't print'

.. ********
.. Comments
.. ********

.. Comments in Python start with the hash character, #, and extend to the end of the physical line

.. 5 ** 2  # 5 squared

.. *************************
.. Data types and structures
.. *************************

.. numbers
.. integers
.. Strings
.. Lists
.. Dictionaries

.. strings can be enclosed in single quotes ('...') or double quotes ("...") w
.. \n means newline (and formatted accordingly by a print command)
.. print('C:\some\name')  # here \n means newline!
.. print(r'C:\some\name')  # note the r before the quote
.. String literals can span multiple lines. One way is using triple-quotes
.. Strings can be concatenated (glued together) with the + operator, and repeated with *
.. Two or more string literals (i.e. the ones enclosed between quotes) next to each other are automatically concatenated.
.. This is particularly useful when you want to break long strings
.. Strings can be indexed (subscripted), with the first character having index 0. There is no separate character type; a character is simply a string of size one
.. Indices may also be negative numbers, to start counting from the right, with -1 being the rightmost character
.. Slicing is also supported; included:excluded. Thus, s[:i] + s[i:] equals to s
.. Python strings are immutable
.. The built-in function len() returns the length of a string

.. Lists; e.g. 
.. squares = [1, 4, 9, 16, 25]
.. Lists can be indexed, sliced, and concatenated
.. Unlike strings, lists are mutable
.. New items can be added at the end using the append method 
.. List elements can themselves be lists

.. zero indexing

.. 5. Data Structures

.. 5.1. More on Lists
.. many methods
.. can be used as stacks or as queues
.. list comprehensions (employed in gurobipy?)
.. e.g. squares = [x**2 for x in range(10)]




.. 5.5. Dictionaries
.. a set of key: value pairs, with the requirement that the keys are unique (within one dictionary)
.. dict comprehensions can also be used

.. pandas and numpy data structures

.. *************
.. if statements
.. *************

.. Type of flow control
.. 4.1. if Statements
.. if elif else

.. **************
.. for statements
.. **************

.. other type of flow control

.. 4.2. for Statements
.. iterates over any sequence type 

.. 4.3. The range() Function
.. can specify start and step values
.. To iterate over the indices of a sequence, one can combine range() and len() 
.. easier to use enumerate in the above case
.. range() doesn't return a list. It is an "iterable"


.. **********************************
.. Comparison and boolean expressions
.. **********************************

.. Standard comparison operators: <, >, ==, <=, >=, !=
.. Any non-zero number is true, 0 is false
.. Any non-empty sequence is true; empty sequence is false

.. ***************
.. Main references
.. ***************

.. Where you can learn about other things
.. https://docs.python.org/3/tutorial/

.. what other things you may be interested in learning

.. if you think it's useful then with high probability someone else thought the same thing and a function libnrary etc has been created another person '


.. ************
.. Coding style
.. ************

.. Be clear and consistent

.. snake case and camel case

.. 4.9. Intermezzo: Coding Style
.. PEP 8 has emerged as the style guide that most projects adhere to

******
Trivia
******

Python was first released in 1991. 
It is named after the BBC show “Monty Python’s Flying Circus” 
(you may be tested on this!).




