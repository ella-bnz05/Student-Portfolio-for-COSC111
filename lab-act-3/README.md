# Student-Portfolio-for-COSC111


## Laboratory Activity 3

Objectives:

  1. Integrate the sensors components (thermistor, photoresistor) in an Arduino circuit.
  2. Create a simple implementation of a fire sensor.


Description:

This Arduino program monitors temperature and ambient light levels using a temperature sensor and a photoresistor. If the temperature exceeds a defined threshold and the brightness level is high, the system triggers a fire indication by blinking an LED rapidly. The program continuously reads sensor values, prints them to the serial monitor, and evaluates conditions to determine whether to activate the LED warning system.

To execute the program, first, diagram shown in A3-Diagram.png. Then, upload the code to the Arduino IDE, ensuring the correct port is selected. Finally, run the code to observe the basic fire sensor. If both temperature and brightness exceed the defined thresholds, the LED will blink rapidly to indicate that there is a potential fire. Open the serial monitor to observe temperature and brightness readings. 

Note: To open the Serial Monitor use Ctrl + Shift + M. 