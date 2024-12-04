# LED-Blinking
# LED Blinking System using Arduino (Embedded C++)

## Overview
This project demonstrates a simple LED blinking system using an Arduino kit programmed in Embedded C++. The LED will blink at a regular interval based on the code provided.

## Components Required
- Arduino Board (e.g., Arduino Uno)
- LED
- 220Ω Resistor
- Breadboard and Jumper wires

## Circuit Diagram
[Include your circuit diagram here]

## Code Explanation
The program blinks an LED connected to pin 13 of the Arduino. The LED will turn ON for 1 second and OFF for 1 second in an infinite loop. 

### Code Breakdown:
1. **Pin Configuration**: The LED is connected to digital pin 13.
2. **Setup**: In the `setup()` function, pin 13 is set as an output pin.
3. **Loop**: In the `loop()` function, the LED is turned ON for 1 second, then OFF for 1 second in a continuous loop.

```cpp
// LED Blinking System

// Define LED pin
#define LED_PIN 13

void setup() {
  // Initialize the digital pin as an output.
  pinMode(LED_PIN, OUTPUT);
}

void loop() {
  // Turn the LED ON
  digitalWrite(LED_PIN, HIGH);
  delay(1000);  // Wait for 1 second

  // Turn the LED OFF
  digitalWrite(LED_PIN, LOW);
  delay(1000);  // Wait for 1 second
}
