## Code challenge 1 - maze

This is a fun little code challenge that you can make as quick or as complex as you like. Your maze can be an individual one or a shared maze where you compete with friends to complete the maze first. You can work with friends to work out how to solve the tricky mathematical challenges that you will come across. 

How much longer does the buggy have to rotate to the right? What would happen if we changed the speed to 65%?

--- task ---

The first step is to make your maze. It can be as small or as large as you like and as space allows.

Here is an example:

![Example maze](images/mazeChallenge_example.png)

This example probaly seems quite easy but getting your code right takes patient trial error. This one has small passages and needs just the right turns. Start off with something more simple that this and build with your successes!

--- /task ---

My maze has a green shape showing me where to start from on each run and to finish I just need to have any part of the buggy back in the purple box.

--- task ---

Once your maze is made, start with a `program start`{:class="crumblebasic"} block followed by `wait 1 second`{:class="crumblecontrol"} to allow you time to turn the battery pack on and move your hand away.

![Starting blocks](images/mazeChallenge_codeStep1.png)

--- /task ---

--- task ---

From here on you will need to code according to your maze problem.

You will either be going forward, turning left or turning right.

A turn to the right will usually involve the left motor going forward, but the right motor could either be stopped or, for a sharper turn, running in reverse. The opposite will be true for a left turn, the right motor runs forward while the left motor is stopped or in reverse.

In the example maze, the first move will be to turn to the left.

`motor 1`{:class="crumbleinputoutput"} (right-hand motor) `forwards`{:class="crumbleinputoutput"} will send me left. There is no need to stop the left-hand motor as it is not running yet.

![First motor block](images/mazeChallenge_codeStep2.png)

--- /task ---

--- task ---

Now add a `wait`{:class="crumblecontrol"} block to decide how long the buggy will turn for. The longer the `wait`{:class="crumblecontrol"}, the further it will rotate.

Note: Raising or lowering the `motor speed %`{:class="crumbleinputoutput"} will also affect the amount of rotation.

![First move wait time block](images/mazeChallenge_codeStep3.png)

--- /task ---

That's the first move done but you must always make sure you end by stopping the motors!

--- task ---

We only have `motor 1`{:class="crumbleinputoutput"} running but just to be sure, and for good practice, we will stop both motors.

Add two `motor`{:class="crumbleinputoutput"} blocks and toggle the boxes to get `motor 1 STOP`{:class="crumbleinputoutput"} and `motor 2 STOP`{:class="crumbleinputoutput"}.

![Stop motor blocks](images/mazeChallenge_codeStep4.png)

--- /task ---

The code so far only turns a bit left and stops. It doesn't even move forwards, but the best way to code a maze run is one step at a time. 

Code it and check it!

--- task ---

Run your code and check that you have a good `motor speed %`{:class="crumbleinputoutput"} and `wait`{:class="crumblecontrol"} time to get the right angle of rotation. If it is not good, adjust and check again.


--- /task ---

Because you will always start from the beginning of the maze. it is important to mark your start point clearly so you always start in excalty the same place and facing exactly the same way. Even a little change in starting angle will take you to a completely different place in the end.

![Start location marker](images/mazeChallenge_startLocation.png)

The next sequence of three blocks is a model for how this challenge goes from now on.

+ set motor 1
+ set motor 2
+ set the duration for the move

--- task ---

Start by pulling the `STOP`{:class="crumbleinputoutput"} blocks away from the code.

Since we are about to go forwards we set `motor 1`{:class="crumbleinputoutput"} and `motor 2`{:class="crumbleinputoutput"} to go `forwards`{:class="crumbleinputoutput"}. I am going to set them at `50%`{:class="crumbleinputoutput"} for now.

The last of the three steps in each move is to set the `duration`{:class="crumblecontrol"} of the move using a `wait`{:class="crumblecontrol"} block.

Enter a `wait`{:class="crumblecontrol"} time.

Don't forget toput the `STOP`{:class="crumbleinputoutput"} blocks back before you run the code.

![Add a forward sequence](images/mazeChallenge_codeStep5.png)

--- /task ---

The next move will be a turn to the right but we still follow the same pattern:

+ set motor 1
+ set motor 2
+ set the duration for the move

--- task ---

Remove the `STOP`{:class="crumbleinputoutput"} blocks.

For a right turn we need `motor 1`{:class="crumbleinputoutput"} to `STOP`{:class="crumbleinputoutput"} and `motor 2`{:class="crumbleinputoutput"} to go `forwards`{:class="crumbleinputoutput"}.

Then set the `duration`{:class="crumblecontrol"} for the turn.

Replace the `STOP`{:class="crumbleinputoutput"} blocks.

![Add a second turn sequence](images/mazeChallenge_codeStep6.png)

--- /task ---

Continue like this, adding a forwards sequence followed by a turn sequence and so on.

### Mistakes WILL happen

Now that I have added the next forward move, my test run shows me I have got it wrong.

--- no-print ---

![Buggy crashing into mug](images/mazeChallenge_crash.gif)

--- /no-print ---

--- print-only ---

![Buggy crashing into mug](images/mazeChallenge_crash.png)

--- /print-only ---

Each time something doesn't go as planned, you need to look carefully at where it went wrong and this is a good opportunity to look and see if you understand your code.

![Annotated code](images/mazeChallenge_codeStep7annotated.png)

 Since the last thing I added was the forward move, it is easy to think that this must be the problem but it was actually the turn before that was wrong. The buggy turned too far so it was pointing too close to the mug - the forward move is fine, I need to reduce the turn time!

Make sure that you have got your code right before going on to the next move, that way it is much easier to find what you need to change.

### Long lines of code

The code for this example maze got so long, adding three lines each time there was a new movement, that it went right off the bottom of the screen!

Redfern Electronics, who make the Crumble, plan to add a scroll bar so that you can move around the code workspace as you would in a web browser and many everyday apps but for now, all you need to do is click and drag on the white background to move around the workspace.

### The completed maze

Here is what the code looked like for the examplebuggy completing the example maze.

![Completed code](images/mazeChallenge_codeStep8finalCode.png)

--- no-print ---

And here is the buggy in action!

![Buggy completing the maze](images/mazeChallenge_completion.gif)

--- /no-print ---