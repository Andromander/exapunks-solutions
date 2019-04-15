# SFCTA Highway Sign #4902 - Remote Access Interface

## The Aim
Write the message given in File 300 onto the Highway Sign.

## Synopsis
If you don't focus properly, this one can trick you up. All you need to know is that you need to COPY everything in File 300 and send it over to #DATA. Here's the thing: You have to write the Row and Column values in first. There is a display at the Host that tells you what type of value to write in.

## Tips and Tricks
Like all coding languages (except those that aren't really a coding language), arrays start at 0, so the starting point is 0,0. A Row goes up to 9, and a Column goes up to 3, so the sign goes from 0,0 to 8,2. You can make an EXA count from 0 to 8 and one from 0 to 2, but an easier way would be to do a bit of maths.

The guide states that you cannot divide by zero, but you can divide zero by a number and get 0 in the end. This can be used for the Row, so you will want to divide the value by the number of characters that can fit on each Row plus 1.

Column will next be using something else: MODI. If you don't know what Modulo does, I would recommend looking it up, but to put it brief, the result of a Modulo is how many more values it would take to be fully divisible. Say you did `MODI 5 7 X`, the result would be 5 because if you divide 7 by 5, you have a remainder of 2, which means you need 5 more values to reach 7. You can use this for the Column to count up until you can MODI to 0. 

Quick Tip: You can use the same value for DIVI and MODI, so you can have a value in X that acts as the counter for both Row and Column.