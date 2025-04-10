# 8-Bit-Accumulator-Based-Processor
🧠 A minimalistic 8-bit accumulator-based processor designed using Verilog. This CPU is ideal for learning digital design principles, understanding instruction flow, and experimenting with basic processor architecture. It supports memory-based operations and includes a register file for enhanced data handling.

Overview
This project implements a basic 8-bit CPU using an accumulator-based architecture. It is designed with modular Verilog code, intended for both simulation and hardware implementation on FPGAs or ASIC flows like Tiny Tapeout. The processor supports essential operations including arithmetic and memory interactions.

Features
8-bit data width

Simple accumulator-centric operations

Register File integration

4-bit instruction opcodes

Easy-to-extend architecture

FPGA and ASIC-compatible design

Modular, readable Verilog code

Architecture
Main Modules:

Accumulator (ACC): Central register for all operations

ALU: Performs addition, subtraction, and logic operations

Register File: Small set of general-purpose registers

Control Unit: Decodes instructions and generates control signals

Instruction Decoder: Extracts opcodes and operands

Data & Instruction Memory: Stores program and temporary data

Data Flow:

Instruction is fetched from memory

Control unit decodes and signals the operation

Data moves from memory or registers to ACC

ALU performs operations using ACC and register/memory

Output is stored back to memory/registers if needed

Instruction Set
Opcode	Mnemonic	Description
0000	LOAD	Load data from memory to ACC
0001	ADD	Add register to ACC
0010	SUB	Subtract register from ACC
0011	STORE	Store ACC value to memory
0100	MOV	Move data between registers
0101	NOP	No operation
0110	CLR	Clear accumulator
0111	JMP	Jump to specified address
Sample Waveform
The simulation demonstrates:

Loading a value into the accumulator

Performing an ADD operation using Register File

Storing the result into memory
