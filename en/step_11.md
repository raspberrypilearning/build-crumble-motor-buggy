## Code challenge 1 - Crumball

Crumball is like football, but played with Crumbles instead of feet.

Its basic coding is much like the maze challenge but with shorter code and added pressure!

This is coding against the clock, or rather, coding against your opponent. The game is designed for two Crumble motor buggies but you could try it with more and you can always practice on your own too.

### The game

As with football, you need a pitch with a goal at each end.

The ball starts in the middle and the object of the game is to knock the ball into the opposite goal.

Players always start off in a set position just to side of their goal facing directly forward. The coders must write code to score a goal as quickly as they can to beat their opponent. 

As soon as your code is done and loaded,  you can unplug your Crumble, put your buggy in its set position facing forward and off it goes.

Once a Crumble is set in motion:

+ it must complete its code without being stopped, interrupted or picked up
+ as soon as the Crumble has completed running its code it must be removed from the pitch so that it does not block the other player
+ once removed it is time to start coding again straight away for your next shot

If you are too slow with your coding, the other player might have moved the ball with their Crumble and your code will need changing.

Note: every shot starts from the same set position and always facing directly forwards!

--- task ---

Make a Crumball pitch.

![Crumball pitch](images/CrumballChallenge_pitch.png)

A large sheet of paper would be fine but often it's easiest to mark a pitch out on the floor with masking tape or similar.

Use anything handy for goal posts and any small ball will do for the Crumball itself.

Mark the set positions for each player's buggy. In the example there are little arrows on masking tape to show the position each wheel starts in.

![Crumball player markers](images/CrumballChallenge_playerMarkers.png)

--- /task ---

### Time to get coding!

Your code will depend on the shot you want to make and where the ball is but in general there is a simple code structure that you can write and then adapt for any shot.

![Crumball shot aim](images/CrumballChallenge_basicAim.png)

+ rotate to space in front of the ball
+ move towards that space ball
+ rotate to the angle you want the move the ball in
+ move forward directly at the goal
+ stop motors

Do remember to stop the motors!

--- task ---

Get the usual start blocks, a `program start`{:class="crumblebasic"} and a `wait 1 second`{:class="crumblecontrol"} block.

![Crumball start blocks](images/CrumballChallenge_codeStep1.png)

--- /task ---

Now the rotation to the space in front of the ball.

--- task ---

Two `motor`{:class="crumbleinputoutput"} blocks and a `wait`{:class="crumblecontrol"}.

One `motor`{:class="crumbleinputoutput"} will be going `forward`{:class="crumbleinputoutput"} and the other in `reverse`{:class="crumbleinputoutput"} depending on the way you want to turn. You'll soon know if you get them the wrong way round.

Set the `wait`{:class="crumblecontrol"} block to however long you think it will take to get to the right angle.

![Rotating towards the ball](images/CrumballChallenge_codeStep2.png)

--- /task ---

Next, move to where the ball is.

--- task ---

Again, two `motor`{:class="crumbleinputoutput"} blocks and a `wait`{:class="crumblecontrol"}.

Both `motors`{:class="crumbleinputoutput"} will be going `forward`{:class="crumbleinputoutput"}.

Set the `wait`{:class="crumblecontrol"} block to however long you think it will take to get just in front of the ball.

![Moving to the ball](images/CrumballChallenge_codeStep3.png)

--- /task ---

Then, rotate to the direction you want to knock the ball.

--- task ---

As with every move in this game, two `motor`{:class="crumbleinputoutput"} blocks and a `wait`{:class="crumblecontrol"}.

Set the correct `motors`{:class="crumbleinputoutput"} to `forward`{:class="crumbleinputoutput"} and `reverse`{:class="crumbleinputoutput"} to turn in the correct direction.

Set the `wait`{:class="crumblecontrol"} time.

![Turn to face the goal](images/CrumballChallenge_codeStep4.png)

--- /task ---

Now push the ball forwards towards the goal.

--- task ---

Set both `motors`{:class="crumbleinputoutput"} to go `forward`{:class="crumbleinputoutput"} for however many `seconds`{:class="crumblecontrol"} you think it will take to score a goal.

Remember that you cannot get your buggy back until it stops moving so don't drive to far!

![Move towards the goal](images/CrumballChallenge_codeStep5.png)

--- /task ---

Don't forget to stop!

--- task ---

Set both `motors`{:class="crumbleinputoutput"} to `STOP`{:class="crumbleinputoutput"}

![Stop the motors](images/CrumballChallenge_codeStep6.png)

--- /task ---

That's the code that should form the basic structure of every shot you take. You don't need to write it again for each shot, just see what went wrong with your last shot and adjust the `speed`{:class="crumbleinputoutput"} or the `move time`{:class="crumblecontrol"}.

### Kick-off!

--- task ---

As soon as you have your code, unplug and take your shot. Try and score a goal before your opponent is ready.

Good luck!

--- no-print ---

![Crumball first shot](images/CrumballChallenge_firstShot.gif)

--- /no-print ---

--- print-only ---

![Crumball first shot](images/CrumballChallenge_firstShot.png)

--- /print-only ---

--- /task ---

My first shot went very wrong and it is unlikely to go right first time. 

My initial turn time was much too long, so I adjust my code and try again. My speeds were often at 100% and that also makes it hard to control. Find a balance between speed to beat your opponent and getting things right.

By working out what you need to change to get a better aim, you will soon be getting some great shots in. You don't have to win the match in one shot!

--- no-print ---

![Crumball first shot](images/CrumballChallenge_winningShot.gif)

--- /no-print ---

