# Mitsuzen HDI-10 - Visual Cortex

## The Aim
Hack your eyes so that values from the optic nerves are sent into the visual cortex

## Synopsis
Your eyes are broken and the only prescription is to put nanobots in. There are two points of interest, one being a 3x3 grid of optic nerves, and a host that connects to the visual corted (V-CTX). This is another level where your solution does not require terminating EXAs by the end, as you don't need to end it.

## Tips and Tricks
I found there are two approaches to this level, one that benefits size, and another that benefits Activity and Cycle. Both are still viable.

The first is to, essentially, send an army of EXAs into the optic nerves, calculate what value should return, then send back to the EXA in the visual cortex to do the rest. This makes it so that the wave of EXAs will bring back all the values needed at that point in time.

The second is to place EXAs in each optic nerve and they all send over the value, saving on Activity. However, this does mean requiring some way to stall an EXA until it is needed again to prevent calculating an incorrect number or EXAs communicating to the wrong EXA. This does, in turn, save on Cycles because of not having to wait for waves to complete and then create another wave.

In both instances, you'll need to get the value in each optic nerve's #NERV and determine whether it is above -55. When you have counted out how many #NERV in the optic nerves are above -55, send them over to an EXA in V-CTX, where it will multiply that tally by 5, then subtract by -75. Repeat ad infinitum as this level technically doesn't end.