# Topic 3: Networks

> SL + HL | Core Topic

## Key Concepts

### 3.1 Network Fundamentals

#### Network Types
- **LAN** (Local Area Network): small geographic area (building, campus)
- **WAN** (Wide Area Network): large geographic area; uses public infrastructure
- **WLAN**: wireless LAN (Wi-Fi)
- **VPN** (Virtual Private Network): secure tunnel over public network
- **Internet**: global network of interconnected networks
- **Intranet**: private network within an organization

#### Network Topologies
- **Bus**: all devices on a single cable; simple but single point of failure
- **Star**: all devices connect to a central switch/hub; most common
- **Mesh**: every device connected to every other; high redundancy
- **Ring**: devices in a circular chain

#### Network Hardware
- **Router**: forwards packets between networks; operates at Layer 3 (Network)
- **Switch**: forwards frames within a network; operates at Layer 2 (Data Link)
- **Hub**: broadcasts to all ports (obsolete, replaced by switches)
- **Wireless access point**: provides Wi-Fi connectivity
- **Modem**: converts digital ↔ analog signals
- **Firewall**: monitors and filters network traffic based on rules

### 3.2 Data Transmission

#### Protocols
- **TCP/IP** model layers:
  - Application layer (HTTP, FTP, SMTP, DNS)
  - Transport layer (TCP, UDP)
  - Internet layer (IP)
  - Network interface layer (Ethernet, Wi-Fi)
- **HTTP/HTTPS**: web browsing (HTTPS = encrypted with TLS/SSL)
- **FTP**: file transfer
- **SMTP/POP/IMAP**: email
- **DNS**: translates domain names to IP addresses

#### Packet Switching
- Data divided into **packets**: header (source, destination, sequence) + payload
- Packets may take different routes; reassembled at destination
- Advantages: efficient use of bandwidth, fault tolerance
- TCP ensures reliable delivery; UDP is faster but unreliable

#### IP Addressing
- **IPv4**: 32-bit address (e.g., 192.168.1.1); ~4.3 billion addresses
- **IPv6**: 128-bit address; vastly more addresses
- **Subnet mask**: defines network and host portions of IP address
- **MAC address**: unique hardware address (48-bit); operates at Layer 2

### 3.3 Network Security

- **Threats**: malware (virus, worm, trojan, ransomware), phishing, DDoS, man-in-the-middle
- **Encryption**: converting data to unreadable form
  - Symmetric (same key) vs. asymmetric (public/private key pair)
  - SSL/TLS for secure web communication
- **Authentication**: passwords, biometrics, multi-factor authentication (MFA)
- **Firewall**: packet filtering, stateful inspection
- **Social engineering**: manipulating humans to gain unauthorized access

### 3.4 Web Technologies
- URL structure, domain names, web servers
- Client-server model
- Cookies and sessions
- Cloud computing: IaaS, PaaS, SaaS

## Key Terminology

| Term | Definition |
|------|-----------|
| **LAN** | Local Area Network; covers a small geographic area |
| **TCP/IP** | Protocol suite governing internet communication |
| **Packet** | Unit of data transmitted across a network with header and payload |
| **DNS** | Domain Name System; translates domain names to IP addresses |
| **Encryption** | Process of encoding data so only authorized parties can read it |
| **Firewall** | Security system that monitors and controls network traffic |
| **VPN** | Virtual Private Network; encrypted tunnel over public network |
| **MAC address** | Unique hardware identifier assigned to network interfaces |

## Common Misconceptions

1. **"The internet and the web are the same"** -- The internet is the network infrastructure; the web (WWW) is a service that runs on it.
2. **"HTTPS is completely secure"** -- HTTPS encrypts data in transit but does not protect against all threats (e.g., compromised server, phishing).
3. **"A firewall stops all attacks"** -- Firewalls filter traffic by rules but cannot stop all threats (e.g., social engineering, zero-day exploits).
4. **"Wi-Fi and internet are the same"** -- Wi-Fi is a wireless network technology; you can have Wi-Fi without internet access.

## Comparison with AP CS

- AP CS Principles covers the internet, protocols, and cybersecurity at a conceptual level
- IB CS goes deeper into network hardware, topologies, and TCP/IP layers
- AP CS A does not cover networking
- IB CS covers network security with more technical detail (encryption types, attack vectors)
