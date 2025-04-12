# FIFO Memory Implementation

## Overview
This repository contains a VHDL implementation of a FIFO (First In, First Out) memory structure for FPGA technology. The project was developed as an assignment for the "Digital Systems Design" course at the Faculty of Automation and Computer Science, Technical University of Cluj-Napoca.

## Project Description
The implementation follows the FIFO logic where the first data entered into memory is the first to be retrieved. The memory structure provides efficient data handling with simultaneous read and write operations through dual-port RAM usage, which significantly improves speed compared to asynchronous memory implementations.

## Components
- **Control Unit (unit_command)**: Manages PUSH and POP operations
- **Status Component**: Indicates when the memory is EMPTY or FULL
- **Reversible Synchronous Counter**: Used for PUSH, POP operations and element counting
- **32x8 RAM Memory**: Storage for 8-bit data words
- **2:1 Multiplexer**: Selects between PUSH and POP address counters
- **Binary to Decimal Converter**: Converts binary inputs to decimal for display

## Features
- 32x8 memory structure (32 addresses, 8-bit words)
- Empty and Full status indicators
- Manual memory reset operation
- BCD 7-segment display for visualization of data and memory status

## Implementation
The project is implemented in VHDL with distinct components connected in a structural design. The control logic follows a state machine approach based on the system flowchart.

##  Authors
 Maria-Magdalena Creț
##  Acknowledgments
- **Technical University of Cluj-Napoca**
- **Faculty of Automation and Computer Science**

## License
This project is provided for educational purposes.
