# IB® Computer Science (SL/HL) -- Course Framework

> Covers concepts aligned with the IB Diploma Programme Computer Science curriculum.
> Two syllabuses currently coexist: the **outgoing** syllabus (Topics 1--7, final assessment 2026) and the **new** syllabus (Themes A/B, first teaching 2025, **first assessment 2027**) which adds **machine learning** and **databases**.
> Last updated: 2026-06-10

## Current Syllabus Structure (First Assessment through 2026)

The current IB Computer Science course is organized into **7 topics** (Topics 1--4 for SL, Topics 1--7 for HL).

### Topics

| Topic | Name | Level | File |
|-------|------|-------|------|
| 1 | [System Fundamentals](https://tsun-u.github.io/tsunumon-kb/cs/topic1_system_fundamentals.md) | SL+HL | |
| 2 | [Computer Organization](https://tsun-u.github.io/tsunumon-kb/cs/topic2_computer_organization.md) | SL+HL | |
| 3 | [Networks](https://tsun-u.github.io/tsunumon-kb/cs/topic3_networks.md) | SL+HL | |
| 4 | [Computational Thinking, Problem-Solving and Programming](https://tsun-u.github.io/tsunumon-kb/cs/topic4_computational_thinking.md) | SL+HL | |
| 5 | [Abstract Data Structures](https://tsun-u.github.io/tsunumon-kb/cs/topic5_abstract_data_structures.md) | HL only | |
| 6 | [Resource Management](https://tsun-u.github.io/tsunumon-kb/cs/topic6_resource_management.md) | HL only | |
| 7 | [Control](https://tsun-u.github.io/tsunumon-kb/cs/topic7_control.md) | HL only | |

## Teaching Hours

| Level | Core (Topics 1--4) | HL Extension (Topics 5--7) | Case Study | IA | Total |
|-------|--------------------|-----------------------------|------------|-----|-------|
| SL | 80 | -- | 30 | 40 | 150 |
| HL | 80 | 45 | 30 | 40 + 45 | 240 |

## Assessment

### External Assessment

| Paper | Content | SL Time | HL Time | SL Weight | HL Weight |
|-------|---------|---------|---------|-----------|-----------|
| 1 | Short-answer questions (Topics 1--4, case study) | 90 min | 130 min | 45% | 40% |
| 2 | Object-oriented programming (Topic 4/5) | 45 min | 45 min | 25% | 20% |
| 3 | Case study (HL only) | -- | 60 min | -- | 20% |

### Internal Assessment

| Component | Description | Weight |
|-----------|-------------|--------|
| Solution | Computational solution to a specified client problem | 30% (SL) / 20% (HL) |

## New Syllabus (First Teaching 2025, First Assessment 2027)

The new syllabus restructures the course into **two themes**. The most significant additions are **A3 Databases** and **A4 Machine Learning**, which did not exist in the outgoing syllabus.

| Theme | Name | Focus |
|-------|------|-------|
| **A** | Concepts of Computer Science | Hardware/fundamentals, networks, databases, machine learning |
| **B** | Computational Thinking and Problem Solving | Computational thinking, programming, OOP, abstract data types |

### Theme A: Concepts of Computer Science

| Topic | Name | Level | File |
|-------|------|-------|------|
| A1 | Computer Fundamentals (A1.1 hardware & operation, A1.2 data representation & logic, A1.3 operating/control systems, **A1.4 translation HL only**) | SL+HL | concepts covered in [topic1](https://tsun-u.github.io/tsunumon-kb/cs/topic1_system_fundamentals.md) / [topic2](https://tsun-u.github.io/tsunumon-kb/cs/topic2_computer_organization.md) |
| A2 | Networks (A2.1 fundamentals, A2.2 architecture, A2.3 data transmission, A2.4 security) | SL+HL | concepts covered in [topic3](https://tsun-u.github.io/tsunumon-kb/cs/topic3_networks.md) |
| A3 | Databases (A3.1 fundamentals, A3.2 design, A3.3 programming, **A3.4 alternative DBs & data warehouses HL only**) | SL+HL | *new topic — not yet a standalone file* |
| **A4** | **Machine Learning (A4.1 fundamentals, A4.2 data preprocessing HL, A4.3 ML approaches HL, A4.4 ethics)** | SL+HL | [**theme_a4_machine_learning.md**](https://tsun-u.github.io/tsunumon-kb/cs/theme_a4_machine_learning.md) |

### Theme B: Computational Thinking and Problem Solving

| Topic | Name | Level | File |
|-------|------|-------|------|
| B1 | Computational Thinking | SL+HL | concepts covered in [topic4](https://tsun-u.github.io/tsunumon-kb/cs/topic4_computational_thinking.md) |
| B2 | Programming (fundamentals, data structures, constructs, algorithms, file processing) | SL+HL | concepts covered in [topic4](https://tsun-u.github.io/tsunumon-kb/cs/topic4_computational_thinking.md) |
| B3 | Object-Oriented Programming (**B3.2 multiple classes HL only**) | SL+HL | concepts covered in [topic4](https://tsun-u.github.io/tsunumon-kb/cs/topic4_computational_thinking.md) |
| B4 | Abstract Data Types | HL only | concepts covered in [topic5](https://tsun-u.github.io/tsunumon-kb/cs/topic5_abstract_data_structures.md) |

> **ML/NN questions** (e.g. neural networks, perceptron, MLP, CNN, training, and LLM/RAG applications) are served by **[theme_a4_machine_learning.md](https://tsun-u.github.io/tsunumon-kb/cs/theme_a4_machine_learning.md)** — the new syllabus is the only IB/AP framework with explicit ML content.

## Key Differences from AP Computer Science

- IB CS covers **broader topics** (networking, databases, control systems, machine learning) vs. AP CS A's focus on Java programming
- AP CS A is purely **programming-focused** (Java); IB CS includes significant **theory** (system design, networking, ML)
- IB CS HL covers **abstract data structures** (linked lists, trees, stacks, queues) similar to a university data structures course
- AP CS Principles is closer to IB CS SL in breadth but with less programming depth
- IB CS includes a **case study** component; AP does not
- IB CS requires an **Internal Assessment** (computational solution for a real client); AP has no equivalent
- The new IB syllabus (2027) adds **machine learning** (neural networks, deep learning) and **databases** as explicit topics — neither AP CS A nor AP CSP covers neural-network theory

## Usage Notes for AI Teaching Agent

- Always specify SL vs. HL content boundaries
- For the new syllabus, use topic codes (e.g., A4.3) when referencing specific content
- IB CS emphasizes **system design** and **real-world application** more than AP
- Programming examples should be in **Java** (IB's officially supported language) or pseudocode
- The case study changes annually; focus on transferable concepts rather than case-study-specific details
- For **machine learning / neural network** questions, route to [theme_a4_machine_learning.md](https://tsun-u.github.io/tsunumon-kb/cs/theme_a4_machine_learning.md); IB depth is **principles + ethics, no mathematical derivation or implementation**
