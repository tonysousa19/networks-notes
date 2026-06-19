# TCP/IP Model

## Definition

The TCP/IP model is the networking model used by the Internet and modern computer networks.

TCP/IP stands for:

- Transmission Control Protocol
- Internet Protocol

Unlike the OSI model, which is mainly a reference model, TCP/IP is a practical model based on real-world protocols.

It explains how data is transmitted between devices across a network.

---

# The 4 Layers of the TCP/IP Model

## Layer 4 - Application

### Purpose

The Application layer provides services directly to applications and users.

It combines the functions of the OSI Application, Presentation, and Session layers.

### Responsibilities

- User interaction
- Data formatting
- Application communication

### Protocols

- HTTP
- HTTPS
- DNS
- DHCP
- FTP
- SSH
- SMTP

### Examples

- Web browsing
- Email
- File transfers

---

## Layer 3 - Transport

### Purpose

The Transport layer manages communication between devices.

It controls how data is delivered.

### Responsibilities

- Reliability
- Flow control
- Error handling
- Data segmentation

### Protocols

### TCP (Transmission Control Protocol)

- Connection-oriented
- Reliable delivery
- Uses acknowledgments

Examples:

- Web pages
- Email
- File transfers

### UDP (User Datagram Protocol)

- Connectionless
- Faster
- No delivery guarantee

Examples:

- Online games
- Video streaming
- DNS queries

---

## Layer 2 - Internet

### Purpose

The Internet layer handles addressing and routing packets between networks.

It determines where data should go.

### Responsibilities

- Logical addressing
- Routing
- Packet delivery

### Protocols

- IP
- ICMP
- ARP

### Devices

- Routers

### Example

Sending data from a computer in Brazil to a server in another country.

---

## Layer 1 - Network Access

### Purpose

The Network Access layer handles communication over the physical network.

It combines the OSI Physical and Data Link layers.

### Responsibilities

- Physical transmission
- MAC addressing
- Frames
- Hardware communication

### Technologies

- Ethernet
- Wi-Fi
- Fiber optic

### Devices

- Switches
- Network adapters

---

# Data Encapsulation

When data is transmitted, each layer adds information.

```
Application
↓
Data

Transport
↓
Segment

Internet
↓
Packet

Network Access
↓
Frame
```

At the destination, the process is reversed.

This is called decapsulation.

---

# TCP/IP Model Table

| Layer | Name | Function | Examples |
|---|---|---|---|
| 4 | Application | User services | HTTP, DNS, SSH |
| 3 | Transport | Communication control | TCP, UDP |
| 2 | Internet | Routing | IP |
| 1 | Network Access | Physical communication | Ethernet, Wi-Fi |

---

# Cybersecurity Importance

The TCP/IP model is important in cybersecurity because almost all network attacks happen through TCP/IP communication.

Examples:

- Application Layer: Web attacks
- Transport Layer: TCP attacks
- Internet Layer: IP spoofing
- Network Access Layer: MAC attacks

Understanding TCP/IP helps security professionals analyze traffic, configure defenses, and investigate incidents.
