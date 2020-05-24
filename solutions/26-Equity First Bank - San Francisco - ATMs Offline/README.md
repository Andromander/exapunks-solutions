# Equity First Bank - San Francisco - ATMs Offline

## The Aim
Create a new account, add it into Checking, then transfer all of the money from other accounts into the new account in small increments.

## Synopsis
Back to the bank, this time without any ATMs to abuse in $20 increments. This time, you're going to create a new account for EMBER-2 and then transfer a little bit of money from each account into this new account.

## Tips and Tricks
No time for questions; give the AI some money.

First thing you'll want to do is, obviously, create this account. This is just a case of taking file 300 and moving it into the CHECKING host for now.

When you are withrawing money from other accounts, you will need the account number (first value in the account file), the keyword 'DEBIT' found in file 301, and then input 1 and 0 (this represents $1 and 0c). This should be written into the end of the file.

Note that when you are depositing money into this new account, it must be done in $1 increments, and requires the 'CREDIT' keyword as well as the account's number. Inputting money is as simple as writing 1 and then 0.

Placing file 300 is not all when it comes to installing the account. File 199 contains all of the account files, so you will need to install that account into file 199. This is as simple as writing 300 into the end of the file, since the account's file number is the same across all tests.

Once you have completed this level, you will unlock a cutscene, followed by the Axiom VirtualNetwork+, which allows you to create your own networks and levels.