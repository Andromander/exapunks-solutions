# Mitsuzen HDI-10 - Cerebral Cortex

## The Aim
Map out all the hosts and the values within them and bring them into a single file in your host.

## Synopsis
So, it comes down to this. If you're reading this, it means you've reached the end and need a pointer to solve this level, just reading this message, or you skipped ahead, in which case I would advise turning away now because you're going to ruin the fun. Oh, and maybe some spoilers, so turn back now if you're skipping ahead. 

In this final level, you're going to map out your brain for EMBER-2 so that you may become one. Sounds simple, until you not only notice that the registers are in random hosts, but the entire layout is different for each test. This will test your ability to be dynamic with EXA language.

## Tips and Tricks
I will not spoil how you solve this level, unless you're going to jump into the solutions, but I'm going to recommend solving it yourself first before taking a look yourself.

To start, the number of registers is random, the placement is random, link values are seemingly random, host names are different, and networks are entirely different per test. The only consistencies are the registry names and what values you use for LINK, and I guess your host stays the same, I guess.

The best method of approach is to, you guessed it, bruteforce your way through in the form of sending an army of EXAs intermittently. Note that attempting to navigate an EXA back will not end well, so you're best to use the M register throughout, making sure that your EXA in your host does not attempt to send any values because this will ruin any flow you might have.

Each #NERV register contains a random value, and you're going to sort these in numerical order. I would advise sending out EXAs to grab all the host names with a #NERV in them and sorting them. I will also mention that, yes, you can sort these host names, since the first two values will always be the same, so it's only a matter of sorting the numbers in that name. Make sure that you leave dummy values between each host name so you can insert the value.

Once you've sorted hosts, it's now a matter of getting that value from the specified host. This will impact Activity if you decide to use this method of solving, as it will involve sending out about 10 waves of EXAs. However, unlike the first wave where you're waiting to collect every value from the wave, you're just listening out for one EXA that is in the correct host to give you that value.

Unlike other levels where you need to repeat ad infinitum, this one just requires you to map out the Cerebral Cortex once and that's it. Make sure you leave no trace.

Once completed, you will have finished the main story and move on to the bonus levels, as well as an Epilogue with your zines will be available.
	