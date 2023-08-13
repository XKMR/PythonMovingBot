# PythonMovingBot
this is a script for simulating a object with a direction that can move in said direction
## demo:
```py
#this is a demo program

try:
    while(True):
        smturn("right")
        print(displayCurrentPlace(currentX, currentY, currentDirection))
        sleep(0.5)
        for i in range(11): 
            smforward(1)
            print(displayCurrentPlace(currentX, currentY, currentDirection))
            sleep(0.1)
except KeyboardInterrupt:
    print("X: ",currentX," Y: ",currentY)
    print("pointing at ", currentDirection)
```
## functions:
### turn():

    turnes the object by 90 degrees clockwise or counterclockwise
    arguments should be: "CC/CW", the current direction
    returns: the new direction ("up" , "down" , "left" , "right")

### forward():

    adds or subtracts an amount based on the inputed steps to/from X and Y 
    (moving the object in the direction that is's looking in)
    arguments: the current X, the current Y, the current direction, a number of steps
    returns: the new x,y

### smturn():

    simplifies the turn command by removing the need for inputing the current direction
    requires the turn() function to work, requires a variable named "currentDirection" to work
    arguments: "left"/"right"
    variables required to work: currentDirction
    functions required to work: turn()
   returns: 0

### smforward():

    simplifies the turn command by removing the need for inputing anything other than the amount
    of steps that is going to be taken.
    arguments: int
    variables required to work: currentX, currentX, currentDirection
    functions required to work: forward()
    returns: 0

### displayCurrentPlace():
> :warning: **WARNING!** the code for this function needs some improvements


    makes a 20x20 "screen" that will display the place and direction of the object.
    arguments:
    variables needed to work: currentX, currentX, currentDirection
    returns: 0

## variables:
    currentX:           the current position of the object on the X axis
    currentY:           the current position of the object on the Y axis
    currentDirection:   the current direction of the object ("up","down","left","right")
