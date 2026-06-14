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
- **Encryption**: transforming data into an unreadable form that only authorized parties can decode
  - Symmetric (same key) vs. asymmetric (public/private key pair)
  - SSL/TLS for secure web communication
- **Authentication**: passwords, biometrics, multi-factor authentication (MFA)
- **Firewall**: packet filtering, stateful inspection
- **Social engineering**: tricking people into handing over credentials or access rather than attacking the technology directly

### 3.4 Web Technologies
- URL structure, domain names, web servers
- Client-server model
- Cookies and sessions
- Cloud computing: IaaS, PaaS, SaaS

## Key Terminology

| Term | Definition |
|------|-----------|
| **LAN** | Local Area Network; a network confined to a limited physical space |
| **TCP/IP** | The layered protocol suite that governs how data travels across the internet |
| **Packet** | A chunk of data prepared for transmission, containing a header with routing info and a payload |
| **DNS** | Domain Name System; the service that resolves human-readable domain names into IP addresses |
| **Encryption** | Converting data into a coded form so that only parties with the correct key can read it |
| **Firewall** | A system that inspects and selectively blocks network traffic according to security rules |
| **VPN** | Virtual Private Network; an encrypted connection that creates a private channel over a public network |
| **MAC address** | A fixed hardware identifier burned into a network interface card, unique to each device |

## Common Misconceptions

1. **"The internet and the web are the same"** — The internet is the underlying global network of connected computers; the World Wide Web is one service that runs on top of it.
2. **"HTTPS is completely secure"** — HTTPS protects data while it travels between client and server but cannot guard against a compromised server or a user falling for a phishing page.
3. **"A firewall stops all attacks"** — Firewalls enforce rule-based filtering but cannot catch everything; social engineering, zero-day exploits, and insider threats slip through.
4. **"Wi-Fi and internet are the same"** — Wi-Fi is a short-range wireless networking technology; it connects devices to a local network, which may or may not have an internet connection.

## Comparison with AP CS

- AP CS Principles covers the internet, protocols, and cybersecurity at a conceptual level
- IB CS goes deeper into network hardware, topologies, and TCP/IP layers
- AP CS A does not cover networking
- IB CS covers network security with more technical detail (encryption types, attack vectors)
