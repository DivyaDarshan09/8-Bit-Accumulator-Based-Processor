# 8-Bit-Accumulator-Based-Processor
🧠 A minimalistic 8-bit accumulator-based processor designed using Verilog. This CPU is ideal for learning digital design principles, understanding instruction flow, and experimenting with basic processor architecture. It supports memory-based operations and includes a register file for enhanced data handling.


# Overview
This project implements a basic 8-bit CPU using an accumulator-based architecture. It is designed with modular Verilog code, intended for both simulation and hardware implementation on FPGAs or ASIC flows like Tiny Tapeout. The processor supports essential operations including arithmetic and memory interactions.



# Features
1) 8-bit data width
2) Simple accumulator-centric operations
3) Register File integration
4) 4-bit instruction opcodes
5) Easy-to-extend architecture
6) FPGA and ASIC-compatible design
6) Modular, readable Verilog code


# Architecture
# Main Modules:

a) Accumulator (ACC): Central register for all operations
b) ALU: Performs addition, subtraction, and logic operations
c) Register File: Small set of general-purpose registers
d) Control Unit: Decodes instructions and generates control signals
e) Instruction Decoder: Extracts opcodes and operands
f) Data & Instruction Memory: Stores program and temporary data

# Data Flow:

Instruction is fetched from memory
Control unit decodes and signals the operation
Data moves from memory or registers to ACC
ALU performs operations using ACC and register/memory
Output is stored back to memory/registers if needed

# Instruction Set
Opcode	Mnemonic	Description
0000	LOAD	Load data from memory to ACC
0001	ADD	Add register to ACC
0010	SUB	Subtract register from ACC
0011	STORE	Store ACC value to memory
0100	MOV	Move data between registers
0101	NOP	No operation
0110	CLR	Clear accumulator
0111	JMP	Jump to specified address
