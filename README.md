# Implementation of 1X3 Router using Verilog HDL
It is designed accepts data packets on a single 8-bit port and routes them to one of the three output ports. It consists of single input port and 3 output ports.
## Functions:
1. Input Register: This block is responsible for extracting the header, calculating and checking the parity.
2. Synchronizer: This block is responsible for decoding the header and determining the output portIt also provides synchronization between FSM and FIFO Modules. It allows faithful communication between the input port and the output port.
3. FSM: This block is basically a controller for the router. It generates necessary controls for FIFO, Synchroniser based on the values of status signals.
4. FIFO: This is an synchronous active low reset FIFO which allows simultaneous read and write operations.
## Procedure:
1. Designed a the block level structure for the Router.
2. Implemented the RTL Design using Verilog HDL and verified using individual verilog testbenches.
3. Synthesized and Implemented the design to generate a bit file and tested on FPGA.
4. Developed the class based verification environment and verified the 1x3 Router RTL model in system verilog using UVM Methodology.
