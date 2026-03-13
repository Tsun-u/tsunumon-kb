# Big Idea 4: Computing Systems and Networks (CSN)
> Exam Weight: 11-15%

Computer systems and networks are used to transfer data. Finding, understanding, and evaluating the use of resources on the Internet are essential skills for today's computing professional.

## Topics

### CSN-1: The Internet

#### CSN-1.A: Explain how computing devices work together in a network
- **Essential Knowledge:**
  - A computing device is a physical artifact that can run a program (computers, tablets, servers, routers, smart sensors)
  - A computing system is a group of computing devices and programs working together for a common purpose
  - A computer network is a group of interconnected computing devices capable of sending or receiving data
  - A computer network is a type of computing system
  - A path between two computing devices on a computer network (a sender and a receiver) is a sequence of directly connected computing devices that begins at the sender and ends at the receiver
  - Routing is the process of finding a path from sender to receiver

#### CSN-1.B: Explain how the Internet works
- **Essential Knowledge:**
  - The Internet is a computer network consisting of interconnected networks that use standardized, open (nonproprietary) communication protocols
  - Access to the Internet depends on the ability to connect to an Internet-connected device, either directly or through a network
  - A protocol is an agreed-upon set of rules that specify the behavior of a system
  - The Internet is built on the TCP/IP protocol suite:
    - **IP (Internet Protocol):** Responsible for addressing and routing packets
    - **TCP (Transmission Control Protocol):** Provides reliable, ordered delivery of data
    - **UDP (User Datagram Protocol):** Provides fast but less reliable delivery
  - The World Wide Web (WWW) is NOT the same as the Internet; it is a system of linked pages, programs, and files accessed via the Internet
  - HTTP/HTTPS is the protocol used for transmitting web pages

#### CSN-1.C: Explain how data are sent through the Internet via packets
- **Essential Knowledge:**
  - Information is passed through the Internet as a data stream, which is a sequence of data sent in a specific order
  - Data streams contain chunks of data called packets
  - Each packet contains a chunk of data and metadata used for routing the packet between the origin and the destination on the Internet, as well as for data reassembly
  - Packets may arrive at the destination in a different order than they were sent; the recipient's device uses metadata to reassemble the data correctly
  - Packets may take different paths through the Internet to reach their destination

#### CSN-1.D: Describe the differences between the Internet and the World Wide Web
- **Essential Knowledge:**
  - The Internet is the underlying network infrastructure
  - The World Wide Web is a system of interlinked hypertext documents and resources accessed via the Internet using HTTP/HTTPS and web browsers
  - The World Wide Web uses the Internet to access and share information

#### CSN-1.E: For fault-tolerant systems
- **Essential Knowledge:**
  - The Internet has been engineered to be fault-tolerant, meaning it can support failures and still continue to function
  - Redundancy is the inclusion of extra components or pathways so that if one fails, another can take over
  - The redundancy of routing options between two points on the Internet increases the reliability of the Internet and helps it scale to more devices and more people
  - If a particular device or connection on the Internet fails, subsequent data will be sent via a different route (if available)
  - A network with more connections (more redundancy) is generally more fault-tolerant
  - Redundancy within a system often requires additional resources but can provide the benefit of fault tolerance

---

### CSN-2: Parallel and Distributed Computing

#### CSN-2.A: For sequential, parallel, and distributed computing
- **Essential Knowledge:**
  - Sequential computing is a computational model in which operations are performed in order, one at a time
  - Parallel computing is a computational model where the program is broken into multiple smaller sequential computing operations, some of which are performed simultaneously
  - Distributed computing is a computational model in which multiple devices are used to run a program
  - Comparing efficiency of solutions can be done by comparing the time it takes to perform the same task

#### CSN-2.B: For parallel and distributed computing
- **Essential Knowledge:**
  - Parallel computing consists of a parallel portion and a sequential portion
  - The "speedup" of a parallel solution is measured in the time it takes to complete the task sequentially divided by the time it takes to complete the task in parallel
  - Solutions that use parallel computing can scale more effectively than solutions that use sequential computing
  - Distributed computing allows problems to be solved that could not be solved on a single computer due to processing time or storage needs
  - Distributed computing allows much larger problems to be solved quicker than would be possible with a single computer
  - When increasing the use of parallel computing in a solution, the efficiency of the solution is still limited by the sequential portion — this is known as Amdahl's Law
