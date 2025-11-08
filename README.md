# **5-Stage Pipelined RISC-V Processor**

---

## **🏗️ Architecture Overview**
- **5-Stage Pipeline**: IF (Instruction Fetch) → ID (Instruction Decode) → EX (Execute) → MEM (Memory Access) → WB (Write Back)
- **Dual-Phase Clocking**: Separate clocks for odd/even pipeline stages  
- **32-bit RISC Architecture**: 32-bit data path and instructions

---

## **📋 Supported Instruction Set**

### **Arithmetic Instructions**
- **ADD, SUB, AND, OR, SLT, MUL**

### **Immediate Operations**
- **ADDI, SUBI, ANDI, ORI, SLTI**

### **Memory Access**
- **LW** (Load Word), **SW** (Store Word)

### **Control Flow**
- **BEQZ** (Branch if Zero), **BNEQZ** (Branch if Not Zero)

### **System Instructions**
- **HLT** (Halt)

---

## **🎯 Key Features**
- **Pipelined Execution**: Multiple instructions processed simultaneously
- **Register File**: 32×32-bit general purpose registers
- **Data Memory**: 1024×32-bit memory space
- **Hazard Handling**: Branch prediction and data forwarding
- **Instruction Types**: RR (Register-Register), RM (Register-Immediate), Load/Store, Branch

---

## **🔧 Pipeline Stages**

### **1. Instruction Fetch (IF)**
- Fetches instructions from memory
- Handles branch prediction
- Manages program counter

### **2. Instruction Decode (ID)**
- Decodes instruction opcode
- Reads register values
- Sign-extends immediate values

### **3. Execute (EX)**
- Performs ALU operations
- Calculates memory addresses
- Evaluates branch conditions

### **4. Memory Access (MEM)**
- Reads/writes data memory
- Handles load/store operations

### **5. Write Back (WB)**
- Writes results to registers
- Updates processor state

---

## **📁 Project Files**
- **RISC_V.v** - Main processor implementation
- **Testbench** - Verification and testing

---

## **🚀 Simulation**
The design can be simulated using Verilog simulators like:
- **ModelSim**
- **Icarus Verilog** 
- **VCS**

---

## **🛠️ Usage**
```verilog
module top;
  wire clk1, clk2;
  pipe_MIPS processor (.clk1(clk1), .clk2(clk2));
endmodule
