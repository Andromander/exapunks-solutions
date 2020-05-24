# KGOG-TV - Satellite Uplink

## The Aim
Override the sattelite to broadcast a different program.

## Synopsis
This reminds me of those analysis videos about broadcast hijackings. You are to start by alligning the sattelite dish, then once you've targetted the sattelite, send some new data in the form of a video. Sounds simple, but things will be complicated if you don't do your research.

## Tips and Tricks
To preface right now: you will need to provided zine to complete this level, otherwise you will have no idea how to solve this.

You have two files in your host. The first file, 300, contains the details required to adjust the sattelite dish. You will need to match the Azimuth and Elevation by iterating by 1 value up or down into the respective #MOTR, while the Frequency can just be written directly into #FREQ. Note that any EXA in this host cannot link back into the SECURE host.

Next, you'll need to encrypt the video file. This is where the second file, 301, comes in. This file contains the data for the video that you will need to broadcast. For each data value, add the video's data by the key in File 199, then determine what the resulting value is. Note that an EXA cannot hold a value over 9999 or below -9999, so think wisely. You may need to use the Show Goal button to guide you.

Once you've calculated what value should be transmitted, LINK over and write that value into #DATA. Again, it should be noted that you cannot LINK back, so keep an EXA in that host with a KILL code, or send in expendable EXAs that HALT when they are done. The Transmit Log has the same number of values in the video file, so this does not need to be repeated ad infinitum. The encryption file, 199, does not end with your video file, however.