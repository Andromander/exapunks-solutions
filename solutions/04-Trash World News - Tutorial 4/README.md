# Trash World News - Tutorial 4

## The Aim
Get the value from File 200, delete it, then decrement the value by 1 and write it to a new file.

## Synopsis
The fourth and last level. This level is honestly not the best solution, however it is one of the more optimised solutions than what the guide gives you.

## Tips and Tricks
This tutorial doesn't give you the answer straight away, but instead gives you an example of a loop. While it is perfectly reasonable, there is a faster approach to this, and it required using the T registry instead of X. 

The guide tells you that the T registry is used for checking values, such as using TEST and setting it to 0 or 1 depending on whether it is true or false. From a surface level, one might assume that FJMP only checks for 0 and TJMP only checks for 1 and they both only work after TEST, but this is a bit of misinterpretation. TJMP works if T is not 0, and FJMP works if T is 0.

Using this, you can use the T register to store the value and check if it is the end of the loop. As long as TEST is not used, the T register will remain unaltered, and you can subtract down T until it hits 0.