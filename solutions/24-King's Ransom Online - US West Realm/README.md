# King's Ransom Online - US West Realm

## The Aim
When the servers are offline, reset all ownership of each real estate so no players own any property.

## Synopsis
It's hacking a game within a game about hacking, how about that? In this level, what you'll want to do is disconnect all the players first. When all players are offline, the server will go offline, allowing you to go through and find all property files, resetting ownership of these files. It's free real estate...now.

## Tips and Tricks
There are 6 hosts each representing a location. In these hosts are EXAs acting as the players, some files representing property, and a master file acting as the Castle for each location. In your host is file 300 containing one keyword, which is the ID that will reset ownership.

The very first thing you'll need to do is disconnect all players. This is done via KILL, but there's a random number of players, so what now? If you go through each test, you'll notice that there's always at most 3 players per host. Note that you don't need to reset ownership of the dropped items.

Next is resetting ownership. File 200 in each host contains the file numbers for each building, so you won't need to iterate file numbers to get the building files. Once that's done, all that's left is to erase your presence from the host.

## Bonus
Those weapons do look kind of cool, if you can see through files. What if you took them for yourself? Do so, and you'll net an achievement. Note that you can't find these file numbers anywhere, so you'll need to iterate through the numbers to find them.