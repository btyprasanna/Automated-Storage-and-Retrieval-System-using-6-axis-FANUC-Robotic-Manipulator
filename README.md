# Automated Storage and Retrieval System using 6-axis FANUC Robotic Manipulator

<p align="justify">
This repository contains documentation for an Automated Storage and Retrieval System (ASRS) implemented using a Fanuc LR Mate 200iD 4S 6-axis manipulator. The system is designed to pick objects and place them in designated storage racks made of Acrylic Sheet. The ASRS utilizes pneumatic cylinders (double acting) and telescopic slides controlled by five-way solenoid valves.
</p>

<img align="center"
src="https://github.com/btyprasanna/Automated-Storage-and-Retrieval-System-using-Fanuc-6-axis-Manipulator/assets/106366271/f554c088-b767-49fb-ba6e-48d3644a52d1">
</a>

<img align="center"
src="https://github.com/btyprasanna/Automated-Storage-and-Retrieval-System-using-6-axis-FANUC-Robotic-Manipulator/assets/106366271/2f8a2010-ca71-4af4-a76c-24ac5f01cf7e">
</a>

> All project images and videos were taken by me unless stated otherwise.

## Index

- [Features](#features)
- [Hardware Components 🔌](#hardware-components)
- [Software Reqs](#software-reqs)
- [System Configuration](#system-configuration)
  - [System Design](#system-design)
  - [System Integration](#system-integration)
  - [PLC Programming](#plc-programming)
  - [Robot Programming](#robot-programming)
  - [System Calibration and Testing](#system-calibration-and-testing)
- [Usage](#usage)

## Features

- Utilizes the Fanuc LR Mate 200iD 4S robotic manipulator for precise object manipulation.
- Integrates a pneumatic system with double-acting cylinders and telescopic slides for rack movement.
- Control system based on Allen Bradley CompactLogix L16 384KB Ctlr (1769-L16ER-BB1B) PLC.
- Communication between the PLC and the Fanuc robot is established through Ethernet I/O, enabling seamless coordination.
- Programmed using Studio 5000 software for PLC programming.

## Hardware Components

- [FANUC LR Mate 200iD/4S](https://www.fanucamerica.com/products/robots/series/lr-mate/lr-mate-200id-4s)
- [Allen Bradley CompactLogix L16 384KB Ctlr (1769-L16ER-BB1B)](https://www.rockwellautomation.com/en-us/products/details.1769-L16ER-BB1B.html)
- [24V Relay Module](https://www.google.com/search?q=24v+relay+module&tbm=shop)
- [24V 10A Power Supply](https://www.google.com/search?q=24V+10A+Power+Supply&tbm=shop)
- [Pneumatic Cylinder (Double acting)](https://www.google.com/search?q=Pneumatic+Cylinder+(Double+acting)&tbm=shop)
- [Five Ways (5/2 or 5/3) Solenoid Valves](https://www.google.com/search?q=Five+Ways+(5/2+or+5/3)+Solenoid+Valve&tbm=shop)
- [One-Way Flow Control Valve](https://www.google.com/search?q=One-Way+Flow+Control+Valve&tbm=shop)
- [Telescopic Slide](https://www.google.com/search?q=Telescopic+Slide&tbm=shop)
- Aluminium Profile
- Aluminium Profile Angle Bracket
- Acrylic Sheet
- 3D Printed Components

We need crimping tools and other necessary tools for PLC panel wiring, as well as pneumatic cables and accessories for the pneumatic system.

## Software Reqs

- [Studio 5000](https://www.rockwellautomation.com/en-us/products/software/factorytalk/designsuite/studio-5000.html)

The robot's position program can be programmed using the teach pendant of the robot.

## System Configuration

### System Design:

<p align="justify">
Identify the requirements and specifications of the Automated Storage and Retrieval System (ASRS). Select the Fanuc LR Mate 200iD 4S robot as the robotic manipulator. Choose Acrylic Sheet for the construction of the storage racks. Determine the suitable Pneumatic Cylinder (Double acting) and Telescopic Slide for rack movement. Select the appropriate Five Ways (5/2 or 5/3) Solenoid Valves for controlling the pneumatic components. Choose the Allen Bradley CompactLogix L16 384KB Ctlr (1769-L16ER-BB1B) PLC for controlling the solenoid valves.
</p>

### System Integration:

<p align="justify">
Design the mechanical structure of the ASRS, incorporating the storage racks, pneumatic cylinders, and telescopic slides.
Integrate the Fanuc LR Mate 200iD 4S robot with the ASRS system.
Connect the pneumatic cylinders and telescopic slides to the Solenoid Valves.
Establish communication between the Allen Bradley PLC and the Fanuc robot through Ethernet I/O feature.
Set up the virtual I/O tags in the PLC to facilitate data exchange and coordination with the robot.
</p>

### PLC Programming:

<p align="justify">
Utilize Studio 5000 software for programming the Allen Bradley CompactLogix L16 384KB Ctlr PLC.
Develop a ladder program that controls the Solenoid Valves for actuating the pneumatic components.
Establish communication between the PLC and the virtual I/O tags of the Fanuc robot for synchronization.
</p>

### Robot Programming:

<p align="justify">
Use the teach pendent provided by Fanuc for the Fanuc LR Mate 200iD 4S robot for position teaching.
Develop subprograms that contain the position path for picking up and placing objects in the designated racks.
Integrate the subprograms with a main programn that contains the virtual I/O tags of the robot for receiving commands from the PLC.
</p>

### System Calibration and Testing:

<p align="justify">
Calibrate the robot and the ASRS system to ensure precise movements and accurate object placement.
Perform testing to verify the functionality of the system, including object picking, rack movement, and placement.
Fine-tune the system parameters as needed to achieve optimal performance and reliability.
</p>

## Usage

- Power on the system and ensure all connections are secure.
- Press the designated push button corresponding to the desired rack in the ASRS.
- The PLC will communicate with the Fanuc robot through Ethernet I/O, triggering the specific subprogram for the designated rack.
- The robot will execute the predefined positions and paths to pick and place the object accurately.
- Once the object is placed, the system is ready for the next operation.

***Note:*** This repository is intended for educational and research purposes. Use caution and follow safety guidelines while working with the automated system.
