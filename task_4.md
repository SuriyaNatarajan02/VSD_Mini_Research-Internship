# 4-Bit Binary Counter

## Overview
A 4-bit binary counter is a simple digital device that counts from 0 to 15 in binary. This project demonstrates how to build a 4-bit binary counter using either digital logic components or a microcontroller.

## Components Required
- Microcontroller (e.g., Arduino) or Logic ICs (e.g., 7474 D flip-flops, 7408 AND gates)
- Clock Source (555 Timer IC or external clock signal)
- Resistors
- Capacitors
- LEDs
- Breadboard and Jumper Wires
- Power Supply (e.g., 5V regulated supply)

## Circuit Connection
1. Connect the clock signal to the clock input of the first flip-flop.
2. Chain the Q output of each flip-flop to the clock input of the next flip-flop.
3. Implement a reset mechanism to reset all flip-flops.
4. Connect LEDs to the Q outputs of each flip-flop to display the binary count.

## Pinout Diagram
(Include a pinout diagram image here)

## Table for Pin Connection
| Component       | Pin Number / Name | Connection                   |
|-----------------|-------------------|------------------------------|
| Flip-Flop IC 1  | Clock             | Clock Source                 |
|                 | Q                 | LED1, Flip-Flop IC 2 Clock   |
|                 | Reset             | Reset Button                 |
| Flip-Flop IC 2  | Clock             | Q output of Flip-Flop IC 1   |
|                 | Q                 | LED2, Flip-Flop IC 3 Clock   |
|                 | Reset             | Reset Button                 |
| Flip-Flop IC 3  | Clock             | Q output of Flip-Flop IC 2   |
|                 | Q                 | LED3, Flip-Flop IC 4 Clock   |
|                 | Reset             | Reset Button                 |
| Flip-Flop IC 4  | Clock             | Q output of Flip-Flop IC 3   |
|                 | Q                 | LED4                         |
|                 | Reset             | Reset Button                 |
| LEDs            | Anode             | Respective Flip-Flop Q Output|
|                 | Cathode           | Ground                       |
| 555 Timer IC    | VCC               | +5V Supply                   |
|                 | GND               | Ground                       |
|                 | Output            | Clock Input for Flip-Flops   |
| Resistors       | -                 | As per LED and IC requirements|

