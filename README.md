# PythonMovingBot
this is a script for simulating a object with a direction that can move in said direction
# functions:
<h2>turn():</h2>
<p>
    turnes the object by 90 degrees clockwise or counterclockwise<br/>
    arguments should be: "CC/CW", the current direction<br/>
    returns: the new direction ("up" , "down" , "left" , "right")
</p>
<h2>forward():</h2>
<p>
  adds or subtracts an amount based on the inputed steps to/from X and Y 
   (moving the object in the direction that is's looking in)
   arguments: the current X, the current Y, the current direction, a number of steps
   returns: the new x,y
</p>
<h2>smturn</h2>
<p>
     simplifies the turn command by removing the need for inputing the current direction
   requires the turn() function to work, requires a variable named "currentDirection" to work
   arguments: "left"/"right"
   variables required to work: currentDirction
   functions required to work: turn()
   returns: 0
</p>
<h2>smforward():</h2>
<p>
     simplifies the turn command by removing the need for inputing anything other than the amount
   of steps that is going to be taken.
   arguments: int
   variables required to work: currentX, currentX, currentDirection
   functions required to work: forward()
   returns: 0
</p>
<h2>displayCurrentPlace():</h2>
<p>
   makes a 20x20 "screen" that will display the place and direction of the object.
   note that this needs some improvements
   arguments:
   variables needed to work: currentX, currentX, currentDirection
   returns: 0
</p>
<h1>variables:</h1>
   currentX:           the current position of the object on the X axis
   currentY:           the current position of the object on the Y axis
   currentDirection:   the current direction of the object ("up","down","left","right")
