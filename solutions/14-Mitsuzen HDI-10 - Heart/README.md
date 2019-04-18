# Mitsuzen HDI-10 - Heart

## The Aim
Make your heart beat properly using the value from CNS #NERV and writing the correct values to SA-N #NERV and AV-N #NERV.

## Synopsis
Back at this again, aren't we? This time, you need to get your heart to beat properly. Like last time, this solution should last forever, or until the end of the log if you are that cheesy.

## Tips and Tricks
There's a number of things to note in regards to this level. First of all, the value you get from CNS will need to be used for both SA-N and AV-N, though they are used at different times. Next, there is a "delay" with these registers. SA-N writes the input of the result, then AV-N. That happens once for that cycle, then it writes -70 for when it idles.

So how do you determine what value to write in? Simple: divide the value in #NERV by -10. This will give you how many times a value needs to be written in for that cycle, so if the result is 4, you write 40 first, then -70 for the rest, keeping in note that AV-N has a 1 Cycle delay to SA-N.

Quick Tip: You can either send in an EXA for each value, utilising synchronisation, or keep an EXA at each register, making sure that you don't send the values improperly. You may want to start with AV-N writing -70 into the log first, as this is the "idle" step, then resume from there.