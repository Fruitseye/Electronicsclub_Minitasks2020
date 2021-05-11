# RING
**Method used by you:**
- A push button to switch on the RGB LED circuit
- It is positioned such a way that it gets triggered when worn

**Problem:**
As mentioned,the push button will hurt the finger when wore for a long time

**Method I thought of:**
- A capacitive proximity detector like MTCH101 can be used.Data sheet is [here](https://docs.rs-online.com/c112/0900766b812bf39b.pdf)
- It operates in the voltage range desired(2.0V to 5.5V)
- The sensitivity of the sensor can be adjusted such that it produces output only when touched
- This detector can be support wide range of conductors as sensor.
- The ring can be designed such a way that a smaller inner ring(made of any conducting metal) can used as the proximity sensor using this detector
- If required,MCU like ATtiny can be used to control the LEDs and make it fade in/out,blink and to do various gimmicks.

**Reason of choice**
- A old metal ring of appropriate sixe can be used for this purpose rather than making a new ring form scratch since the ring itself can act as the proximity sensor
- IR is also a good choice.But in this case of using Capacitive proximity sensor,wherever the ring is touched,the ring gets activated
- There might be doubt whehther the ring will activate when kept on metal tables,etc.No,it won't activate because the sensing ring is present in the inner part.The outer part can be covered by nonconducting material
- The IC has low power mode option as well.So that it can sleep for longer time when nothing is detected

