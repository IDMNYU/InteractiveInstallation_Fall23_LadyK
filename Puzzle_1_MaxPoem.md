# Interactive Installation 

* **DM-GY 4913-B Special Topics: Interactive Installation**

## Challenge 1: Create a Poem with Max

Create a max patch that generates an unknown poem and prints out that poem to the Max console window. 
You are to also think about the performance of this poem. Think of this as the machine's performance. You are designing the structure for this random performance.

Load some text phrases or words as messages. Then trigger these messages to print in the console. 
Now think about how to vary the output and to make different choices or _selections_ by chosing a _random_ value (or _decide_). You will hit one button to start the performance of this poem. Think about the pacing of the words for emphasis, with _counter_ and _metro_. Take it to another level with _if_ statements, _join_ strings, _append_ and _prepend_, _gate_, _pack_,  _unpack_,....

Let's break this idea down into steps:

In order to do this, you will need to get a system going. Think: toggle, metro, bang/button. 

A poem is filled with words. We can use text within Max with a message box. We can print to the Max console with a print message.

Once you have a basic system printing out to the console, your next task to randomize it and to automate it. Your goal is to randomize it in a (some what) controlled (ie, performed) manner. 

We can assign a number, or a range of numbers, to each word. Then, when that number is chosen, we can output that word into our poem. Use these numbers to "select" a message box. The random object (and ones similar), can generate random values.

We need to think about how to massage this random object. Instead of just getting a blitz of numbers with the random object, can you get a random number within a range? Can you get a random number that is relative to the one that came before it? What about just getting X random values ("counter")? We only need certain random numbers, so we can use a "counter" to give us a certain number of options. We can always sprinkle in some math (see the unary and binary operators), and logical operators are available for your use.

We can take it to another level, and spice things up not only by making multiple units of these, but with combinations and "join"ing them together. Or, we can "pack" that word into a list to be "joined" with other words/"messages". We can take these lists of words and compare them to each other, filtering out repetitions, particular words, a place in a series of values. We can even scramble these lists. See the "zl" object. (Make sure to check out all the arguments that it can take.)

We can even make mad libs sections by "append"ing and "prepend"ing messages. So many options! Remember that every time you trigger a poem, it should be different that the one that came before it.

Think about the pacing of your bangs or selections. Perhaps some areas are more frequently generated. Perhaps some are generated more often. Use one metro object and a counter object with a % and a number to only bang when a zero is output and therefor "select"ed. In essence, you can have multiple metro's this way, through the use of only one metro.


Create an automated poem that utlizes something random/unexpected. The final output of the poem must be unknown to you. The poem *must print out to your Max Console window*.

You will want to have some bangs happen at regular intervals. What are they banging?

How can you add probabilty, selection, matching, etc to further diversify the outcome?

See the Max Patch - Poem Palette on Slack under "resources" to explore various objects and operations. Comment your code!

### Process:

* Review how Max works with the Luke's 10 Things patcher

* Get some messages to print to the window

* Read over this brief closely. It has hints as to which objects to look at to acheive these means. Focus on these objects only. Read each's help files and study how each object works individually. Then, start piecing different objects together, checking your work as you go.

* Explore different ways to automate the system

* Explore different ways to randomize, choose, manipulate, augment the poem and it's irregularity.

* submit your patch to your github repo label as FirstName_P1.maxpat

* write a post reflecting on this process. talk about what you've learned and where you are at.