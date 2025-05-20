# Elevator Project in CODESYS

## Overview
This project simulates an elevator system for a five-storey building, programmed using the Ladder Diagram (LD) language in CODESYS. It includes floor call buttons, up and down direction buttons, and limit switches at the top and bottom of each floor. The elevator's logic is controlled by timers and button presses to manage the elevator’s movement and door opening sequences.

---

## Prerequisites

Before running the project, you need to install the CODESYS software. You can download it from the official website:

- [CODESYS Download](https://store.codesys.com/en/codesys.html)

---

## System Description

- **Building Layout**: A five-storey building with floors numbered 1 to 5.
- **Limit Switches**: Each floor is equipped with both top and bottom limit switches that are pressed manually.
- **Timers**:
  - **7-second Timer**: Activates when the elevator door opens, giving a 7-second delay before the door closes.
  - **10-second Timer**: If no button inside the elevator is pressed, the door reopens after 10 seconds to allow the passenger to make a selection.
- **Elevator Operation**: 
  - The elevator's movement is determined by the current direction (up or down) and the requested direction (based on the up or call buttons pressed on the floors).

---

## Key Components

### 1. **Buttons**:
   - **Up Button**: Requests the elevator to go up from any floor.
   - **Call Button**: Requests the elevator to stop on a specific floor.
   - **Inside Buttons**: Located inside the elevator cabin to choose the destination floor.

### 2. **Limit Switches**:
   - **Top and Bottom Limit Switches**: Ensure that the elevator stops at the correct floors and doesn't travel beyond the designated limits.

### 3. **Timers**:
   - **7-second Timer**: This timer controls the duration the elevator doors stay open after arriving at a floor.
   - **10-second Timer**: If no buttons are pressed inside the elevator cabin, the doors will remain open for 10 seconds before automatically closing.

---

## How the System Works

1. **Call Buttons**: When a user presses a call button on any floor (up or down), the elevator responds according to its current direction and the requested floor.
2. **Direction Control**: The elevator moves either up or down depending on the current floor and the direction requested via the call buttons or inside buttons.
3. **Door Operation**:
   - The elevator doors automatically open when it reaches a floor.
   - After 7 seconds, if no further interaction occurs, the doors will close.
   - If no button is pressed inside the elevator, a 10-second timer will trigger, reopening the doors for another 10 seconds.

---

## How to Run the Project

1. **Install CODESYS**: Ensure that you have installed CODESYS on your system. Refer to the [CODESYS official website](https://www.codesys.com/) for installation instructions.
2. **Download the Project Files**: Import the project files into CODESYS.
3. **Compile and Run**: Compile the program and download it to the CODESYS runtime environment to simulate the elevator operation.

---

## Demo

For a better understanding of how the system works, you can watch the demonstration video linked below.

[Watch the Video Demo](https://www.youtube.com/watch?v=aE5h5UhwjUU)

---

## Good Luck!

We hope this project helps you understand the basics of controlling an elevator system using Ladder Diagram programming. If you have any questions or need assistance, feel free to reach out.
