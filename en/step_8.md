## Random journey 1

Now you are going to code a random journey for your Crumble buggy using the `motor`{:class="crumbleinputoutput"}, `wait`{:class="crumblecontrol"} and `random`{:class="crumbleoperators"} blocks.

--- task ---

We start with, you guessed it, the `program start`{:class="crumblebasic"} block and add two `motor`{:class="crumbleinputoutput"} blocks, one for `motor 1`{:class="crumbleinputoutput"} and the other for `motor 2`{:class="crumbleinputoutput"}.

Add a `wait 100 milliseconds`{:class="crumblecontrol"} block.

![Turning both motors on code](images/randomJourney1_codeStep1.png)

--- /task ---

Now it's time to put in our first random factors.

We are going to randomise the speeds at which the motors move and the time they run for.

Since it is likely that the two motors will have different speeds the buggy is likely to not drive straight forwards.

--- task ---

Pick a `random 0 to 10`{:class="crumbleoperators"} block from the `Operators`{:class="crumbleoperators"} palette.

Place it in the speed section of the first `motor`{:class="crumbleinputoutput"} block and set the number range from `50`{:class="crumbleoperators"} to `80`{:class="crumbleoperators"}.

![First random speed block](images/randomJourney1_codeStep2.png)

--- /task ---

--- task ---

Duplicate the `random 50 to 80`{:class="crumbleoperators"} block and place it the speed control of the second `motor`{:class="crumbleinputoutput"} block.

![Second random speed block](images/randomJourney1_codeStep3.png)

--- /task ---

--- task ---

Duplicate either of the `random 50 to 80`{:class="crumbleoperators"} blocks, place it the `wait`{:class="crumblecontrol"} block and set the range from `500`{:class="crumbleoperators"} to `2000`{:class="crumbleoperators"}. That is half a second to two seconds.

![Random wait block](images/randomJourney1_codeStep4.png)

--- /task ---

This is a good time to test the code so far, but before we do that we need to add code to `stop`{:class="crumbleinputoutput"} the `motors`{:class="crumbleinputoutput"} and a short `wait`{:class="crumblecontrol"} at the start of our code.

--- task ---

Add a `2 second wait`{:class="crumblecontrol"} at the start of the code.

Get two `motor`{:class="crumbleinputoutput"} blocks and set `motors 1 and 2`{:class="crumbleinputoutput"} to `stop`{:class="crumbleinputoutput"}. Add them to the end of your code so far

![Added motor blocks](images/randomJourney1_codeStep5.png)

Go through the usual routine of checking the battery power is off, click play, unplug and then test your code.

Run it a few times to see the variation in speeds and times.

--- no-print ---

![Running first random journey test](images/randomJourney1_firstTestRun.gif)

--- /no-print ---

--- print-only ---

![Running first random journey test](images/randomJourney1_firstTestRun.png)

--- /print-only ---

--- /task ---

Now to code the some random turns. In this example we will turn right and then turn left. Since the turns are random, the buggy is likely to turn further one way than the other.

--- task ---

First things first, the `stop`{:class="crumbleinputoutput"} blocks need to always be at the end of the code so let's pull them away while we are working on the rest of our programme.

![Separate the stop block](images/randomJourney1_codeStep6.png)

--- /task ---

--- task ---

Duplicate the whole `random`{:class="crumbleoperators"} moving section including both `motor`{:class="crumbleinputoutput"} blocks and the `random`{:class="crumbleoperators"} `wait`{:class="crumblecontrol"}.

Keep them separate from your main code for now.

![Dulplicated motion block](images/randomJourney1_codeStep7.png)

--- /task ---

--- task ---

To make a right-hand turn, toggle the `motor 1`{:class="crumbleinputoutput"} block to `reverse`{:class="crumbleinputoutput"}.

Change the `wait`{:class="crumblecontrol"} time to between `100`{:class="crumbleoperators"} and `1500 millisenconds`{:class="crumbleoperators"}.

![Right turn block](images/randomJourney1_codeStep8.png)

--- /task ---

--- task ---

To make a left-hand turn, duplicate the right-hand turn blocks that you have just made, toggle the `motor 1`{:class="crumbleinputoutput"} block to `forward`{:class="crumbleinputoutput"} and the `motor 2`{:class="crumbleinputoutput"} block to `reverse`{:class="crumbleinputoutput".

Now join up your blocks - the `forward`{:class="crumbleinputoutput"}, `right turn`{:class="crumbleinputoutput"} and `left turn`{:class="crumbleinputoutput"} sections only leaving aside the `stop`{:class="crumbleinputoutput"} blocks.

![Random single run code](images/randomJourney1_codeStep9.png)

--- /task ---

You're almost there. You have a random forward move, a random right-hand turn and a random left-hand turn. The only thing left to do is make it carry on doing that again.

--- task ---

Pull your main code below the `wait 2.0 seconds`{:class="crumblecontrol"} away in to a little space.

Put all of this main code into a `do 10 times`{:class="crumblecontrol"} loop. That's the `forward`{:class="crumbleinputoutput"}, `right turn`{:class="crumbleinputoutput"} and `left turn`{:class="crumbleinputoutput"} sections all in the `repeat`{:class="crumblecontrol"} loop.

Add the loop to the `program start`{:class="crumblebasic"} and the `wait 2 seconds`{:class="crumblecontrol"}blocks. 

Now add the `stop`{:class="crumbleinputoutput"} blocks to the end of the code.

Note: If you only have a very small space for your buggy, make the `forward`{:class="crumbleinputoutput"} `wait`{:class="crumblecontrol"} time smaller, e.g. between `100`{:class="crumbleoperators"} and `500 millisenconds`{:class="crumbleoperators"}.

![Random repeat run code](images/randomJourney1_codeStep10.png)

--- /task ---

--- task ---

Run your code and adjust it if you think anything needs changing.

--- no-print ---

![Running repeat random journey code](images/randomJourney1_finalRun.gif)

--- /no-print ---

--- print-only ---

![Running repeat random journey code](images/randomJourney1_finalRun.png)

--- /print-only ---

--- /task ---