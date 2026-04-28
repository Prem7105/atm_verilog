# FPGA-Based ATM System (Verilog)

## Overview

This project implements a simplified Automated Teller Machine (ATM) on an FPGA using Verilog HDL. The system supports basic banking operations including user authentication, cash deposit, and cash withdrawal. It integrates hardware components such as a matrix keypad for input and a 16×2 LCD for output display.

The design focuses on digital system implementation using a Finite State Machine (FSM) and demonstrates real-time interaction between user inputs and hardware-controlled outputs.

## Features

- PIN-based user authentication
- Deposit functionality with balance update
- Withdrawal functionality with balance verification
- Real-time display using 16×2 LCD
- Keypad-based user input
- FSM-based control logic

## System Design

The system is structured around a Finite State Machine with the following states:

- Idle
- PIN Entry
- Authentication
- Menu Selection
- Deposit
- Withdrawal
- Transaction Processing
- Display Output

Each state handles a specific part of the ATM workflow, ensuring a clear and modular design.

## Hardware Requirements

- FPGA board (e.g., Basys 3, Spartan-6, Artix-7)
- 4×4 matrix keypad
- 16×2 LCD display
- Power supply

## Software and Tools

- Verilog HDL
- Xilinx Vivado or ISE
- ModelSim (optional, for simulation)

## Working

The user interacts with the system through a keypad to enter a PIN. The system verifies the PIN and, upon successful authentication, allows the user to select a transaction type. For deposits, the entered amount is added to the stored balance. For withdrawals, the system checks for sufficient balance before processing the transaction. All instructions and outputs are displayed on the LCD.

## Simulation

Simulation verifies correct FSM transitions, PIN validation, and transaction handling. Testbenches are used to validate different operational scenarios including invalid PIN attempts and insufficient balance conditions.

## Future Improvements

- Card-based authentication
- Transaction history storage
- Enhanced security mechanisms
- Integration with external systems
