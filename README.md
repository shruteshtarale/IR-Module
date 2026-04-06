# IR-Module

What is an IR Beam Sensor?

An Infrared (IR) Beam Sensor is a device that uses invisible infrared light to detect the presence or movement of an object by checking whether the beam is interrupted.

It has 2 main parts:
1. IR Transmitter (Emitter)
Usually an IR LED
Emits infrared light continuously
2. IR Receiver
Photodiode / Phototransistor
Detects IR light

⚙️ Working Principle
Step-by-Step
Case 1: No Object
IR beam reaches receiver
Output = HIGH (or stable signal)
Case 2: Object Present
Beam is interrupted
Receiver doesn’t get IR light
Output = LOW

This change is detected by circuit

Types of IR Sensors
#Break Beam Sensor (Used in YOUR project 🔥)
Separate transmitter & receiver
Accurate
Used for entry/exit detection
#Reflective IR Sensor
Transmitter & receiver together
Detects reflection
Used in line-following robots
#Proximity Sensor
Detects nearby objects
Short range



| Condition   | Output |
| ----------- | ------ |
| Beam intact | HIGH   |
| Beam broken | LOW    |




#Components Inside IR Module
IR LED
Photodiode / Phototransistor
Comparator (sometimes)
Resistors
