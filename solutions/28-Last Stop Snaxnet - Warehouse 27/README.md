# Last Stop Snaxnet - Warehouse 27

## The Aim
Destroy all the centrifuges in a warehouse by overloading the pressure in each one, disabling the most pressured ones first.

## Synopsis
Honestly, there's way too many quips to use with this level, especially with a name as fitting as Last Stop Snaxnet. Basically, it's time to shut down a snack cult creating nukes to ascend into the next dimension, or something that involves trying to...maybe I won't spoil it.

## Tips and Tricks
In the STATUS host is the array of each Centrifuge, each with a value representing the amount of each pressure in each one. You're tasked with finding the highest pressure of each one. Note that, once a Centrifuge is disabled, the pressure in each active one will update randomly, so the order may not stay the same.

When you have found the highest pressue, find which Centrifuge it is, then LINK to the appropriate host. Note that the Centrifuge network has that legend above, so you'll need to LINK 800 to go further in, and LINK -1 to move back. Disabling the Centrifuge is as easy as writing 0 into #POWR. Repeat until you stop them all.