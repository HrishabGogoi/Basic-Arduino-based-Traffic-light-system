Arduino Traffic Light System
Description:
This repository contains the code and documentation for an Arduino-based traffic light system. The project was created to teach a beginner the fundamentals of Arduino programming and electronics.
Features:
 * Simulates a basic traffic light system with red, yellow, and green lights.
 * Uses a delay function to control the timing of the light changes.
 * Provides a simple and easy-to-understand code structure.
Getting Started:
 * Hardware:
   * Arduino board (e.g., Uno, Nano)
   * 3 LEDs (red, yellow, green)
   * 3 resistors (220 ohms)
   * Breadboard
   * Jumper wires
 * Software:
   * Arduino IDE (https://www.arduino.cc/en/Main/Software)
 * Circuit Diagram:
 * ![WhatsApp Image 2024-10-05 at 19 27 44_e1b44f44](https://github.com/user-attachments/assets/214f616c-e39f-43f4-8fee-159ea17f5410)

 * Code:
   // Define the pins for the LEDs
const int redPin = 9;
const int yellowPin = 10;
const int greenPin = 11;

void setup() {
  // Initialize the LED pins as outputs
  pinMode(redPin, OUTPUT);
  pinMode(yellowPin, OUTPUT);
  pinMode(greenPin, OUTPUT);
}

void loop() {
  // Red light ON
  digitalWrite(redPin, HIGH);
  digitalWrite(yellowPin, LOW);
  digitalWrite(greenPin, LOW);
  delay(5000); // Wait for 5 seconds

  // Yellow light ON
  digitalWrite(redPin, LOW);
  digitalWrite(yellowPin, HIGH);
  digitalWrite(greenPin, LOW);
  delay(2000); // Wait for 2 seconds

  // Green light ON
  digitalWrite(redPin, LOW);
  digitalWrite(yellowPin, LOW);
  digitalWrite(greenPin, HIGH);
  delay(5000); // Wait for 5 seconds
}

Usage:
 * Upload the code to your Arduino board.
 * Connect the LEDs, resistors, and breadboard according to the circuit diagram.
 * Power on the Arduino board.
 * Observe the traffic light system in action.
Note:
You can customize the timing of the lights by adjusting the delay values in the code.
Contributing:
Feel free to contribute to this project by improving the code, adding new features, or fixing bugs.
License:
MIT License
