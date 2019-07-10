## Forwards, backwards, right and left

We have already looked at how to make your motor buggy go forwards and backwards. Now we are going to look at controlling the speed as well as turning left and right.

### Controlling the speed

--- task ---

Starting, of course, with a `program start`{:class="crumblebasic"} block, add two `motor`{:class="crumbleinputoutput"} blocks, one for `motor 1`{:class="crumbleinputoutput"} and the other for `motor 2`{:class="crumbleinputoutput"}.

Add a `wait`{:class="crumblecontrol"} block and change it to `wait 300 milliseconds`{:class="crumblecontrol"}.

![Turning both motors on code](images/rightLeft_speedControlCodeStep1.png)

--- /task ---

--- task ---

Duplicate these three blocks and place them beneath the existing ones. 

Change the `motor`{:class="crumbleinputoutput"} speed to `50%`{:class="crumbleinputoutput"} and the `wait`{:class="crumblecontrol"} time to `600 milliseconds`{:class="crumblecontrol"}.

![Turning both motors on and changing speed code](images/rightLeft_speedControlCodeStep2.png)

--- /task ---

--- task ---

Now duplicate the last three blocks and place them at the bopttom of your code. 

Change the `motor`{:class="crumbleinputoutput"} speed to `25%`{:class="crumbleinputoutput"} and the `wait`{:class="crumblecontrol"} time to `1200 milliseconds`{:class="crumblecontrol"}.

![Turning both motors on and changing speed twice code](images/rightLeft_speedControlCodeStep3.png)

--- /task ---

--- task ---

Lastly, add two `motor`{:class="crumbleinputoutput"} blocks telling the motors to `STOP`{:class="crumbleinputoutput"}.

![Turning both motors on, changing speed twice and stopping code](images/rightLeft_speedControlCodeStep4.png)

Run your code and see the buggy run at three different speeds.

If the change is too quick, make longer waiting times and run it again.

--- /task ---

--- no-print ---

![Running speed control code](images/rightLeft_runningSpeedControlCode.gif)

--- /no-print ---

--- print-only ---

![Running speed control code](images/rightLeft_runningSpeedControlCode.png)

--- /print-only ---

### Right and left

