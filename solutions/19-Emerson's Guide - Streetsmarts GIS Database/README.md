# Emerson's Guide - Streetsmarts GIS Database

## The Aim
Change the rating of a restaurant to 5 stars.

## Synopsis
This is where the grids become more complicated. Unlike the last time, the direction you want to go is based on the compass-shaped directional key, and all the hosts are connected to each other. Along with this, there are multiple steps that need to be taken.

## Tips and Tricks
Unlike the last time there was a grid-based network, it's not based on going forwards or backwards, but whatever the Link ID is, that is the direction you will go. Luckily, you won't need to LINK in the West direction as it is unnecessary. To navigate to the correct Host, you have two coords: one for East direction, and one for North or South. Going East is as simple as counting down, but going North or South depends on whether you count up or down.

Once you have found the correct host, you need to find the correct restaurant and change the rating. Finding the correst result is as simple as a check. Changing the rating would require getting the "star" and copying it over the blank spaces. Reason for this is because you can't COPY a non-numerical value if it is not in a register.