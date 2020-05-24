# Sawayama WonderDisc - Drive Controller

## The Aim
Send modified files from DISC to BUFFER (technically CORE) ad infinitum.

## Synopsis
Thanks to the wonderous invention that is Geolocking, the games you were given are completely useless. In this level, you are making it so that not only are you able to play the games, but unlock your system to play all games from all regions (not that this matters, but that is what you are doing).

## Tips and Tricks
If you read the 2nd issue of Trash World News, you'll find a chapter called "Hardware Hacks: Sawayama WonderDisc". You will need to read this chapter as it contains the code to unlock the Disc. Unfortunately, there is no clean-cut way to input the code without inputting one digit at a time.

Once unlocked, you will gain access to DISC, where you will find several files. There is a hardware register called #TRAK which contains the file you need to copy over to BUFFER. Take the value there and grab the file with that number. Pretty simple so far.

Now it gets a little tricky. Every file in DISC contains the keyword SSEC, which you need to replace with SSEA. The correct keyword is in file 300 in your Host, and you have to replace the exact position of the keyword. This can be done by copying data into a new file and checking if the input is not a number, then adding the correct keyword in and resuming. Note that all files contain a random occurrence of SSEC in random positions. When you are done creating a modified version of the required file, place it in BUFFER, and a little black EXA comes in to take that file into CORE, where it comes accepted or failed, depending on if the file is correct. Repeat this forever, or until the end of the log, your choice.

When you are done, you will gain access to a game, HACK*MATCH.

## Bonus
That little black EXA is only important to transfer files into CORE, so what if you KILL it? Doing so nets you an achievement.