# 5-Stage Pipelined RISC-V Processor

![Verilog](https://img.shields.io/badge/Verilog-HDL-blue)
![RISC-V](https://img.shields.io/badge/ISA-RISC--V-green)
![Pipeline](https://img.shields.io/badge/Architecture-5--Stage%20Pipeline-orange)
![Simulation](https://img.shields.io/badge/Tested-QuestaSim-success)

A complete Verilog implementation of a 5-stage pipelined RISC-V processor with advanced hazard handling and dual-phase clocking architecture.

## 📋 Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Architecture](#architecture)
- [Instruction Set](#instruction-set)
- [Pipeline Stages](#pipeline-stages)
- [Installation](#installation)
- [Simulation](#simulation)
- [Results](#results)
- [Future Work](#future-work)
- [Contributing](#contributing)
- [License](#license)

## 🏗️ Overview

This project implements a fully functional 5-stage pipelined RISC-V processor in Verilog HDL. The design demonstrates fundamental computer architecture concepts including instruction pipelining, hazard detection, and data forwarding mechanisms.

## ✨ Features

- **5-Stage Pipeline Architecture** - IF, ID, EX, MEM, WB
- **Dual-Phase Clocking** - Separate clocks for odd/even pipeline stages
- **Comprehensive Instruction Support** - Arithmetic, Memory, Control Flow
- **Advanced Hazard Handling** - Branch prediction and data forwarding
- **32-bit RISC Architecture** - 32-bit data path and instructions
- **Memory System** - 1024×32-bit data memory
- **Register File** - 32×32-bit general purpose registers

## 🏛️ Architecture

### Pipeline Structure
