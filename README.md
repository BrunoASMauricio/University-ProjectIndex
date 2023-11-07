# University Projects Index

This repository is an index for the projects I developed during my masters.
It describes them and details what parts I developed (in the cases where there was a team effort)

---

## Table of Contents

- [Network Protocol Definition](#network-protocol-definition-telecommunication-systems-course)
- [Network Protocol Implementation](#network-protocol-implementation-telecommunication-systems-course)
- [Network Simulator](#network-simulator-telecommunication-systems-course)
- [Java-- compiler](#java---compiler-compilers-course)
- [Distributed Systems](#distributed-system-node-distributed-systems-course)
- [Custom Chess game in Java](#custom-chess-game-in-java-programming-laboratory-course)
- [Arduino window manager](#arduino-window-manager-computers-course)
- [Atduino JTAG bitbang](#arduino-jtag-bitbang-electronic-systems-course)

---

## Network Protocol Definition: Telecommunication Systems course

**Repository**: [GitHub Link](https://github.com/BrunoASMauricio/University-NetworkProtocolDefinition)

**Description**:

The whole project was a full end-to-end solution for wind sensing nodes that could connect ad hoc.

My responsibility was to define a custom protocol standard for this purpose, and implement it.

Main protocol functionality:

1. Time Division Multiple Access (Medium Access)
2. Clock synchronization
3. Distance-Vector based routing
4. Non-byzantine fault resistance
5. Application packet multiplexing

The latest protocol definition (RFC style) can be found [here](https://github.com/BrunoASMauricio/University-NetworkProtocolDefinition/blob/master/versions/V3.txt)

**My Role**:

- Protocol designer
  - Fully design the protocol
  - Coordinate with antennas team to define minimum bandwidth necessary and acceptable error amounts
  - Coordinate with sensor team to define amount of data per second that could be transmitted

**Note:** There are many other repos that belong to the project as a whole, but as they were not my main focus I do not include them here.

---

## Network Protocol Implementation: Telecommunication Systems course

**Repository**: [GitHub Link](https://github.com/BrunoASMauricio/University-NetworkProtocol)

Implementation of the protocol specified above

Extra implementation specific functionality:

1. Protocol implementation unit tests
2. Reproducibility
   1. The implementation generate or consume random values
3. Logging
   1. Also dumps binary packets for improved debugging

**My Role**:

- Lead developer
  - Responsible for delineating tasks and coordinating with other teams
  - Creator of the protocol definition linked above
  - Main developer (developed all functionalities above)
- Other team members performed packet \[de]serialization and small maintenance tasks

**Note:** There are other repos that belong to the project as a whole, but as they were not my main focus I do not include them here.

---

## Network Simulator: Telecommunication Systems course

**Repository**: [GitHub Link](https://github.com/BrunoASMauricio/University-NetworkSimulator)

**Description**:

A network simulator written in C, used to test the protocol above.
Functionality description:

1. UDP port based connections
2. Errors supported:
   1. Random bit flip
   2. Packet loss
   3. Extreme packet delay
3. Use distance maps to calculate appropriate delay in delivering packets between devices
4. Generate/Consume probability files for packet transmission to accurately recreate and debug failure scenarios
5. Ability to Mute/Deafen/Shutdown a specific node for a specific time

**My Role**:

- Main developer
- Other team members performed small maintenance tasks

**Note:** There are many other repos that belong to the project as a whole, but as they were not my main focus I do not include them here.

---

## Java-- compiler: Compilers course

**Repository**: [GitHub Link](https://github.com/BrunoASMauricio/University-Java--Compiler)

**Description**:

In this project, I developed a compiler for a subset of the Java language (nicknamed Java--), using Java.
Besides supporting the Java-- language, it features basic optimizations such as:

1. Liveliness analysis for register allocation
2. Constant propagation
3. Constant folding
4. Smaller optimizations
   1. Utilize less expensive comparisons by reorganizing the inputs
   2. Constant push instructions optimized based on the size of the constant
   3. Precise stack calculation
   4. Array of size 1 as variables
   5. ...

**My Role**:

- Single developer

---

## Distributed System node: Distributed Systems course

**Repository**: [GitHub Link](https://github.com/BrunoASMauricio/University-DistributedSystem)

**Description**:

Implement paxos and bully leader election algorithms to create a fault tolerant node for a distributed system, which can automatically appoint a leader and begin transmitting messages between nodes

**My Role**:

- Network simulation
- Bully protocol leader election implementation

---

## Custom Chess game in Java: Programming Laboratory course

**Repository**: [GitHub Link](https://github.com/BrunoASMauricio/University-CustomChess)

**Description**:

In this game of chess, each piece is described by its' movement pattern and image.
Using a visual interface (or the txt file representations), it is possible to generate new pieces with custom movement patterns, and assemble them into custom boards.
These boards can then be sent to another peer in the same LAN network, for a custom PvP game.

**My Role**:

- Single developer

---

## Arduino Window Manager: Computers course

**Repository**: [GitHub Link](https://github.com/BrunoASMauricio/University-ArduinoWindowManager)

**Description**:

This window manager was one of the first projects of my career.
It supports 7 concurrent windows, that can be dragged and overlap, and support basic character sets, or direct bitmap manipulation.
Due to the refresh rate constraints of the LCD used, I had to implement an optimized refresh, where only the pixels that were altered would update (whenever it was possible to infer this)

The second part of the project was created by @rycostinha, and involved using these windows to run the pong and snake games.

**My Role**:

- Create underlying resource management
- Create windowing system

---

## Arduino JTAG Bitbang: Electronic Systems course

**Repository**: [GitHub Link](https://github.com/BrunoASMauricio/University-JTAGBitbanger)

**Description**:

Simple Arduino implementation of JTAG via bitbanging

**My Role**:

- Single developer
