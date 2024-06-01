
# Two Blinking LEDs

This project demonstrates how to control two LEDs using a microcontroller, such as an Arduino. The LEDs blink alternately, creating a simple but visually appealing effect. This example serves as a foundational exercise for learning basic electronics and programming concepts related to microcontrollers and digital output.

## Table of Contents

- [Introduction](#introduction)
- [Components](#components)
- [Circuit Diagram](#circuit-diagram)
- [Setup and Assembly](#setup-and-assembly)
- [Code Explanation](#code-explanation)
- [Uploading the Code](#uploading-the-code)
- [Troubleshooting](#troubleshooting)
- [Conclusion](#conclusion)

## Introduction

The Two Blinking LEDs project is a beginner-friendly introduction to working with microcontrollers. By controlling two LEDs, you will learn how to:

- Set up a basic electronic circuit.
- Write simple code to control digital outputs.
- Understand timing and delays in microcontroller programming.

## Components

To complete this project, you will need the following components:

- 1 x Arduino (or any compatible microcontroller)
- 2 x LEDs (any color)
- 2 x 220 ohm resistors
- Breadboard
- Jumper wires
- USB cable to connect the Arduino to a computer

## Circuit Diagram

Here is a simple circuit diagram to help you set up the project:

```
[Arduino] --- [LED1] --- [Resistor1] --- [GND]
     |
     |--- [LED2] --- [Resistor2] --- [GND]
```

- Connect the positive leg (anode) of LED1 to pin 8 on the Arduino.
- Connect the negative leg (cathode) of LED1 to one end of Resistor1.
- Connect the other end of Resistor1 to the GND pin on the Arduino.
- Connect the positive leg (anode) of LED2 to pin 9 on the Arduino.
- Connect the negative leg (cathode) of LED2 to one end of Resistor2.
- Connect the other end of Resistor2 to the GND pin on the Arduino.

## Setup and Assembly

1. Place the LEDs and resistors on the breadboard.
2. Use jumper wires to connect the components according to the circuit diagram.
3. Connect the Arduino to your computer using a USB cable.

## Code Explanation

Here is the code you will upload to the Arduino:

```cpp
// Define the LED pins
const int ledPin1 = 8;
const int ledPin2 = 9;

void setup() {
  // Initialize the LED pins as outputs
  pinMode(ledPin1, OUTPUT);
  pinMode(ledPin2, OUTPUT);
}

void loop() {
  // Turn on LED1 and turn off LED2
  digitalWrite(ledPin1, HIGH);
  digitalWrite(ledPin2, LOW);
  // Wait for 500 milliseconds
  delay(500);

  // Turn off LED1 and turn on LED2
  digitalWrite(ledPin1, LOW);
  digitalWrite(ledPin2, HIGH);
  // Wait for 500 milliseconds
  delay(500);
}
```

### How the Code Works

1. **Define LED Pins**: The pins connected to the LEDs are defined at the beginning.
2. **Setup Function**: The `setup()` function initializes the LED pins as outputs.
3. **Loop Function**: The `loop()` function repeatedly turns the LEDs on and off alternately with a 500-millisecond delay.

## Uploading the Code

1. Open the Arduino IDE on your computer.
2. Copy and paste the provided code into a new sketch.
3. Select the correct board and port from the Tools menu.
4. Click the Upload button to upload the code to your Arduino.

## Troubleshooting

- **LEDs not blinking**: Check all connections, ensuring the LEDs are connected with the correct polarity (anode to pin, cathode to resistor).
- **Code upload errors**: Ensure the correct board and port are selected in the Arduino IDE. Try resetting the Arduino and uploading the code again.
- **LEDs stay on or off**: Verify that the resistors are properly connected and have the correct value (220 ohms).

## Conclusion

The Two Blinking LEDs project is a great starting point for learning about microcontrollers, circuits, and programming. Once you've mastered this project, you can expand on it by adding more LEDs, using different patterns, or incorporating sensors to create more complex behaviors.

By understanding the basics presented in this project, you'll be well-equipped to take on more advanced electronics projects in the future. Enjoy experimenting and learning!
