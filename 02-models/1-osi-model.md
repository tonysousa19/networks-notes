# OSI Model

## Definition

The OSI (Open Systems Interconnection) model is a conceptual framework used to understand how devices communicate over a network.

It divides network communication into **seven layers**, where each layer has a specific responsibility.

The model helps professionals troubleshoot networks, design systems, and understand how data moves.

---

# The 7 Layers of the OSI Model

## Layer 7 - Application

### Purpose

The Application layer is the closest layer to the user.

It provides network services directly to applications.

### Examples

- Web browsers
- Email clients
- File transfer applications

### Protocols

- HTTP
- HTTPS
- FTP
- DNS
- SMTP

---

## Layer 6 - Presentation

### Purpose

The Presentation layer handles how data is formatted and represented.

It ensures that different systems can understand the data.

### Responsibilities

- Data translation
- Encryption
- Compression

### Examples

- SSL/TLS encryption
- Data encoding formats

---

## Layer 5 - Session

### Purpose

The Session layer manages communication sessions between applications.

### Responsibilities

- Starting sessions
- Maintaining sessions
- Ending sessions

### Examples

- Authentication sessions
- Remote connections

---

## Layer 4 - Transport

### Purpose

The Transport layer provides end-to-end communication between devices.

It controls how data is delivered.

### Responsibilities

- Reliability
- Flow control
- Error recovery
- Segmentation

### Protocols

- TCP
- UDP

### Examples

TCP:

- Reliable
- Connection-oriented

UDP:

- Faster
- Connectionless

---

## Layer 3 - Network

### Purpose

The Network layer handles addressing and routing.

It decides the best path for data to reach the destination.

### Responsibilities

- Logical addressing
- Packet forwarding
- Routing

### Protocols

- IP
- ICMP

### Devices

- Routers

---

## Layer 2 - Data Link

### Purpose

The Data Link layer handles communication between devices on the same network.

It uses physical addresses.

### Responsibilities

- Frame creation
- MAC addressing
- Error detection

### Protocols

- Ethernet
- ARP

### Devices

- Switches

---

## Layer 1 - Physical

### Purpose

The Physical layer transmits raw bits through physical media.

### Responsibilities

- Electrical signals
- Radio waves
- Cables
- Connectors

### Examples

- Ethernet cable
- Fiber optic
- Wi-Fi signals

---

# Data Encapsulation

When data is sent through a network, each layer adds its own information.

The process:

```
Application
↓
Data
↓
Transport
↓
Segment
↓
Network
↓
Packet
↓
Data Link
↓
Frame
↓
Physical
↓
Bits
```

At the destination, the process is reversed.

This is called **decapsulation**.

---

# OSI Model Table

| Layer | Name | Main Function | Example |
|---|---|---|---|
| 7 | Application | User services | HTTP, DNS |
| 6 | Presentation | Format/encryption | TLS |
| 5 | Session | Connections | Sessions |
| 4 | Transport | Delivery | TCP, UDP |
| 3 | Network | Routing | IP |
| 2 | Data Link | MAC communication | Ethernet |
| 1 | Physical | Signals | Cables |

---

# Cybersecurity Importance

The OSI model is important in cybersecurity because attacks can happen at different layers.

Examples:

- Layer 7: Web attacks (SQL Injection, XSS)
- Layer 4: TCP attacks (SYN Flood)
- Layer 3: IP attacks
- Layer 2: MAC spoofing
- Layer 1: Physical access attacks

Understanding the OSI model helps security professionals identify where problems and attacks occur.
