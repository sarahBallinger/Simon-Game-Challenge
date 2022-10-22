# Simon-Game-Challenge
Single player pattern mirroring game involving sounds and colors.

# Description:

This challenge required an understanding of HTML, CSS & basic javascript.

# What I Learned:

**How to implement a handler function**

I needed to use jQuery to detect when a button was clicked and trigger a handler function. A handler does an action once an event occurs, in this case the event is a mouse click. Inside the handler function I created the variable "userChosenColor to store the id of the button that was clicked. These values were then stored in an empty array called userClickedPattern in order to use this pattern later on to check accuracy against the correct game pattern.

**Tricky if else Statements**

At this point the game was storing the user pattern as well as to game pattern, now I needed to compare those arrays to determine if the user was correct. first I created a function checkAnswer() that took one input of currentLevel. checkAnswer() was called after the user has clicked their answer, and the index of their last chosen answer gets passed into the user sequence. I used an if else statement first checking if userClickedPattern[currentLevel] === gamePattern[currentLevel]. If this was true, then it checked to see if the arrays were the same length, if true then it went to the next level. if the first if userClickedPattern[currentLevel] === gamePattern[currentLevel] was false, the game restarts by calling startOver() which sets all paramaters back to zero and arrays to empty.
