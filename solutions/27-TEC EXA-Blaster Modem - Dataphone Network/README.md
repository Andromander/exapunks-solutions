# TEC EXA-Blaster Modem - Dataphone Network

## The Aim
Dial into each modem on the network and gather a list of all the numbers listed in each modem.

## Synopsis
This is why we now have social media...or some other quip that involves no longer needing phones, because AI are sneaking into all of them. You're the one going into each modem, but it's the principle of the matter. You'll need to dial into each modem and gather the list of numbers in the file, name not required.

## Tips and Tricks
A few things. One: You can only dial into one modem at a time, meaning you can only LINK into one at a time. Two: If you clear the number in #DIAL, you disconnect from the modem. This will be an issue due to the way EXAs cannot communicate globally when disconnected, as well as not being able to LINK out. Three: You only get one number at the start, but each modem has at least one number that can dial into another modem.

The aim asks that you collect all the numbers into file 300, not creating a sequence of new files, so make sure you don't delete this file.

To dial into a modem, input an 11 digit number into #DIAL, and if the number is valid, a link will be established. All links use 800 to get into the modem and -1 to get out, so no need to increment through numbers to guess the link.

All modems share the same file number, 200, so there's no need to guess what the file is in the modem. However, the number of, well, numbers in each file varies, so one modem might have one number, but another might have 3. On top of this, not all numbers are going to create a link to another modem, so you will need to trial each number you get, noting that you must not disconnect the host if you haven't done collecting all the numbers yet.