# Student-Portfolio-for-COSC111


## Laboratory Activity 6

Objectives:

1. To develop a system that detects button presses using an Arduino and communicates the button state to a Python script, which then triggers an API based on the state. The system establishes a connection to another device via Wi-Fi or a hotspot. 


Prerequisites


● Arduino board.


● USB cable to connect the Arduino to your computer.


● Arduino IDE installed on your system.


● Python (3.x) with pySerial, requests and FastAPI installed.


pip install pyserial requests fastapi[standard]




Description:

This project focused on implementing code for the button on the Arduino, while the connected device, using Wi-Fi or a hotspot, controls an LED on a breadboard with its own Arduino code.

To run the program, first follow the setup shown in A6-Diagram.png. Then, upload the .ino code to the Arduino IDE, ensuring the correct port is selected. Next, modify the given Python script according to your IP address, where in it communicates with the Arduino via the serial port. To integrate Arduino control into a web API, FastAPI is used.

To trigger an API call whenever the button is pressed, modify the Python script to send an HTTP request using a library like requests.


Run the Server:


fastapi dev <name_of_file>.py


Test the API using Command line:

Turn LED On: curl -X POST http://127.0.0.1:8000/led/on


Turn LED Off: curl -X POST http://127.0.0.1:8000/led/off



Note: This activity is connected to lab-act-5, it is the other arduino setup that can be controlled by this arduino button setup.

