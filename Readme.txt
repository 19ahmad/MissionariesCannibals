=== Title ===
Project 1: Missionaries and Cannibals
Author: Eli Allen

== Description ==
This is a program written in Javascript and utilizes the JQuery framework for manipulating the HTML and the buckets.js library for basic data structures. 

The meat of the code is in project1.js in the js directory. 

**NOTE** I wasn't able to finish the movement animations for the images, so at the moment, the only output is at the bottom of the page and in the browser's console. 

Whenever I finish the animations, you can view it at http://107.170.157.210/531/project1/
 

== Input ==

Accepted input: the number of missionaries and cannibals you wish to solve the problem with, as well as the size of the boat.

Input restrictions:
- The number of missionaries must be greater than 1. I limited the number of missionaries to 20 because numbers higher (and even that high) are trivial to work with, and the program takes a long time to run. 

- The number of cannibals can range from 0 to 6 per project instructions

- The boat size can range from 2 to 4 per project instructions


== Output ==

The output is a list of steps taken by the algorithm. It is displayed at the bottom of the index.html page as well as in the browser's console

The form of the output is <M,C,B> <M,C,B> 
- Each list included in the angle brackets <> represent either side of the river. The left list is the left side of the river, and the right side is the right side of the river.
- M is the nubmer of missionaries
- C is the number of cannibals
- B is the boat. For whichever side the boat is not currently on, the list will instead look like this: <M,C>. So if the boat is on the left side of the river, the output will look like this: <M,C,B><M,C>

The total number of nodes expanded by the program is displayed at the bottom along with the number of moves taken to find a solution. 

If no solution is found, the number of expanded nodes is stil displayed

== Usage ==
To run the program, simply open the index.html file in your browser, select the inputs from the selection boxes, and hit the run button

== Implementation notes ==

I utilized a breadth-first search to solve the problem. 

Each "node" is just a dictionary with keys. The specific mappings can be seen in project1.js. 

When the "run" button is pressed, the function called solve() at line 47 is called and the rest is fairly easy to follow from the comments in the source code






