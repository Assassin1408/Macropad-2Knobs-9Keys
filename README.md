# Custom Programmable Macropad

A 9-key, 2-knob programmable input device built around an Arduino Pro Micro (ATmega32U4), from custom PCB design through to firmware.

Full step-by-step build guide: [Instructables writeup](https://www.instructables.com/MACROPAD-With-2-Knobs)

<!-- TODO: add a photo or short demo GIF of the finished build here -->

## Features
- 9 mechanical keys and 2 rotary knobs
- 3 NeoPixel LED strips
- Custom PCB designed in Eagle
- Circuit simulated in Tinkercad before parts were ordered

## How it works
**Key matrix.** Each key has its own diode, wired as a scanned matrix. This prevents ghosting and lets 9 keys share a small set of microcontroller I/O pins. The firmware scans the matrix, reads the knobs, and drives the LED strips.

**Hardware.**
- Microcontroller: Arduino Pro Micro (ATmega32U4)
- PCB: designed in Eagle
- Prototyping: Tinkercad
- Enclosure: <!-- TODO: Fusion 360 case? say so if yes -->

## Repository layout
<!-- TODO: fill in to match your repo -->
- `firmware/`  Arduino C++ sketch
- `pcb/`  Eagle schematic and board files
- `docs/`  photos and wiring diagrams

## Build it yourself
1. Order the PCB using the files in `pcb/` (or follow the Instructables guide).
2. Solder the switches, a diode for each one, the knobs and the LED strips.
3. Open the sketch in the Arduino IDE, select the Pro Micro board, and upload.

<!-- TODO: add the exact bill of materials and any libraries needed -->

## Author
Samarth Saxena. Master of Artificial Intelligence student at Monash University, B.Tech in Electrical Engineering from MNIT Jaipur.
[LinkedIn](https://www.linkedin.com/in/samarth-saxena-14a6772a3/)
