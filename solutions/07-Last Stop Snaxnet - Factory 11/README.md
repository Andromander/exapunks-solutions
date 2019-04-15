# Last Stop Snaxnet - Factory 11

## The Aim
Delete the keyword given in File 300 from File 237.

## Synopsis
This level sounds straightforward, and in essence, it is quite easy. However, there are a few rookie mistakes that people might make.

## Tips and Tricks
The level asks you to delete the Keyword PEANUTS from File 237. Not too bad, but one question: How do you find the Keyword?

To start off, you can't search by Keyword by going `TEST KEYWORD`, but you can still use TEST. You need the keyword from File 300 and put it in the X Register, otherwise if you put it into T, you will accidentally delete the Keyword. Then you just find that keyword and delete it.

Next question, how exactly can you find the keyword? This is where you have to think adeptly, because each run positions the Keyword differently, so you can't SEEK by a certain value. What you can do instead is do a loop, checking each value at a time. Since you have the Keyword in your Register, you can do a quick TEST on each value until you come across the right value. Note that every time you compare a value in F, the cursor moves forward, so once you found the value, go back a space and remove the Keyword.

Quick Tip: You can do this with one EXA, but if you do it with 2, you can cut down on Cycle time.