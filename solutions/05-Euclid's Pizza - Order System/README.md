# Euclid's Pizza - Order System

## The Aim
Get the data from File 300, then append it to the end of File 200.

## Synopsis
The first level where you must make your own way through this level. It looks big and twisted, but really, all you need is your File and the destination File. Don't worry about that weird EXA sitting in the Terminal, it does nothing and you can't touch it.

## Tips and Tricks
There's a hint that this level gives you right from the beginning. File 300 will always have 5 Keywords, so you don't need to work your code dynamically...yet. Note that you can copy values into Registries, but you cannot write Keywords, so you can't just tell the EXA to stop at the last Keyword (which their order doesn't change, but that doesn't matter).

First, how do you copy values from one file to the other? You could have a number for your EXA to keep track of where it was in the file, so when you pick up the File, you SEEK to the next value you were after, or you use this neat little command: REPL. REPL creates a new EXA, so that way you can have one EXA hold File 300, while the other holds File 200.

Next, how do you loop through the file? You could repeat the same command 5 times, create a loop that counts down or checks for the end of file (`TEST EOF`), or crash your EXA. Remember how the guide mentions that you can utilise the death of EXAs? You could make a loop that copies the value, creates an EXA with the copied value, send it over to File 200, write to it, and then let it terminate itself. This way, you aren't using DROP or HALT to stop the program.

## Bonus
There's no need to LINK to the other hosts, but there is a little bonus. LINK over to the LIGHTS host and create a loop that writes 1 and 0 to #POWR.