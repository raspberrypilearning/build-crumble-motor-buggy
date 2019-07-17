## Speed and spins

We have already looked at how to make your motor buggy go forwards and backwards. Now we are going to look at controlling the speed as well as turning left and right.

### Controlling the speed

--- task ---

Starting, of course, with a `program start`{:class="crumblebasic"} block, add two `motor`{:class="crumbleinputoutput"} blocks, one for `motor 1`{:class="crumbleinputoutput"} and the other for `motor 2`{:class="crumbleinputoutput"}.

Add a `wait`{:class="crumblecontrol"} block and change it to `wait 300 milliseconds`{:class="crumblecontrol"}.

![Turning both motors on code](images/speedAndSpins_speedControlCodeStep1.png)

--- /task ---

--- task ---

Duplicate these three blocks and place them beneath the existing ones. 

Change the `motor`{:class="crumbleinputoutput"} speed to `50%`{:class="crumbleinputoutput"} and the `wait`{:class="crumblecontrol"} time to `600 milliseconds`{:class="crumblecontrol"}.

![Turning both motors on and changing speed code](images/speedAndSpins_speedControlCodeStep2.png)

--- /task ---

--- task ---

Now duplicate the last three blocks and place them at the bopttom of your code. 

Change the `motor`{:class="crumbleinputoutput"} speed to `25%`{:class="crumbleinputoutput"} and the `wait`{:class="crumblecontrol"} time to `1200 milliseconds`{:class="crumblecontrol"}.

![Turning both motors on and changing speed twice code](images/speedAndSpins_speedControlCodeStep3.png)

--- /task ---

--- task ---

Lastly, add two `motor`{:class="crumbleinputoutput"} blocks telling the motors to `STOP`{:class="crumbleinputoutput"}.

![Turning both motors on, changing speed twice and stopping code](images/speedAndSpins_speedControlCodeStep4.png)

Run your code and see the buggy run at three different speeds.

If the change is too quick, make longer waiting times and run it again.

--- no-print ---

![Running speed control code](images/speedAndSpins_runningSpeedControlCode.gif)

--- /no-print ---

--- print-only ---

![Running speed control code](images/speedAndSpins_runningSpeedControlCode.png)

--- /print-only ---

--- /task ---

### Set your Crumble free!

My Crumble motor buggy ran off the edge of mydesk which tells me it is time to look at unplugging the Crumble and setting it free to roam on the floor.

While the Crumble is plugged in to your computer it is getting continuous power through the USB cable and so turning your battery pack on or off does not turn the Crumble on and off but when you unplug the USB cable, whatever code was last run on your Crumble will run as soon as the battery pack is turned on.

In this case, the Crumble buggy will start moving forward at slower and slower speeds until, after 2.1 seconds, it stops.

The problem with the code we have at the moment is that the motors will want to start the moment I switch the power on and won't even give me time to get my hands out of the way!

--- task ---

Add a short `delay`{:class="crumblecontrol"} to the beginning of your code to give you time to get your hands out the way when turning your battery pack on.

![Added wait at start of code](images/speedAndSpins_speedControlCodeWithAddedWait.png)

Run your code to transfer the changes to the Crumble controller, turn the battery pack off and unplug the USB cable.

Find yourself a bit of space and turn the battery pack on to set your buggy in motion.

--- no-print ---

![Running speed control code without USB cable](images/speedAndSpins_runningSpeedControlCodeUnplugged.gif)

--- /no-print ---

--- print-only ---

![Running speed control code without USB cable](images/speedAndSpins_runningSpeedControlCodeUnplugged.png)

--- /print-only ---

--- /task ---

### Turning right and turning left

