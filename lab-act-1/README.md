# Student-Portfolio-for-COSC111


## Laboratory Activity 1 

Objectives:

  1. To implement digital signals in a Arduino circuit.
  
  2. To create a sequential LED lighting system where LEDs turn on and off in a specific order. The system can be modified to control odd or even-numbered LEDs separately.

Description:

In this activity, we created an Arduino circuit consisting of five LEDs with resistors connected to the Arduino Uno board. The code enabled the LEDs to turn on and off sequentially with a delay between each action. In order for it to run, you should connect the LEDs first to the Arduino like the one in act1.png, then upload the code to the Arduino IDE, make sure that you checked and selected the right port. Run the Code to observe the LED sequence with a 1-second delay. You can also modify for Odd/Even LEDs by adjusting the loop function. The code for odd and even LEDs are also on the .ino file on this folder.

The key components of the code that you need to understand are the following:
- LED Pins (ledPins[]): An array specifying the pins connected to the LEDs. 
- Number of LEDs (numLeds): The total count of LEDs in the setup.
- Setup: Configures each LED pin as an output.
- Loop: Manages the sequence of turning the LEDs on and off.


