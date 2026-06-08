Arduino Dual LED Toggle System

Project Overview

This project demonstrates a multi-state LED control system using Arduino Uno and a single push button. The system controls two LEDs in a predefined sequence, showcasing digital input handling, state management, and event-driven programming.


Objectives

* Control multiple LEDs using a single push button.
* Understand Arduino digital inputs and outputs.
* Learn state-based programming.
* Demonstrate sequential LED operation.


Components Required

| Component     | Quantity    |
| ------------- | ----------- |
| Arduino Uno   | 1           |
| Push Button   | 1           |
| LED           | 2           |
| 220Ω Resistor | 2           |
| Breadboard    | 1           |
| Jumper Wires  | As Required |


Working Principle

The push button changes the system state whenever it is pressed.

State Sequence

| Button Press | LED 1 | LED 2 |
| ------------ | ----- | ----- |
| Initial      | OFF   | OFF   |
| Press 1      | ON    | OFF   |
| Press 2      | ON    | ON    |
| Press 3      | ON    | OFF   |
| Press 4      | OFF   | OFF   |

The sequence repeats continuously.


Circuit Connections

Push Button

* Arduino Pin 2 → Push Button → GND
* Internal Pull-Up Resistor enabled using `INPUT_PULLUP`

LED 1

* Arduino Pin 12 → 220Ω Resistor → LED 1 Anode
* LED 1 Cathode → GND

LED 2

* Arduino Pin 13 → 220Ω Resistor → LED 2 Anode
* LED 2 Cathode → GND


Project Images

Initial State
<img width="1200" height="1600" alt="Off State" src="https://github.com/user-attachments/assets/ed0b4f41-16be-4dd1-8a2b-a6b688b82a50" />


LED 1 ON
<img width="1200" height="1600" alt="LED 1 On" src="https://github.com/user-attachments/assets/3211f172-0cac-4a0e-80f1-f31dc1ee2e16" />


Both LEDs ON
<img width="1200" height="1600" alt="Both LED&#39;sOn" src="https://github.com/user-attachments/assets/16dae1b7-8690-412e-a59a-9d1cbd0db992" />


Concepts Used

* Arduino Programming
* Digital Input/Output
* Push Button Debouncing
* State Machine Logic
* Embedded Systems Fundamentals


Future Improvements

* Add buzzer indication.
* Add LCD display for state count.
* Add RGB LED control.
* Convert into an IoT-enabled system.
