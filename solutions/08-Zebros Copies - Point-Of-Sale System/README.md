# Zebros Copies - Point-Of-Sale System

## The Aim
Copy the debt from File 200 and add it into File 201

## Synopsis
Things can get a little tricky here. File 300 contains the Customer ID that you will need to not only find the entry in File 200, but append it into File 201. You'll also need the values from File 200 and then once sent over, zero out the balance. While your at it, get the Date. All of this sounds colvoluted, but break it down into steps and it becomes easier.

## Tips and Tricks
Two things need to happen: erase the debt and make the payment.

To start things off, get the date. File 201 orders payments by Date, Customer ID, Dollars, and Cents, and the date is the easiest part of this.

Then, you need the customer ID. Of course, this can be found in File 300, so all that need to happen next is to COPY the value from File 300 to File 201, making sure you keep the ID so you can find the debt.

Finally, get File 200 and find the Customer ID. Like Last Stop Snaxnet, you cannot SEEK a certain value, so you have to search each entry for the right Customer ID. Quick Tip: if you want to reduce on Cycles, make a loop that SEEKS to the next Customer ID. This will reduce on time because you aren't searching the other 2 values that aren't a Customer ID.

Once you have thr right Customer ID, COPY the two values, zero them out, then go back to File 201 and copy those values over.

## Bonus
You don't need to do any copying in this level, but you can overload the Copiers. Create a loop that sends EXAs into each copier and write a value into it and repeat ad infinitum.