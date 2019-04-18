# Equity First Bank - San Francisco

## The Aim
Dispense all the money in the available ATMs.

## Synopsis
Another brute-forcing level, this time linking to the available ATMs. Each run does not have the same number of ATMs at the same links, so it is recommended to make EXAs Link to ATMs that may not exist. Also, each ATM has a certain amount of cash within them, so once the ATM hits 0 and you attempt to dispense more notes, you will fail the level.

## Tips and Tricks
Getting the perfect solution isn't exactly the easiest here. You can have the smallest Activity easily, but the Cycles and Size may not be desirable, depending on your solution.

Of course, because the Links are different per run, you need to make EXAs that can Link to even those that don't exist yet. There is a short, relatively static range of values these Links have, so it is possible to make a loop last a certain amount before EXAs should stop being replicated.

The next part is the slightly messy part, and solutions will vary based on what the desired result is. The less Cycles you want, the greater the Size may be, and vice-versa can apply. There are multiple ways to approach it, but note that there will always be faster results than others.