# Reinforcement Learning based Hexapod
**Questions to be answered:**
- How to recreate the robot and its motion in a computer?
- How to obtain data from the sensor?
- What Microcontroller to use?
- And How to manage with the wires?
## Recreation part:
 - IMUs sensors can be attached to the bot to measure values of all 18 DOF
 - ROS packages can be implemented to collect the datas from IMUs
 - Blender software and ROS can be integrated to simulate the Hexapod in 3D real time
## Obtaining data from Sensor:
- IMU sensor like MPU6050([Datasheet](https://invensense.tdk.com/wp-content/uploads/2015/02/MPU-6000-Datasheet1.pdf)) can be used.
- This sensor contains a 3 axis MEMS accelerometer
and a 3 axis MEMS gyro in a single chip. 
- Talking about readings resolution, it contains 16-bits analog to digital
conversion hardware for each channel.
- Input voltage range: 2.3V-3.4V
## Microcontroller to use:
BotBoarduino microcontroller can be used \
Reasons:
- It is based on arduino
- Its specially designed to make these kind of bots
- One of the big advantage is that all of the I/O pins are replaced with standard three pins servo/sensor connections.
- This helps tremendously in reducing the forth coming problem that is managing with wires
## Managing with wires:
- For prototyping phase,we can go with normal wires
- If we move onto manufacturing phase,my idea is to use Spiral cable coiled spring in replacement of unshielded twisted pair cable 

