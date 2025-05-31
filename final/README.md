
# Final Project

This final project is worth 50% of your total grade and will give you the opportunity to apply your knowledge in Verilog, FPGA, and ASIC implementation. This assignment is designed to be both challenging and flexible, allowing you to focus on areas that align with your interests and expertise.

## Project Overview

You will work in teams of 2-4 to design, implement, and verify a substantial Verilog-based system. The project must involve three key components:

* Verilog Writing: Crafting RTL designs to implement your system.
* FPGA Implementation: Testing your design on real hardware.
* ASIC Implementation: Preparing your design for tape-out using tools like OpenLane and the SKY130 PDK.

However, your team must choose one area to focus deeply on, based on your interests and skill sets.

### FPGA-Implementation-Heavy Track

Design less complex RTL, but utilize high-speed interfaces such as Ethernet or PCIe.

* For Ethernet, I recommend the Nexys A7 FPGA board.
    * Open source Ethernet implementation: <https://github.com/alexforencich/verilog-ethernet/tree/master/example/NexysVideo/fpga>.
    * Can be controlled with with Python code that sends packets over the Ethernet port
* For PCIe, I recommend the [Acorn CLE-215+ with LiteX Baseboard](https://enjoy-digital-shop.myshopify.com/products/litex-acorn-baseboard-mini-sqrl-acorn-cle215).
    * Open source PCIe implementation: <https://github.com/alexforencich/verilog-pcie>.
    * Sample project: <https://github.com/RHSResearchLLC/NiteFury-and-LiteFury/tree/master/Sample-Projects/Project-0>

### ASIC-Focused Track

Design less complex RTL, but go very deep into an ASIC implementation.

Specifications for this track will depend on your team's proposal. Examples include passing DRC for ASAP7, targeting Caravel-mini, significant optimizations for power/performance, or advanced utilizations of VLSI tools.

### Simple RTL Ideas for FPGA or ASIC-Heavy Track

* Complex Arithmetic Algorithm: Implement division, CORDIC, or square root. Refer to *Computer Arithmetic: Algorithms and Hardware Designs* by B. Parhami for ideas and guidance (ISBN-13 978-0-19-532848-6).
* RISC-V Core Integration: Get a small RISC-V core IP working by handling memory read requests over UART.
    * Suggested cores: [SERV](https://github.com/olofk/serv), [Ibex](https://github.com/lowRISC/ibex), [PicoRV32](https://github.com/YosysHQ/picorv32).
* VGA Game: Create a basic VGA game such as Tic-Tac-Toe, Flappy Bird, or Asteroids.

### Complex RTL Ideas for SystemVerilog-Implementation-Heavy Track

Focus on building a complex RTL design, simply using the UART infrastructure you built in HW1. All designs must be paired with extremely strong testbenches.

* Design an embedded-class RISC-V core that communicates over UART.
* Implement several complex arithmetic operations, such as a full floating-point unit, or a suite of dividers.
* Build an eigenvalue calculator or an SVD processor.
* Create a GPU controllable via UART.
* Stream data from an Arducam to VGA, applying video filters.

## Timeline and Milestones

**1/12/2025: Introduction Post**

On Piazza, write a paragraph introducing yourself and explaining what project(s) you are interested in working on.

**1/17/2025: Team Formation and [Proposal Submission](./proposal.md)**

Assemble your teams and submit a one-page proposal outlining your project idea and a timeline of goals.

**1/27/2025 - 1/31/2025: First Checkpoint**

Meet with Ethan to demonstrate significant progress and verify that your project is on track.

**2/17/2025 - 2/21/2025: Second Checkpoint**

Meet with Ethan again to show further progress and confirm readiness for the final phase.

**Week of 3/10/2025: Final Presentation**

Deliver a 10-minute presentation detailing your project, including implementation steps, challenges, results, and a demo if applicable. A final project report is due before your presentation.
