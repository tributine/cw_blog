---
layout: post
title:  "Backwards String Project"
date:   2019-04-04 13:14:45 -0700
categories: jekyll update
---

#Date: 04/04/2019 13:14

I'm going to challenge myself by writing a script that takes a 'string' and returns the string printed backwards.

It's going to require me to:  <br>
1 - Set up a string to copy  <br> 
2 - Identify each different character in the string (learn to iterate through the string) <br>
3 - Assign the iterated strings from highest to lowest. (ex. 5:0) to simulate 'backwards'  <br>

Potential ideas:  <br>
Use pyperclip.paste() to take a string from the clipboard. When the python code is executed, using <br>  
pyperclip.copy() it will allow the user to simply paste the backwards string in any text document.  <br>
 <br>
 <br>
#Update: 04/04/2019 18:04 
<br>
Successfully created a python file capable of reversing a string: <br>

\# Name: Climber <br>
\# Project: Takes a string and flips it in reverse <br>

text = ['Hello my name is carr0t'] # This is the string to be reversed <br>
Let's reverse THIS <br>
<br>
\# Create a decrementing for loop that starts from the full length - 1 <br>
for i in range((int(len(text[0]) - 1) ),-1 ,-1): <br>
    print(text[0][i], end='') \# Iterate through the string character within the list <br>
<br>
\# Ex: i in range(25, -1, -1) <br>
    \# i would be 25 at first <br>
    \# print(text[0][25], end='') <br>
<br>
\# text is a list with a string. text[0] returns the string thus, <br>
\# text[0][i] returns the string character within the string in the list! <br>

Now it's time to implement pyperclip, I'll see you all later  <br>
<br>
<br>
#Update: 04/04/2019 18:04 
<br>
\# Name: Climber <br>
\# Project: Takes a string and flips it in reverse<br>
import pyperclip<br>
text = pyperclip.paste() # This is the string to be reversed taken from clipboard<br>
textrev = '' # Reverse string variable<br>
\# Let's reverse THIS<br>
<br>
\# Create a decrementing for loop that starts from the full length - 1<br>
for i in range((int(len(text) - 1) ),-1 ,-1): # Iterate in reverse through string<br>
    textrev += text[i] # Text2 = previous character + new character <br>
<br>
pyperclip.copy(textrev) # Copy the reversed string into the clipboard<br>
<br>
Example time:<br>
Hello there, today I have successfully fulfilled my goal of reversing a string!<br>
<br>
!gnirts a gnisrever fo laog ym dellifluf yllufsseccus evah I yadot ,ereht olleH<br>
<br>
<br>
IT WORKS!<br>
... !SKROW TI<br>