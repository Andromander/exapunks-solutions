# Workhouse - Work Management System

## The Aim
Modify the user file to make activity "less suspicious".

## Synopsis
This level now plays with the required File changing ID, so you cannot just pick up the required file. Next point of note os that once you are in the USERS host, you cannot Link back to the SECURE host, so once your EXA is in the USERS host, it has to terminate somehow, and all Files that do not belong there must be erased. This level tests your skill in maths.

## Tips and Tricks
File 300 contains the username, and File 199 contains a list of usernames, another name, and a value. You just need the value because that's the File you need. Once you have the file, here's the maths part.

To make things less of a headache, the total of the values in the file will never exceed 9999, that way you can store the value in a single register. Then, this value needs to be divided down. What I mean is that each value cannot be above 75, so for each 75 you can divide from the result is the amount of times you write 75 to file. Once you reach a value below 75, that's when you know you are done. 