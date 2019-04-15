# Mitsuzen HDI-10 - Left Arm

## The Aim
Copy the value from #NERV in CNS to #NERV in ARM on loop.

## Synopsis
Now you arm is broken...at the moment. Remember that Phage-thing that was mentioned at the start? It does affect you in game, and you can reverse the effect by injecting yourself with EXAs. As the level states, you do not need to leave no trace, rather you keep the loop running, but really it just has to run until the list on the right of the screen is filled with the correct results.

## Tips and Tricks
There's a few ways to solve this problem, each one affects the Cycles, Size, and Activity of the level.

If you want to prioritise Cycles, you'll learn how to abuse the MARK-REPL trick. Here, you MARK the start of the EXA, REPL itself, then continue the cycle as you would normally. This keeps an EXA in your Host continuously making copies of itself.

If you want the smallest Size, you have a less intense version of the Cycles solution. Instead of cloning itself in the main host, you clone in the CNS Host. Due to less amount of spaces, it can be slower, so Cycles might take longer.

If you want less Activity, you keep 3 EXAs by CNS, and 3 by ARM. This might be a little tricky to handle because you will have to learn synchronising. Luckily in this case, it isn't as convoluted as it will be in later levels. 

One last thing: the level mentions that you will have to "clamp" values, which means you keep all values within a set range, which in this case is between -120 and 50. You could add a check to see if the value is above or below that clamp and adjust accordingly, or use the EXA's built-in clamp. EXAs are restricted from -9999 to 9999, and values higher than that will not work, so what you could do is get the value from #NERV, then add-subtract by the level's clamp, and then you have the clamped value.