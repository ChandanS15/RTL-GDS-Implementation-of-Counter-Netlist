RTL coding is a way of converting design specification into set of high-level design using Hardware Description language called verilog.

In this repo you can find detailed explanantion of how to perform RTL-GDS flow of a simple Counter netlist including the details of Cadence tools used.

![RTL-GDS Flow from design specification to extracting GDS2 file](<Screenshot 2023-09-25 210709.png>)

The first step Design specification and RTL coding invloves conversion of desing specification into code using verilog HDL. The design is further verified using HDLs like System Verilog, Verilog or VHDL considering various parameters such as code coverage, functional coverage etc. Verification is one of the most tedious step where most of the engineers work on verifying the deign. There are various kinds of verification such as functional verification, formal verification. Functional simulation makes sure that the intended code works as expected. 

Cadence tool Xcelium Simulator is used to perform functional simulation of the deisng and it supports various languages such as verilog, systemVerilog etc.


![Running xcelium simulator](<Screenshot (89).png>)


![Xcelium simulator ](<Screenshot (90).png>)


![Running Xcelium Simulator](<Screenshot (91).png>)

Synthesis involves compilation, elaboration and simulation of the high-level design to obtain gate-level netlist. This step converts the high level coding constructs such as if-else-if, while and others into simple logical elements such as universal gates(AND, NAND, NOR), multiplexes, decoders and flipflops.

The below tcl script depicts the steps of synthesis where the design file is complied and elaborated to obtain the gate-level netlist file.


The TCL tool commnad language is used to have a  seamless communication between various EDA tools.

![TCL file for Genus](<Screenshot (92).png>)


![The gate-level synthesis of the counter](<Screenshot (102).png>)


