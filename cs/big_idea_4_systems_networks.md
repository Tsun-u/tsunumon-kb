# Big Idea 4: Computing Systems and Networks (CSN)
> Exam Weight: 11-15%

Computing systems and networks are responsible for moving data around. Being able to find, understand, and evaluate resources on the internet is an essential skill in modern computing.

## Topics

### How the Internet Works

#### How Devices in a Network Work Together

- A **computing device** is any physical device capable of running a program, including computers, tablets, servers, routers, and smart sensors
- A **computing system** is a group of devices and programs working together toward a common purpose
- A **computer network** is a group of connected devices that can send and receive data with one another
- A computer network is a specialized type of computing system
- In a network, a **path** from sender to receiver is a chain of directly connected devices
- **Routing** is the process of finding the best path from sender to receiver

#### The Architecture of the Internet

- The internet is a large computer network made up of many interconnected networks, using open, standardized communication protocols
- Connecting to the internet depends on having access to a device that is already connected (directly or through another network)
- A **protocol** is a set of agreed-upon rules that govern how systems behave
- The internet is built on the TCP/IP protocol suite:
  - **IP (Internet Protocol)**: handles address assignment and packet routing
  - **TCP (Transmission Control Protocol)**: ensures data is delivered reliably and in order
  - **UDP (User Datagram Protocol)**: transmits data faster but without reliability guarantees
- The **World Wide Web (WWW)** is not the same as the internet: the internet is the underlying infrastructure, while the WWW is the system of hyperlinked documents that runs on top of it
- HTTP/HTTPS are the protocols used to transfer web pages

#### How Data Travels Across Networks as Packets

- Information on the internet is sent as a **data stream** — a sequence of data arranged in a specific order
- Data streams are broken into chunks called **packets**
- Each packet carries a portion of the actual data, plus metadata used for routing and reassembly
- Packets from the same data stream may arrive out of order; the receiving device uses the metadata to reassemble them correctly
- Different packets from the same transmission may travel along different paths to reach the destination

#### The Difference Between the Internet and the World Wide Web

- The internet is the underlying network infrastructure
- The World Wide Web is a system of hyperlinked documents and resources accessed through HTTP/HTTPS and a browser — it runs on top of the internet
- The WWW uses the internet to access and share information

#### Fault Tolerance by Design

- The internet is designed to be **fault-tolerant**: even if some components fail, the overall system keeps working
- **Redundancy** means adding backup components or paths so that if one path fails, data can reroute through another
- More routing options between two points means more redundancy, and in turn a more reliable and scalable internet
- If a device or connection on the internet fails, subsequent data is automatically redirected through available alternative paths
- More network connections (higher redundancy) generally means stronger fault tolerance
- Redundancy requires additional resources but delivers higher system reliability in return

---

### Parallel and Distributed Computing

#### Sequential, Parallel, and Distributed Computing Models

- **Sequential computing**: operations execute one after another in order
- **Parallel computing**: a program is broken into smaller sequential subtasks, and some of them run simultaneously
- **Distributed computing**: multiple devices work together to execute a single program
- Efficiency can be compared by measuring how long it takes to complete the same task under each approach

#### Characteristics of Parallel and Distributed Computing

- A parallel solution has portions that can run in parallel and portions that must still run sequentially
- The **speedup** of a parallel solution is defined as: sequential execution time ÷ parallel execution time
- Solutions that use parallel computing generally scale better than purely sequential solutions
- Distributed computing makes it possible to solve problems that would exceed the processing time or storage capacity of any single machine
- Distributed computing lets large problems be solved faster than a single computer could manage
- As the degree of parallelism increases, overall efficiency is still bounded by the portion that must run sequentially — this is known as **Amdahl's Law**
