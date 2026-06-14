# Topic 2: Computer Organization

> SL + HL | Core Topic

## Key Concepts

### 2.1 Computer Architecture

#### CPU Architecture
- **Von Neumann architecture**: a design where instructions and data share the same memory space
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
| **ALU** | Arithmetic Logic Unit; the CPU component that carries out arithmetic and logic operations |
| **Fetch-decode-execute cycle** | The repeating sequence a CPU follows to retrieve, interpret, and carry out each instruction |
| **RAM** | Random Access Memory; fast, volatile memory used for active programs and data |
| **ROM** | Read-Only Memory; persistent memory that retains content without power, used for firmware |
| **Cache** | A small, very fast memory layer sitting between the CPU and main RAM |
| **ASCII** | American Standard Code for Information Interchange; a 7-bit encoding scheme for text characters |
| **Logic gate** | An electronic building block that computes a Boolean output from one or more inputs |

## Common Misconceptions

1. **"More RAM means a faster computer"** — RAM determines how much can run at once, not raw processor speed; CPU architecture and storage speed also matter significantly.
2. **"Deleting files removes them permanently"** — Usually only the file's entry in the directory is removed; the underlying data stays on disk until new data overwrites it.
3. **"Binary is only used in computers"** — Binary underlies all digital systems, from smartphones to IoT sensors.
4. **"Higher clock speed always means better performance"** — Factors like core count, cache size, memory bandwidth, and software design all affect real-world speed.

## Comparison with AP CS

- AP CS Principles covers binary, data representation, and basic computer architecture
- AP CS A does not cover hardware or organization
- IB CS covers logic gates and CPU architecture in more detail than AP CS Principles
