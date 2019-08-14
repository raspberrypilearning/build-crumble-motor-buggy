## Write a test program for the motors

Before you can start properly coding your motor buggy, you need to gather some information. You can find some of the information by looking at the buggy. To find the other information you need, you will write a test program.

You will use the test program to find the answers to the following questions:
+ Which motor output controls which gear motor?
+ When the right gear motor is programmed to go forwards, does the right-hand side of the buggy go forwards or backwards?
+ When the left gear motor is programmed to go forwards, does the left-hand side of the buggy go forwards or backwards?

If you use the code block that says `FORWARD`, the buggy does not necessarily move forwards.

The gear motors are not aligned in the same way. The left motor is a mirror image of the right motor, which means that if it has been wired up in the same way, i.e. positive to positive and negative to negative, it will make the attached wheel turn in the opposite direction!

![The left motor will turn in the opposite direction to the right motor](images/testCode_mirroredMotors-01.png)

--- task ---

First, check which Crumble motor output is connected to which gear motor. You could either use coding, or follow the wires from the gear motors to see where they lead.

In this example project:
+ Crumble motor 1 output controls the gear motor on the right-hand side
+ Crumble motor 2 output controls the gear motor on the left-hand side

--- /task ---

Next, use code to test whether a motor will go forward if it has been programmed to do so.

--- task ---

As usual, start your program with a `program start`{:class="crumblebasic"} block.

From the **Input/Output** blocks menu, take a `motor 1 FORWARD at 75%`{:class="crumbleinputoutput"} block and place it under your `program start`{:class="crumblebasic"} block.

Duplicate the `motor 1 FORWARD at 75%`{:class="crumbleinputoutput"} block, and toggle the `FORWARD`{:class="crumbleinputoutput"} part until the block reads, `motor 1 STOP`{:class="crumbleinputoutput"}.

Finally, between the two blocks that you have just added, add a `wait 100 milliseconds`{:class="crumblecontrol"} block from the **Control** blocks menu, and adjust the time to `wait 300 milliseconds`{:class="crumblecontrol"}.

![Test code for motor output 1](images/testCode_testCode1.png)

When you run the program, the motor on the right-hand side (in this example) should either move forwards or backwards.

--- no-print ---

![Running test code 1](images/testCode_runningTestCode1.gif)

--- /no-print ---

--- print-only ---

![Running test code 1](images/testCode_runningTestCode1.png)

--- /print-only ---

--- /task ---

Since the `motor 1 FORWARD` block makes the motor on the right-hand side go backwards, programming the motor 1 output to go backwards must make the motor on the right-hand side go forwards. Check that to make sure.

--- task ---

Toggle the `FORWARD`{:class="crumbleinputoutput"} part of the first `motor`{:class="crumbleinputoutput"} block until the block reads `motor 1 REVERSE at 75%`{:class="crumbleinputoutput"}.

![Test code 2 for motor output 1](images/testCode_testCode2.png)

Now, run the program to check that the motor runs in the opposite direction, i.e. forwards.

--- no-print ---

![Running test code 2](images/testCode_runningTestCode2.gif)

--- /no-print ---

--- print-only ---

![Running test code 2](images/testCode_runningTestCode2.png)

--- /print-only ---

--- /task ---

As long as you remember that `FORWARD`{:class="crumbleinputoutput"} means 'backwards' for the motor on the right-hand side, your code should work fine. But it would be easier if `FORWARD`{:class="crumbleinputoutput"} meant that the motor moved forwards.

Whether the motors go one way or another is simply a matter of polarity. In other words, it is a matter of which way round the positive and negative wires are connected. In the case of the motors, this is not important, so in this example, I will swap the positive and negative wires around. I could do this anywhere in the circuit, but I will do it where the crocodile clips meet the gear motor wires.

![Reversing the right motor polarity](images/testCode_crumbleMotorRReversePolarity-01.png)

**WARNING**: It is safe to reverse the polarity on these gear motors but in other situations, reversing the positive and negative polarity can damage components.

--- task ---

Run your last code, `motor 1 REVERSE`{:class="crumbleinputoutput"}, again to see if the motor now runs in reverse when programmed to do so.

--- no-print ---

![Running test code 2 again](images/testCode_runningTestCode2b.gif)

--- /no-print ---

--- print-only ---

![Running test code 2 again](images/testCode_runningTestCode2b.png)

--- /print-only ---

--- /task ---

Now that the motor on the right-hand side does what it is told to do, it is time to do the same for the motor on the left-hand side.

--- task ---

Toggle the `1`{:class="crumbleinputoutput"} part of both `motor`{:class="crumbleinputoutput"} blocks so that they read `motor 2`{:class="crumbleinputoutput"}, so that you can test the gear motor on the left-hand side.

Then, toggle the `REVERSE`{:class="crumbleinputoutput"} part of the first `motor`{:class="crumbleinputoutput"} block until the block reads `motor 2 FORWARD at 75%`{:class="crumbleinputoutput"}.

![Test code 3 for motor output 2](images/testCode_testCode3.png)

Run the program.

--- no-print ---

![Running test code 3](images/testCode_runningTestCode3.gif)

--- /no-print ---

--- print-only ---

![Running test code 3](images/testCode_runningTestCode3.png)

--- /print-only ---

--- /task ---

Since the gear motor on the left-hand side goes forwards when programmed to go `FORWARD`{:class="crumbleinputoutput"}, you do not need to reverse the polarity.

You now know that, in this example project:

+ Motor 1 output forward makes the wheel on the right-hand side go forwards.
+ Motor 1 output reverse makes the wheel on the right-hand side go backwards.
+ Motor 2 output forward makes the wheel on the left-hand side go forwards.
+ Motor 2 output reverse makes the wheel on the left-hand side go backwards.

Now, write a program to check.

--- task ---

Duplicate the `motor`{:class="crumbleinputoutput"} and `wait`{:class="crumblecontrol"} blocks as needed to write a program that tells motors `1` and `2`{:class="crumbleinputoutput"} to go `FORWARD`{:class="crumbleinputoutput"}, then `wait for 0.3 seconds`{:class="crumblecontrol"}, then tells both motors to `REVERSE`{:class="crumbleinputoutput"}, then `wait for 0.3 seconds`{:class="crumblecontrol"} again before both motors `STOP`{:class="crumbleinputoutput"}.

![Test code 4 for both motors](images/testCode_testCode4.png)

Run the program.

--- no-print ---

![Running test code 3](images/testCode_runningTestCode4.gif)

--- /no-print ---

--- print-only ---

![Running test code 3](images/testCode_runningTestCode4.png)

--- /print-only ---

--- /task ---

You now have all of the information you need to write a program and control what your motor buggy does!
