# Topic 7: Control

> HL only

## Key Concepts

### 7.1 Control Systems

#### Centralized vs. Distributed Systems
- **Centralized control**: single controller manages all operations
  - Advantages: simpler design, easier to monitor
  - Disadvantages: single point of failure, scalability limits
- **Distributed control**: multiple controllers share responsibilities
  - Advantages: fault tolerance, scalability, parallel processing
  - Disadvantages: complexity, synchronization challenges

#### Autonomous Agents
- Systems capable of operating on their own and making decisions without continuous human input
- **Sensors**: input devices that detect environmental changes
  - Temperature, pressure, light, motion, humidity, proximity
- **Actuators**: output devices that affect the environment
  - Motors, valves, heaters, displays, speakers
- **Microprocessors/microcontrollers**: embedded processors that control operations

### 7.2 Control System Types

#### Feedback Systems
- **Open-loop control**: no feedback; output not measured or compared to input
  - Example: a toaster timer (runs for set time regardless of toast state)
- **Closed-loop control**: the system measures its own output and uses that measurement to correct its behavior
  - Example: thermostat (measures temperature, adjusts heating/cooling)
  - Components: sensor → comparator → controller → actuator → process → (feedback to sensor)

#### Digital vs. Analog
- **Digital signals**: discrete values (0 or 1)
- **Analog signals**: continuous range of values
- **ADC** (Analog-to-Digital Converter): converts analog sensor readings to digital
- **DAC** (Digital-to-Analog Converter): converts digital signals to analog for actuators
- Sampling rate and resolution affect quality of analog-to-digital conversion

### 7.3 Robotics and Automation

- **Robot**: programmable machine capable of carrying out complex actions
- Components: sensors, actuators, processor, power supply, programming
- Industrial robots: manufacturing, assembly, welding, painting
- Autonomous vehicles: sensor fusion, decision-making, path planning
- **AI in control systems**: machine learning for adaptive control

### 7.4 Ethical and Social Implications

- Automation and employment: job displacement vs. new job creation
- Safety considerations in autonomous systems
- Privacy concerns with sensor data collection
- Reliability and accountability when systems fail
- Bias in AI-controlled systems
- Environmental impact of technology manufacturing and disposal

### 7.5 Applications of Control Systems

- **Smart home systems**: automated lighting, heating, security
- **Traffic control**: adaptive traffic signals, flow optimization
- **Industrial process control**: manufacturing quality, chemical processing
- **Medical devices**: patient monitoring, drug delivery systems
- **Environmental monitoring**: weather stations, pollution sensors
- **Agricultural technology**: precision farming, irrigation control

## Key Terminology

| Term | Definition |
|------|-----------|
| **Sensor** | A device that measures some physical property of the environment and converts it into a signal a processor can read |
| **Actuator** | A device that receives a control signal and produces a physical effect (movement, heat, sound, etc.) |
| **Open-loop control** | A control design where the system acts on fixed instructions with no measurement of the result |
| **Closed-loop control** | A control design where the output is continuously measured and fed back to correct the system's behavior |
| **ADC** | Analog-to-Digital Converter; samples a continuous signal and expresses it as digital values |
| **DAC** | Digital-to-Analog Converter; turns digital values back into a continuously varying signal |
| **Microcontroller** | A compact integrated circuit that combines a processor, memory, and I/O interfaces on one chip, designed for embedded control tasks |
| **Feedback** | The process of routing information about a system's output back to its input so the system can self-correct |

## Common Misconceptions

1. **"Automation always leads to unemployment"** — The historical pattern shows that automation tends to eliminate certain roles while creating new categories of work, though transitions can be disruptive.
2. **"Open-loop systems are always inferior"** — When the environment is predictable and high precision is not required, open-loop control is a perfectly valid choice that is simpler and cheaper to build.
3. **"Robots are always humanoid"** — The vast majority of robots are purpose-built machines for specific industrial tasks and look nothing like a human.
4. **"AI control systems are infallible"** — AI-driven controllers can fail in situations that were not well represented in training data.
5. **"Sensors provide perfect measurements"** — Every sensor has accuracy limits, a finite range, and a response time; real systems must account for noise and error.

## Comparison with AP CS

- AP CS A does not cover control systems, robotics, or embedded systems
- AP CS Principles covers some ethical/social implications of computing
- IB HL's control topic is unique among high-school CS curricula
- This topic connects computer science to engineering and real-world applications
