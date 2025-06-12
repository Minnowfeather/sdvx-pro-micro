# DJDao Arduino Drop-in Replacement

This project aims to be a drop-in replacement for DJDao SVSE5 and SVRE9 PCBs. Only supports potentiometers and DJDao-style wiring.

LEDs are wired to 5V and a pin on the Pro Micro. Writing LOW will turn ON the LED, and writing HIGH will turn it OFF.

# Pin assignments

| Button | Data | LED |
| ------ | ---- | --- |
| BT-A   | 2    | 3   |
| BT-B   | 4    | 5   |
| BT-C   | 6    | 7   |
| BT-D   | 10   | 16  |
| FX-L   | 14   | 15  |
| FX-R   | A0   | A1  |
| Start  | 1    | 0   |
| VOL-L  | A2   | N/A |
| VOL-R  | A3   | N/A |

# Code

Use a modifed version of [KnucklesLee's code](https://github.com/knuckleslee/RhythmCodes/).

# Known Issues

V1: Pots are jittery, affected by the LEDs, and each other(?)

V1: Button pins have swapped GND and 5V
