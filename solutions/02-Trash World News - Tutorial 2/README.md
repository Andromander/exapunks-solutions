# Trash World News - Tutorial 2

## The Aim
Get File 200, complete the maths required, then take the file from the host to the outbox

## Synopsis
The first level. If you are reading this, chances are you're not reading the provided guide the game is giving you, or you can see the histogram beating you and you can't seem to see why (somehow). I can give the quick run down, and explain a few tips and tricks that can be learned here.

Comparing what is done here than what the guide is giving you is that it does everything step by step, no shortcuts. However, what this guide doesn't show you is how to make this look better.

## Tips and Tricks
Much like the first one (yes, I did take the Synopsis from the first tutorial, shut it), there are other ways to make this shorter, however it is best for the new players to understand how instructions work first. This one's a little trickier in application, but worth the saved Size and Cycles.

Just like the first level, it tells you to DROP the file and HALT the EXA. You can cut these out to save 2 Size and 1 Cycle.

This next optimisation will require some explaination, and affects the first and last two instructions. Of course, you can just COPY the value from the File (F) into the X registry, or you can ADDI F into X. You might be asking "what are you on about?" and just clicked on the solution, but bear with me. The first thing to do after you COPY F to X is to ADDI X to F and add that into X. To explain, you can use registries more than once in an equation, barring M, and every time you use F, the position jumps by 1. Doing this twice means you can ADDI the first value in the file by the second value, then put that into X.

The last optimisation is getting the value from X to F via SUBI. Just like the ADDI optimisation, using F twice causes it to move position more than once. Once you SUBI X by F, you can then put the value straight from X to F without needing to use COPY.

To explain the trickery with F, say you did `ADDI F F F`. First, it will take the first F value, add the second F value to the first, then put the result in the third position. Using this to the best ability can significantly cut down Cycle and Size.