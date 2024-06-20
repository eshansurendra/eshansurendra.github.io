---
layout: page
title: UART-FPGA
description: Developed as part of the EN2111 Electronic Circuit Design module at the University of Moratuwa, focusing on the implementation of a UART communication link between two FPGA boards. This project provides a practical understanding of UART communication protocols and their implementation within an FPGA environment.
img: assets/img/uart/thumb.png
importance: 3
category: hardware
tags : ['uart', 'fpga', '7-segment']
github: https://github.com/eshansurendra/UART-FPGA
---

> For detailed documentation and source code, visit my [GitHub Repository](https://github.com/eshansurendra/UART-FPGA).

### Project Overview

The objective of this project was to establish a functional UART communication link between two FPGA boards using the Quartus Prime development platform. This involved:

* **Design and Implementation:** Designing and implementing the UART transmitter and receiver modules in SystemVerilog.
* **Verification and Testing:** Utilizing Quartus Prime and ModelSim to simulate and verify the functionality of the designed UART modules.
* **FPGA Integration:** Integrating the UART modules with hardware components, specifically a 7-segment display connected to the receiver FPGA board.

**Functional Breakdown:**

* **Transmitter:** The transmitter module receives data (binary numbers in this case) and converts it into serial data streams, adhering to the UART protocol. These serial data streams are transmitted over the communication channel. 
* **Receiver:** The receiver module receives the serial data stream, converts it back to parallel data, and sends it to a designated output, in this case, a 7-segment display driver to display the received binary number.

### Implementation and Verification

The project utilizes `Quartus Prime 20.1.1` and `ModelSim` for FPGA development and ModelSim for simulation. 

**Timing Diagram:**

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid path="assets/img/uart/timing_diagram.png" title="Timing Diagram" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

**Key Technical Concepts:**

* **UART Protocol:**  Understanding the UART communication protocol, including the signal timing, start and stop bits, parity bit, and data format.
* **SystemVerilog:** Proficiency in SystemVerilog for designing and implementing digital circuits within the FPGA environment.
* **FPGA Architecture:** Understanding the basic architecture of FPGAs and how logic modules are interconnected to create custom circuits.
* **Simulation and Verification:** Utilizing tools like Quartus Prime and ModelSim to test and verify the functionality of the designed circuits.

This project serves as a practical foundation for learning about serial communication protocols, their implementation within FPGAs, and the tools and techniques used in FPGA design and development.
