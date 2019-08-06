## Create random journey that is even more random!

In the last step, you made a repeat loop with three basic steps:
+ Move a random distance
+ Turn right in a random rotation
+ Turn left in a random rotation

It would make more sense to simply turn either left or right by a random amount,  so that's what you are going to do next!

--- task ---

Start with the code that you had at the end of the last step.

![Random journey 1 code](images/randomJourney1_codeStep10.png)

--- /task ---

This is a recap of what each part of the code does:

![Random journey 1 code breakdown](images/randomJourney2_codeBreakdown.png)

--- task ---

First, separate and pull out the sections that turn right and turn left.

![Pull out turn sections](images/randomJourney2_codeStep1.png)

--- /task ---

From now on, you will use either the right turn or the left turn, but not both.

Next, you will make a variable to help the program decide which direction to turn in.

--- task ---

In the **Variables** blocks menu, click `Add New Variable`{:class="crumblevariables"}.

Enter a name that describes what the variable will be used for, such as `direction` or `right or left?`. In this example, the variable will be called `direction`.

**Note**: It doesn't matter to the computer or the Crumble what the variable is called, but it is best to choose a name that will help you understand what the variable is for.

![New variable called direction](images/randomJourney2_codeStep2.png)

--- /task ---

--- task ---

Take a `let   = 0`{:class="crumblevariables"} block from the **Variables** blocks menu and add a `direction`{:class="crumblevariables"} block into the empty space.

![Set the direction variable](images/randomJourney2_codeStep3.png)

--- /task ---

--- task ---

Take a `random number`{:class="crumbleoperators"} block and put it in the `let direction = 0`{:class="crumblevariables"} value box, then set the range from `1`{:class="crumbleoperators"} to `2`{:class="crumbleoperators"}.

![New variable called direction](images/randomJourney2_codeStep4.png)

--- /task ---

This means that for each `repeat`{:class="crumblecontrol"} cycle, the `direction`{:class="crumblevariables"} variable will be set to either `1`{:class="crumbleoperators"} or `2`{:class="crumbleoperators"}.

The program will be set up as follows:
+ `if`{:class="crumblecontrol"} `direction =`{:class="crumblevariables"} `1`{:class="crumbleoperators"} `then`{:class="crumblecontrol"} `turn right`{:class="crumbleinputoutput"}
+ `else`{:class="crumblecontrol"}  (i.e.`if`{:class="crumblecontrol"} `direction =`{:class="crumblevariables"} `2`{:class="crumbleoperators"} `then`{:class="crumblecontrol"}) `turn left`{:class="crumbleinputoutput"}

First, you will ask `if`{:class="crumblecontrol"} `direction =`{:class="crumblevariables"} `1`{:class="crumbleoperators"}.

--- task ---

Take an `if... then... else...`{:class="crumblecontrol"} block from the **Control** blocks menu. Add it under the `variable`{:class="crumblevariables"} setting block.

Add a `0 = 0`{:class="crumbleoperators"} block in the hexagonal space.

Place a `direction`{:class="crumblevariables"} variable block in the place of the first `0`{:class="crumbleoperators"} and change the second `0`{:class="crumbleoperators"} to `1`{:class="crumbleoperators"}.

![New variable called direction](images/randomJourney2_codeStep5.png)

--- /task ---

The `if... then... else...`{:class="crumblecontrol"} block has two open sections waiting for code. 
+ The first is for what happens if the condition is true, i.e. `if`{:class="crumblecontrol"} `direction`{:class="crumblevariables"} does `equal`{:class="crumblevariables"} `1`{:class="crumbleoperators"}
+ The second, the `else`{:class="crumblecontrol"} part, is for what happens `if`{:class="crumblecontrol"} `direction`{:class="crumblevariables"} does **not** `equal`{:class="crumblevariables"} `1`{:class="crumbleoperators"}.

--- task ---

Inside the `if direction = 1 then` block, add the code that you wrote earlier to make your buggy turn right.

![New variable called direction](images/randomJourney2_codeStep6.png)

--- /task ---

--- task ---

Next, inside the `else`{:class="crumblecontrol"} block, add the code that you wrote to make your buggy turn left.

![New variable called direction](images/randomJourney2_codeStep7.png)

--- /task ---

Now, run your program.

--- no-print ---

![Running random journey 2 code](images/randomJourney2_finalRun.gif)

--- /no-print ---
