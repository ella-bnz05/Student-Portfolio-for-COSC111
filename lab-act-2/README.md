# Student-Portfolio-for-COSC111


## Laboratory Activity 2 

Objectives:

  1. Discuss analog signals and its implementation in a Arduino circuit.
  2. Understand analog to digital signal conversion using the map() function.

The objective of this project is to create a running light effect using multiple LEDs. The LEDs will gradually increase in brightness and then turn off one by one, creating a smooth transition effect.

Description:

The logic is same with the first activity but in this one, there will be five different LEDs with resistors that connected to the pins 8 to 12 of the Arduino Uno board. To execute the program, first, connect the LEDs to the Arduino as shown in A2-Diagram.png. Then, upload the code to the Arduino IDE, ensuring the correct port is selected. Finally, run the code to observe the LED sequence in action.


The code creates a running light effect, where the LEDs gradually brighten before turning off one by one, producing a smooth transition.
The additional components of the code that you need to understand are the following:
-LedON() Function – Gradually increases the brightness of each LED using analogWrite() until it reaches a mapped target value, resulting in a smooth fade-in effect.
-LedOFF() Function – Sequentially turns off each LED with a delay between actions.
-map() Function – Transforms the LED index value (i) into a specific brightness level. For example, map(i, 0, numLeds - 1, 50, 255) converts the index i (from 0 to 4) into a brightness range between 50 and 255, enabling smoother transitions.
-analogWrite() Function – Controls the brightness of an LED by setting a PWM (Pulse Width Modulation) value between 0 (off) and 255 (full brightness). This function allows for smooth dimming and brightening, creating a fade effect.