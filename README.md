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

#Components Inside IR Module
IR LED
Photodiode / Phototransistor
Comparator (sometimes)
Resistors

 Project Summary

The project titled **“IR Beam-Based Room Occupancy Detection System (RoomSense IR)”** presents a low-cost, efficient, and non-intrusive solution for real-time room occupancy detection. The system is designed to automatically determine whether a room is occupied or vacant without requiring any manual intervention.

The proposed system utilizes two IR break beam sensor pairs positioned at the entrance of a room to detect the direction of movement. By analyzing the sequence in which the beams are interrupted, the system distinguishes between entry and exit events. This information is processed using digital logic circuits, specifically AND gates (7408) for sequence detection and NAND gates (7400) configured as an SR latch for maintaining the occupancy state.

When a person enters the room, the system sets the latch, indicating an occupied state, and activates an LED indicator. Conversely, when a person exits, the latch is reset, marking the room as vacant and turning off the indicator. The system operates entirely on hardware logic, eliminating the need for microcontrollers or software programming, thereby ensuring simplicity, reliability, and low power consumption.

This solution is particularly suitable for applications such as classrooms, laboratories, restrooms, and office spaces where automatic occupancy indication is required. While the system demonstrates high accuracy under proper alignment, it has certain limitations, including sensitivity to ambient light and inability to handle multiple simultaneous entries. Future enhancements may include integration with microcontrollers, IoT-based monitoring, and occupancy counting features.

Overall, the project successfully demonstrates the practical implementation of basic electronics and digital logic principles to solve a real-world problem in an efficient and scalable manner.

 Hardware Components:

1. IR Break Beam Sensor Modules (2 pairs)
   Used to detect entry and exit by sensing interruption of infrared beams across the doorway.

2. 7408 IC (Quad 2-input AND Gate)
   Used for sequence detection. It identifies whether Sensor A is triggered before Sensor B (entry) or vice versa (exit).

3. 7400 IC (Quad 2-input NAND Gate)
   Configured as an SR latch to store the occupancy state (Occupied/Vacant).

4. 7404 IC (Hex Inverter)
   Used for signal inversion where required to maintain correct logic levels.

5. LED Indicator
   Displays room status:

   * ON → Occupied
   * OFF → Vacant

6. Resistors

   * 220Ω → Current limiting for LED
   * 10kΩ → Pull-down resistors for stable sensor outputs

7. Power Supply Module (5V regulated)
   Provides stable voltage to sensors and ICs (via battery or USB).

8. Breadboard & Jumper Wires
   Used for prototyping and circuit connections.
