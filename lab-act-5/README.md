# Student-Portfolio-for-COSC111


## Laboratory Activity 5

Objectives:

  1. Understand and implement Arduino Serial Connection
  2. Utilize Python as a tool for implementing serial connection
  3. Create a simple circuit that can be controlled using Serial connection using Arduino and Python

Prerequisites


● Arduino board.


● USB cable to connect the Arduino to your computer.


● Arduino IDE installed on your system.


● Python (3.x) with pySerial, requests and FastAPI installed.


pip install pyserial requests fastapi[standard]




Description:

TThis project establishes a serial communication interface between a FastAPI backend and an Arduino board to remotely control an LED via HTTP requests. The FastAPI server sends commands to the Arduino through a serial connection, allowing users to turn the LED on and off using API endpoints.

To execute the program, first, diagram shown in A5-Diagram.png. Then, upload the code to the Arduino IDE, ensuring the correct port is selected. Then create a Python script which can be used to send commands to the Arduino via the serial port. To integrate the Arduino control into a web API, we use FastAPI.

Run the Server:
fastapi dev <name_of_file>.py

Test the API using Command line:


Turn LED On: curl -X POST http://127.0.0.1:8000/led/on


Turn LED Off: curl -X POST http://127.0.0.1:8000/led/off



Explanation for the Python Code:


● Serial Initialization: Opens the serial connection with the specified port (COM5) and baud rate
(9600).


● Delay (2 seconds): Allows the Arduino to complete its reset and initialization process.


● Write Commands: Sends 1 to turn on the LED and 0 to turn it off.



Note: This activity can be connected to lab-act-6, it is the other arduino setup that will control this arduino light set up.