.. 
   15071 Software Guide 
   created by sphinx-quickstart on Sun Dec 26 13:01:32 2021.

############
Using Python
############

********************
Stepping into Python
********************

.. If you're familiar with R then the transition into Python will not be hard.
.. Both are interpreted languages (you write and execute script)
.. Two differences. 
.. First indentation.
.. Second objects.
.. zero indexing

.. indentation is Python’s way of grouping statements

.. When a compound statement is entered interactively, it must be followed by a blank line to indicate completion (since the parser cannot guess when you have typed the last line).


*********************
Arithmetic operations
*********************

.. 5 ** 2  # 5 squared

.. comparison ==


*******************
Variable assignment
*******************

.. The R <- doesn't work here'
.. Assignment doesn't print'

********
Comments
********

.. Comments in Python start with the hash character, #, and extend to the end of the physical line

.. 5 ** 2  # 5 squared

*************************
Data types and structures
*************************

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

*************
if statements
*************

.. Type of flow control
.. 4.1. if Statements
.. if elif else

**************
for statements
**************

.. other type of flow control

.. 4.2. for Statements
.. iterates over any sequence type 

.. 4.3. The range() Function
.. can specify start and step values
.. To iterate over the indices of a sequence, one can combine range() and len() 
.. easier to use enumerate in the above case
.. range() doesn't return a list. It is an "iterable"


**********************************
Comparison and boolean expressions
**********************************

.. Standard comparison operators: <, >, ==, <=, >=, !=
.. Any non-zero number is true, 0 is false
.. Any non-empty sequence is true; empty sequence is false

***************
Main references
***************

.. Where you can learn about other things
.. https://docs.python.org/3/tutorial/

.. what other things you may be interested in learning

.. if you think it's useful then with high probability someone else thought the same thing and a function libnrary etc has been created another person '


************
Coding style
************

.. Be clear and consistent

.. snake case and camel case

.. 4.9. Intermezzo: Coding Style
.. PEP 8 has emerged as the style guide that most projects adhere to

******
Trivia
******

Python was first released in 1991. 
It is named after the BBC show “Monty Python’s Flying Circus” 
(you may be tested on this).






This page will guide you in setting up your computer with the **Python 
programming environment** and the **Gurobi optimization solver**. 
You will need an active internet connection. 
We recommend that you close all open programs on your computer before working 
through the following tasks. 



We recommend installing the free Anaconda distribution [#f1]_. 
This distribution provides Python 3.8.x along with 
a large collection of commonly used packages 
(but not including guropipy which we will install separately). 
This task takes approximately 10 minutes to complete.


1. Visit https://www.anaconda.com/products/individual 
   and click the Download button to download the installer 
   (see screenshot below). 
   Wait until the installer file downloads completely. 
   You may be asked if you wish to create a free Anaconda cloud account 
   (and, later, an Anaconda Nucleus account which provide access to training 
   material). 
   This is optional and can be skipped.
   
   .. image:: images/image1.png
   
2. Double click the installer to start the installation process. 
   Review and agree to the license terms. 
   Complete the installation process. 
   We recommend using the default options throughout. 
3. Launch Anaconda Navigator from the start menu 
   (you may need to be patient the first time it loads). 
   Confirm that your installation was successful in the following two ways:

   a. Launch CMD.exe Prompt from Navigator (see icon below) 
      and type python at the prompt. 
      This should return a short message 
      indicating that Python 3.8.8 is available. 
      Type exit() and close the shell window.
      
      .. image:: images/image2.png
      
   b. Launch Jupyter Notebook from Navigator (see icon below) 
      or from the Anaconda program group under the start menu. 
      This should launch a notebook file menu in a browser. 
      Try creating and saving a new notebook file. 
      Several Python Integrated Development Environments are available 
      and commonly used. We will use Jupyter notebooks throughout this course.

      .. image:: images/image3.png


<To be completed>
 

**Gurobi** is a state-of-the-art solver for optimization models 
(linear, convex quadratic, and mixed-integer models). 
Gurobi’s Python interface, called **guropipy**, 
enables you to integrate Gurobi’s functionality into Python programs. 
A full-featured, no-size limit, free academic license is available 
to academic users (students, faculty, and staff) for academic use. 
The license is free but requires that you complete 
the following registration step. 


1. Visit https://pages.gurobi.com/registration 
2. Register as an Academic user. 
   You will need to provide your name and @mit.edu email address 
   among other information. 
   Note: You do not need to provide your phone number 
   (you can type 0 instead).
3. You will receive an email from Gurobi to confirm your email address 
   and lets you set a password. 
   The link in that email expires in a few minutes, 
   so make sure you check your Inbox immediately. 
   Also check your Spam or Junk folders if you do not receive the email 
   within a few minutes.


1. Log onto your account at www.gurobi.com.
2. From the top of the webpage select “Downloads & Licenses” 
   and then select “Gurobi Optimizer – Download Software”.
3. Review and accept the End User Agreement.
4. Download the installer file of the latest Gurobi release 
   corresponding to your operating system.
5. Run the installer and restart your computer when prompted to complete 
   the installation step.


.. note::

   Make sure you are connected to the *MIT network*. 

1. Log onto your account at www.gurobi.com.
2. From the menu bar select “Academia” 
   and then select “Academic Program and Licenses”.
3. Scroll down the page to the section titled “Individual Academic Licenses” 
   and click on the link “Free Academic License page” (see screenshot below) 
4. Review and agree to the license conditions
5. The license is issued immediately 
   and its details will be available on your browser page
6. The final step is to install the license on your computer 
   using the grbgetkey command. 
   Copy the entire grbgetkey command provided and paste it into a shell 
   (or Terminal) window.

   * Windows users can access the shell window by typing "Run" 
     in the Windows search box 
     (alternatively, use the combination shortcut Windows+r). 
     Paste the grbgetkey command into the command dialogue box 
     that appears and press Enter.
   * Mac users can access the Terminal window by clicking on the search spotlight icon and typing "Terminal". Paste the grbgetkey command into the command line window that appears and press Enter.

7. Your Gurobi license should now be ready for use.



Install the python API as follows:

1. Launch Jupyter Notebook.
2. Type and run the following code (you’ll need an internet connection): 
   pip install gurobipy

Step 2 needs to be done only once on a given computer. 
However, to access guropipy functions in any Jupyter notebook 
we recommend you always type and run the following two lines 
at the top of your code:

import gurobipy as gp
from gurobipy import GRB
 
Additonal resources:

https://support.gurobi.com/hc/en-us

.. rubric:: Footnotes

.. [#f1] Google Colab (https://colab.research.google.com/) 
   is a convenient and free cloud-based alternative platform. 
   However, currently, it is only compatible with a Gurobi license 
   that imposes problem size limitations.


