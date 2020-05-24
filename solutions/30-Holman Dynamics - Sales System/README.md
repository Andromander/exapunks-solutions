# Holman Dynamics - Sales System

## The Aim
Going through the file in GARBAGE, find a valid credit card number and store it in your host.

## Synopsis
Depending on how you see this level, this will either be fun or tedious. It's also where levels are going to get long, as displayed by the maximum size of 150. You are tasked with finding a valid credit card sequence from a file containing a jumbled sequence of numbers, and then having that number stored in a file in your host.

## Tips and Tricks
File 199 is the only file you need to worry about in this network. To note, there is one number in this file that is scattered throughout: -9999. This number is garbage, but is also used to cut off a sequence of numbers. If a sequence ends before you get 15 numbers (you get to -9999), it is invalid and you should skip.

Once you do get a sequence of 15 numbers, you must then validate that this sequence isn't just a bunch of numbers. You can find more information in the "How to Validate Credit Card Numbers" section in the zine provided. If it is considered invalid, dump those numbers and continue through the sequence. To help, the number will never be overlapped with an "invalid" sequence, so if those 15 numbers are wrong, it will be in the next 15 numbers.

Once you do find a valid number, you can end the search. Each test only has one number sequence that is correct, so you don't need to spend any more time finding any more. This is done just by creating a new file, putting the sequence in, then placing it into your host.