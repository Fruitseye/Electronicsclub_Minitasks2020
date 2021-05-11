# Debugging Phase
**Bot going sideways:**
   - Make sure the wheels are straight and parallel to each other
   - Code need to be tweaked for handling different speeds of the wheel and make it same if thats the reason
   
**Bot chassis:**
   - If the space is not sufficient in the chassis to keep the electronic circuits,then it needs to modified to accomodate stuffs
   
**Uneven Loads:**
   - The robot would have been programmed to produce tilt feedbacks which will be accurate only when centre
   of gravity coincides with geometrical/physical centre of robot
   - To tackle problems due to uneven loads,add something like a push button that zeros the desired tilt angle whenever it is pressed, 
   in order to enable calibration of the robot for uneven loads that may move the center of gravity off from the physical
   center of the robot.
   
**Hardware**
   - Multimeters can be used to check for checking break in current flow and to find faulty components
   
**Software debugging:**
   - Check for the main culprit ";" \
    <img width="200" alt="portfolio_view" src="https://i.pinimg.com/originals/2b/87/17/2b8717e385f04061c8b6b78cd4c663c7.png">
   - Then check if the variables are initialised before using,etc
   - Now coming to the algorithmic part:
      - For debugging purposes, LCD display can be used to display the current tilt, rotation rate and other parameters that can be tuned via onboard potentiometers.
      - Or to be cost efficient,we can go about debugging with Serial communication
      - From Serial Monitor output, we can compare the output values. For eg: when the robot is still(perpendicular to ground), acceleration along Y and Z should be zero and that along X should be approximately equal to g(9.8). Similarly, the output can be checked for different positions.
      
**NONE OF THE ABOVE**
   - If none of the debugging works,or if the components are damaged.....
   - BUY A NEW ONE
