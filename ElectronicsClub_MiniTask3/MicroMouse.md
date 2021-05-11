# MicroMouse
Ideation:
![Flow Chart](/flowchartmicro.PNG) \
**Sensors:**
- The choice of Time of flight sensor(also infrared) is actually good since it has 
    * faster transmission-reception times
    * long-range (<60 meters)
    * rapid refresh rates
    * lower power consumption
- Same TOF sensor is not recommended to be used in the front side of the mouse because TOF sensor's accuracy range is in centimetres
- Rather in the front Ultrasonic sensor/triangulation infrared sensor can be used

**Communication**
- Microcontroller:
   * We can go with usual arduino board since it has enough numbers of analog/digital/PWM and interrupt pins needed
   * Teensy Family MCUs have greater memory but main drawback is its cost
   * Another way to go about is to pick a microcontroller chip such as ATMega328 and incorporate it into our own custom-made PCB board, which can serve as frame/chassis(***Design problem solved :)*** ) for the robot.
   * Doing this can greatly reduce the overall size of your mouse.
   
**Locomotion**
 - DC motors can be used
 - Steppers motors not recommended as it reduces speed because of its weight
 - Motor drivers:The function of motor drivers is to take a low-current control signal and then turn it into a higher-current signal that can drive a motor.This can't be done by MCU directly
   
**Control**
- Using Flood fill algorithm for navigating the maze with shortest possible solution
- Using PID Controller algorithm to control the movement of mouse with the constantly updating error feedback


