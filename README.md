5-Stage Pipelined RISC-V Processor
This project implements a complete 5-stage pipelined RISC-V processor in Verilog, demonstrating fundamental computer architecture concepts through a working CPU design.

🏗️ Architecture
5-Stage Pipeline: IF (Instruction Fetch) → ID (Instruction Decode) → EX (Execute) → MEM (Memory Access) → WB (Write Back)

Dual-Phase Clocking: Separate clocks for odd/even pipeline stages

32-bit RISC Architecture: 32-bit data path and instructions

📋 Supported Instructions
Arithmetic: ADD, SUB, AND, OR, SLT, MUL

Immediate Operations: ADDI, SUBI, ANDI, ORI, SLTI

Memory Access: LW (Load Word), SW (Store Word)

Control Flow: BEQZ (Branch if Zero), BNEQZ (Branch if Not Zero)

System: HLT (Halt)

🎯 Key Features
Pipelined Execution: Multiple instructions processed simultaneously

Register File: 32×32-bit general purpose registers

Data Memory: 1024×32-bit memory space

Hazard Handling: Branch prediction and data forwarding

Instruction Types: RR (Register-Register), RM (Register-Immediate), Load/Store, Branch

🔧 Pipeline Stages
IF: Fetches instructions from memory, handles branches

ID: Decodes instructions, reads registers, sign-extends immediates

EX: Performs ALU operations, calculates addresses

MEM: Reads/writes data memory

WB: Writes results back to register file
