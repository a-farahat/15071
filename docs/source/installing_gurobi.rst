.. 
   15071 Software Guide 
   created by sphinx-quickstart on Sun Dec 26 13:01:32 2021.

#################
Installing Gurobi
#################

This page will guide you through setting up your computer 
with the **Gurobi optimization solver**.

You should already have installed Python. 
If not, follow these instructions first: :ref:`installing-python`. 

You will need an active internet connection. 
We recommend closing all open programs on your computer before 
starting the installation process. 

**Gurobi** is a state-of-the-art solver for optimization models 
(linear, convex quadratic, and mixed-integer models). 
Gurobi’s Python interface, **guropipy**, 
enables you to formulate and solve optimization models within Python programs. 
A full-featured, no-size limit, free academic license is available 
to academic users (students, faculty, and staff) for academic use. 
The license is free but requires that you complete 
the following registration step. 

***********************************
Registering for an academic license
***********************************

1. Visit https://pages.gurobi.com/registration 
2. Register as an Academic user. 
   You will need to provide your name and your <@mit.edu> email address 
   among other information. 
   Note: You do not need to provide your phone number 
   (feel free to type 15071 instead!).
3. You will receive an email from Gurobi to confirm your email address 
   and to set a password. 
   The link in that email expires in a few minutes, 
   so check your Inbox immediately. 
   Also check your Spam or Junk folders if you do not receive the email 
   within a few minutes.

************************
Downloading the software
************************

1. Log onto your account at www.gurobi.com.
2. From the top of the webpage select “Downloads & Licenses” 
   and then select “Gurobi Optimizer – Download Software”.
3. Review and accept the End User Agreement.
4. Download the installer file of the latest Gurobi release 
   corresponding to your operating system.
5. Run the installer and restart your computer when prompted to complete 
   the installation step.

*********************************************
Obtaining and activating the academic license
*********************************************

Important note: Make sure you are connected to the *MIT network* in this step. 

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

*******************
Installing gurobipy
*******************

Install the Python API as follows:

1. Launch Jupyter Notebook 
   (either from within the Anaconda Navigator 
   or directly from the file menu 
   <note to Teaching team: figure our Windows / Mac differences>
   <note to Teaching team: allow for students who prefer to the Spider IDE>
2. Type and run the following code (you’ll need an internet connection): 
   pip install gurobipy 
   <note to Teaching team: perhaps better use conda install>

Step 2 needs to be done only once on a given computer. 
However, to access guropipy functions in any Jupyter notebook 
we you always type and run the following two lines 
at the top of your code:

import gurobipy as gp
from gurobipy import GRB
 
Additonal resources:

https://support.gurobi.com/hc/en-us


<note to Teaching team: include a small optimization problem as 
installation verification.>