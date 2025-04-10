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

1) Accumulator (ACC): Central register for all operations
2) ALU: Performs addition, subtraction, and logic operations
3) Register File: Small set of general-purpose registers
4) Control Unit: Decodes instructions and generates control signals
5) Instruction Decoder: Extracts opcodes and operands
6) Data & Instruction Memory: Stores program and temporary data

# Data Flow:

1) Instruction is fetched from memory
2) Control unit decodes and signals the operation
3) Data moves from memory or registers to ACC
4) ALU performs operations using ACC and register/memory
5) Output is stored back to memory/registers if needed


> ## 🧾 Instruction Set
> 
> Below is the list of supported instructions for the 8-bit Accumulator-Based Processor:
>
> ```
> Opcode   Mnemonic   Description
> -------  ---------  -------------------------------
> 0001     LOAD       Load immediate value into ACC
> 0010     ADD        Add immediate value to ACC
> 0011     SUB        Subtract immediate value from ACC
> 0100     AND        Bitwise AND with immediate value
> 0101     OR         Bitwise OR with immediate value
> 0110     XOR        Bitwise XOR with immediate value
> 0111     NOT        Bitwise NOT of ACC (ignores operand)
> 1000     SHL        Shift ACC left by 1 bit
> 1001     SHR        Shift ACC right by 1 bit
> 1010     HALT       Halt execution
> ```



