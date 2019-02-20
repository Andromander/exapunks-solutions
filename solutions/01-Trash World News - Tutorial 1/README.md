# Trash World News - Tutorial 1

## The Aim
Get File 200 from the host to the outbox

## Synopsis
The first level. If you are reading this, chances are you're not reading the provided guide the game is giving you, or you can see the histogram beating you and you can't seem to see why (somehow). I can give the quick run down, and explain a few tips and tricks that can be learned here.

Comparing what is done here than what the guide is giving you is that it does everything step by step, no shortcuts. However, what this guide doesn't show you is how to make this look better.

## Tips and Tricks
To start off, let's see what can be cut out.

The DROP instruction makes the EXA drop the file it is holding. However, if an EXA suddenly terminates, like it tries to link to a link that doesn't exist or grab a second file, it will crash and die. When an EXA dies, they drop what they are holding. Cutting out the DROP instruction means that the EXA will drop the file and die at the same time, saving you 1 Cycle and 1 Size.

Let's get smaller. The HALT instruction tells the EXA to die. As stated in the last paragraph, EXAs can also suddenly terminate if it cannot perform the instruction. One such error is running out of instructions. Removing the HALT instruction, along with the DROP instruction, saves you 1 Size.

Of course, the tutorial won't tell you this because you are a first-timer (if you haven't completed this level) and it needs to explain each instruction one at a time.