# TEC EXA-Blaster Modem - Pager Network

## The Aim
Relay the message from one file in your host to all pagers on the network at the same time.

## Synopsis
Again, this is why we don't use old technology now, because AI wants to be human, or something. You will need to dial into each pager, but instead of taking information, you're going to send a message via #PAGE. This also uses the modem network.

## Tips and Tricks
Like the last TEC-EXA Blaster level, you can only dial one number at a time. However, unlike last time, you have all the numbers you need in another file. First thing you need to do is dial into the modem from file 301, send an EXA into the connected host, then write each value in sequence into #DATA. Do not write anything into #PAGE just yet, because you need to send the message from all pagers at once.

Once each pager has the message, the tricky part comes in. The aim is to send the message all at once, but because only one modem is going to be connected at each time, you need a sort of timer or stall code in each EXA so that they can all fire at once. The value written into #PAGE does not matter; any value written here will cause the message to send. Again, I will note: this needs to be done in the same Cycle.

	