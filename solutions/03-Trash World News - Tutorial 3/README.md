# Trash World News - Tutorial 3

## The Aim
Reading from the one-way link file, send the data from it to a new file in the outbox

## Synopsis
The third level, and the only Tutorial level to not give you the answer right there. The game is testing your skills in instructions, otherwise you're going to have a hard time playing the game (or you could find tutorials like this and copy answers, whatever).

## Tips and Tricks
The host in which the file is held captive is *one-way*, which means once an EXA is in there, it cannot get out. You'll need to start off with a second EXA or use the REPL instruction, however the latter is not as efficient as it would seem.

This one's a bit important, so listen up: *EXAs will stop what they are doing until one EXA sends a value throught M to another EXA*. This means that if an EXA is reading or writing to M, but there's no EXA to respond, they will be stuck there forever. In some situations, it is great for synchronising EXAs, but on the other, one poorly written loop can jam an EXA in place on that one instruction.

Another slightly less important tip, but will help out, is that EXAs are randomly determined who will link through first. XA could go first through, or XB will get out there first. The most important part about that is it will save you Cycles if you can get the timing right.

That's about all I can give to this level without using the solution, however these two tricks will come in handy in many levels.