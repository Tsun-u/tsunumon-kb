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
- Systems that can operate independently and make decisions
- **Sensors**: input devices that detect environmental changes
  - Temperature, pressure, light, motion, humidity, proximity
- **Actuators**: output devices that affect the environment
  - Motors, valves, heaters, displays, speakers
- **Microprocessors/microcontrollers**: embedded processors that control operations

### 7.2 Control System Types

#### Feedback Systems
- **Open-loop control**: no feedback; output not measured or compared to input
  - Example: a toaster timer (runs for set time regardless of toast state)
- **Closed-loop control**: output is measured and fed back to adjust input
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
| **Sensor** | Device that detects and measures physical properties of the environment |
| **Actuator** | Device that converts control signals into physical action |
| **Open-loop control** | System with no feedback; operates on preset instructions |
| **Closed-loop control** | System that uses feedback to adjust its operation |
| **ADC** | Analog-to-Digital Converter; converts continuous signals to discrete |
| **DAC** | Digital-to-Analog Converter; converts discrete signals to continuous |
| **Microcontroller** | Small computer on a single chip designed for embedded applications |
| **Feedback** | Output information returned to the input to adjust system behavior |

## Common Misconceptions

1. **"Automation always leads to unemployment"** -- Historically, automation creates new types of jobs even as it eliminates others.
2. **"Open-loop systems are always inferior"** -- Open-loop is simpler and cheaper; appropriate when conditions are predictable and precision is not critical.
3. **"Robots are always humanoid"** -- Most robots are industrial machines designed for specific tasks, not human-like.
4. **"AI control systems are infallible"** -- AI systems can make errors, especially in situations not represented in training data.
5. **"Sensors provide perfect measurements"** -- All sensors have limitations: accuracy, precision, range, and response time.

## Comparison with AP CS

- AP CS A does not cover control systems, robotics, or embedded systems
- AP CS Principles covers some ethical/social implications of computing
- IB HL's control topic is unique among high-school CS curricula
- This topic connects computer science to engineering and real-world applications
