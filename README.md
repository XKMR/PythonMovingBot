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
  adds or subtracts an amount based on the inputed steps to/from X and Y <br/>
   (moving the object in the direction that is's looking in)<br/>
   arguments: the current X, the current Y, the current direction, a number of steps<br/>
   returns: the new x,y
</p>
<h2>smturn</h2>
<p>
     simplifies the turn command by removing the need for inputing the current direction<br/>
   requires the turn() function to work, requires a variable named "currentDirection" to work<br/>
   arguments: "left"/"right"<br/>
   variables required to work: currentDirction<br/>
   functions required to work: turn()<br/>
   returns: 0
</p>
<h2>smforward():</h2>
<p>
     simplifies the turn command by removing the need for inputing anything other than the amount<br/>
   of steps that is going to be taken.<br/>
   arguments: int<br/>
   variables required to work: currentX, currentX, currentDirection<br/>
   functions required to work: forward()<br/>
   returns: 0
</p>
<h2>displayCurrentPlace():</h2>
<p>
   makes a 20x20 "screen" that will display the place and direction of the object.<br/>
   note that this needs some improvements<br/>
   arguments:<br/>
   variables needed to work: currentX, currentX, currentDirection<br/>
   returns: 0
</p>
<h1>variables:</h1>
   currentX:           the current position of the object on the X axis<br/>
   currentY:           the current position of the object on the Y axis<br/>
   currentDirection:   the current direction of the object ("up","down","left","right")
