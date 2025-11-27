# Smart Dustbin Project

## Overview

This project implements an automated "Smart Dustbin" system using an Arduino microcontroller. The primary objective is to create a touch-free waste disposal mechanism to improve hygiene and sanitation. The system utilizes an ultrasonic sensor to detect proximity and a servo motor to automatically open and close the dustbin lid.

## Features

- **Automatic Detection**: Uses an HC-SR04 ultrasonic sensor to detect objects (e.g., a hand) within a 30cm range.
- **Touch-less Operation**: Reduces the risk of germ transmission by eliminating physical contact with the lid.
- **Automated Lid Control**: A servo motor opens the lid upon detection and closes it automatically after a 3-second delay.

## Hardware Requirements

- Arduino Uno R3
- Ultrasonic Distance Sensor (HC-SR04)
- Micro Servo Motor (SG90 or equivalent)
- Jumper Wires
- Breadboard
- 9V Battery or USB Power Supply

## Pin Configuration

The circuit connections are defined as follows:

| Component | Pin Type | Arduino Pin |
|-----------|----------|-------------|
| Servo | Signal | Pin 9 |
| Sensor | Trig | Pin 10 |
| Sensor | Echo | Pin 11 |
| Sensor | VCC | 5V |
| Sensor | GND | GND |

## Simulation

The project has been simulated and tested using TinkerCAD. You can view the circuit design and run the simulation at the link below:

[View TinkerCAD Simulation]

## Setup and Installation

1. Connect the hardware components according to the pin configuration table above.
2. Open the project code in the Arduino IDE.
3. Connect the Arduino Uno to your computer via USB.
4. Select the correct Board and Port in the IDE.
5. Upload the code to the board.

## How it Works

1. The ultrasonic sensor continuously emits sound waves to measure the distance of objects in front of the bin.
2. The Arduino processes the signal duration to calculate the distance in centimeters.
3. If an object is detected within 30 cm, the servo motor rotates to 180 degrees, opening the lid.
4. The lid remains open for 3 seconds to allow for waste disposal.
5. After the delay, the servo rotates back to 0 degrees, closing the lid.

## Contributors

- Aniket Pandey (23803008)
- Mudit Maheshwari (23803017)

Submitted to Jaypee Institute of Information and Technology.
