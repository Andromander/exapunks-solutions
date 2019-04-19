# Mitsuzen HDI-10 - Left Hand

## The Aim
Send the values from M-CNS, H-HND, and P-HND to M-CNS, H-HND, and P-CNS respectively.

## Synopsis
First the Arm, now the hand. This time you need to send three different values to their respected #NERV registers. There are regular solutions to this, but it is recommended that you use synchronisation to cut down on all areas. 

## Tips and Tricks
Synchronisation is not the easiest thing to write, but is worth the patience. This technique, if we apply it to other coding languages, would also be referred to as multi-threadding, where multiple actions are done at the same time. A lot of the time, if it is not written properly, it can result in logic errors. In this case, it means that precision reading and writing is required. This, of course, may require NOOP.

In this case, you would need to have the readers send their values to their writers first. This creates a small delay between reading and writing. Then there will need to be turns where the other nerves will need to be created. Again, the readers should be sent out first. When it comes to writing, this is where you have to enforce a delay, since if the NOOP is not there, then the EXAs will write the wrong values.

If synchronisation is used, then Activity is substantially reduced, but there are a few Alternatives. One of them is to just have a single EXA run between all the registers, or have two EXAs between the respective registers and cheese the result.