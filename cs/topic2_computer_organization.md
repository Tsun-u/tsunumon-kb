# Topic 2: Computer Organization

> SL + HL | Core Topic

## Key Concepts

### 2.1 Computer Architecture

#### CPU Architecture
- **Von Neumann architecture**: single memory for instructions and data
  - Components: ALU (arithmetic logic unit), control unit (CU), registers, buses
  - **Memory Address Register (MAR)**: holds address of memory being accessed
  - **Memory Data Register (MDR)**: holds data being transferred to/from memory
  - **Program Counter (PC)**: holds address of next instruction
  - **Accumulator (ACC)**: holds results of ALU operations
- **Fetch-decode-execute cycle**:
  1. Fetch: instruction retrieved from memory (address in PC → MAR → memory → MDR)
  2. Decode: control unit interprets the instruction
  3. Execute: ALU performs the operation

#### Machine Instruction Cycle
- Clock speed: frequency of fetch-decode-execute cycles (measured in GHz)
- Factors affecting CPU performance: clock speed, number of cores, cache size, word size

### 2.2 Secondary Memory

- Types of storage:
  - **Magnetic**: HDD (high capacity, cheaper, mechanical)
  - **Solid-state**: SSD, USB flash drives (faster, no moving parts, more expensive)
  - **Optical**: CD, DVD, Blu-ray (portable, archival)
- Storage capacity: bits, bytes, KB, MB, GB, TB, PB
- Volatile vs. non-volatile memory
- **RAM** (Random Access Memory): volatile, fast, working memory
- **ROM** (Read-Only Memory): non-volatile, stores firmware/BIOS

### 2.3 Operating Systems and Application Software

- **Operating system** functions:
  - Memory management, process management, file management
  - User interface (CLI, GUI)
  - Device driver management
  - Security (authentication, access control)
- **Application software**: word processors, databases, spreadsheets, browsers
- Utility software: antivirus, disk management, compression tools

### 2.4 Binary Representation

- **Binary number system**: base-2 (0 and 1)
- Binary ↔ decimal conversion
- Binary addition and subtraction
- **Hexadecimal**: base-16 (0--9, A--F); compact binary representation
- Data representation:
  - **ASCII**: 7-bit character encoding (128 characters)
  - **Unicode**: supports all world scripts (UTF-8, UTF-16)
  - **Pixels and color depth**: RGB color model; bit depth determines colors available

### 2.5 Logic Gates

- Basic gates: AND, OR, NOT, NAND, NOR, XOR
- Truth tables for all basic gates
- Constructing logic circuits from Boolean expressions
- Simplifying Boolean expressions using logic laws

## Key Terminology

| Term | Definition |
|------|-----------|
| **ALU** | Arithmetic Logic Unit; performs calculations and logical operations |
| **Fetch-decode-execute cycle** | Steps the CPU follows to process each instruction |
| **RAM** | Random Access Memory; volatile working memory |
| **ROM** | Read-Only Memory; non-volatile memory for firmware |
| **Cache** | Small, fast memory between CPU and main memory |
| **ASCII** | American Standard Code for Information Interchange; 7-bit character encoding |
| **Logic gate** | Electronic circuit that performs a Boolean operation |

## Common Misconceptions

1. **"More RAM means a faster computer"** -- RAM affects multitasking capacity, not raw speed; CPU and storage speed also matter.
2. **"Deleting files removes them permanently"** -- Typically only the reference is removed; data remains until overwritten.
3. **"Binary is only used in computers"** -- Binary is the foundation of all digital systems, including phones, IoT devices, etc.
4. **"Higher clock speed always means better performance"** -- Architecture, cores, cache, and software optimization also matter significantly.

## Comparison with AP CS

- AP CS Principles covers binary, data representation, and basic computer architecture
- AP CS A does not cover hardware or organization
- IB CS covers logic gates and CPU architecture in more detail than AP CS Principles
