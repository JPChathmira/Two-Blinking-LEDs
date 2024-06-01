# Two-Blinking-LEDs
This project demonstrates how to control two LEDs using a microcontroller, such as an Arduino. The LEDs blink alternately, creating a simple but visually appealing effect. This example serves as a foundational exercise for learning basic electronics and programming concepts related to microcontrollers and digital output.

Table of Contents
Introduction
Components
Circuit Diagram
Setup and Assembly
Code Explanation
Uploading the Code
Troubleshooting
Conclusion
Introduction
The Two Blinking LEDs project is a beginner-friendly introduction to working with microcontrollers. By controlling two LEDs, you will learn how to:

Set up a basic electronic circuit.
Write simple code to control digital outputs.
Understand timing and delays in microcontroller programming.
Components
To complete this project, you will need the following components:

1 x Arduino (or any compatible microcontroller)
2 x LEDs (any color)
2 x 220 ohm resistors
Breadboard
Jumper wires
USB cable to connect the Arduino to a computer
Circuit Diagram
Here is a simple circuit diagram to help you set up the project:

css
Copy code
[Arduino] --- [LED1] --- [Resistor1] --- [GND]
     |
     |--- [LED2] --- [Resistor2] --- [GND]
Connect the positive leg (anode) of LED1 to pin 8 on the Arduino.
Connect the negative leg (cathode) of LED1 to one end of Resistor1.
Connect the other end of Resistor1 to the GND pin on the Arduino.
Connect the positive leg (anode) of LED2 to pin 9 on the Arduino.
Connect the negative leg (cathode) of LED2 to one end of Resistor2.
Connect the other end of Resistor2 to the GND pin on the Arduino.
Setup and Assembly
Place the LEDs and resistors on the breadboard.
Use jumper wires to connect the components according to the circuit diagram.
Connect the Arduino to your computer using a USB cable.
How the Code Works
Define LED Pins: The pins connected to the LEDs are defined at the beginning.
Setup Function: The setup() function initializes the LED pins as outputs.
Loop Function: The loop() function repeatedly turns the LEDs on and off alternately with a 500-millisecond delay.
Uploading the Code
Open the Arduino IDE on your computer.
Copy and paste the provided code into a new sketch.
Select the correct board and port from the Tools menu.
Click the Upload button to upload the code to your Arduino.
Troubleshooting
LEDs not blinking: Check all connections, ensuring the LEDs are connected with the correct polarity (anode to pin, cathode to resistor).
Code upload errors: Ensure the correct board and port are selected in the Arduino IDE. Try resetting the Arduino and uploading the code again.
LEDs stay on or off: Verify that the resistors are properly connected and have the correct value (220 ohms).
Conclusion
The Two Blinking LEDs project is a great starting point for learning about microcontrollers, circuits, and programming. Once you've mastered this project, you can expand on it by adding more LEDs, using different patterns, or incorporating sensors to create more complex behaviors.

By understanding the basics presented in this project, you'll be well-equipped to take on more advanced electronics projects in the future. Enjoy experimenting and learning!
