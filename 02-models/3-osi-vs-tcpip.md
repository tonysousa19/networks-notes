# OSI vs TCP/IP Model

## Overview

The OSI and TCP/IP models are frameworks used to understand network communication.

The OSI model is a theoretical reference model with seven layers.

The TCP/IP model is a practical model used by the Internet with four layers.

---

# Main Differences

| Feature | OSI Model | TCP/IP Model |
|---|---|---|
| Layers | 7 layers | 4 layers |
| Purpose | Reference model | Practical networking model |
| Created by | ISO | Department of Defense (DoD) |
| Usage | Learning and troubleshooting | Real-world networks |
| Protocol dependency | Protocol independent | Based on TCP/IP protocols |

---

# Layer Comparison

```
OSI Model                 TCP/IP Model

Application  ┐
Presentation │
Session      ┘  →  Application

Transport    →  Transport

Network      →  Internet

Data Link    ┐
Physical     ┘  →  Network Access
```

---

# Layer Mapping

## OSI Layers 7, 6, 5

Become:

## TCP/IP Application Layer

Includes:

- User services
- Data formatting
- Encryption
- Sessions

Examples:

- HTTP
- DNS
- SSH

---

## OSI Layer 4

Becomes:

## TCP/IP Transport Layer

Handles:

- End-to-end communication
- Reliability
- Segmentation

Examples:

- TCP
- UDP

---

## OSI Layer 3

Becomes:

## TCP/IP Internet Layer

Handles:

- IP addressing
- Routing

Examples:

- IP
- ICMP

---

## OSI Layers 2 and 1

Become:

## TCP/IP Network Access Layer

Handles:

- Frames
- MAC addresses
- Physical transmission

Examples:

- Ethernet
- Wi-Fi

---

# Which One Should I Use?

## OSI Model

Useful for:

- Learning networking concepts
- Troubleshooting
- Understanding where problems happen

Example:

"The problem is at Layer 3 because the router cannot route packets."

---

## TCP/IP Model

Useful for:

- Real networks
- Configuring systems
- Cybersecurity analysis

Example:

"An attacker is abusing TCP communication."

---

# Cybersecurity Importance

Both models are important for cybersecurity.

Security analysts use them to:

- Analyze network traffic
- Understand attacks
- Configure firewalls
- Troubleshoot connectivity issues
- Identify where vulnerabilities exist

The OSI model provides a detailed view, while TCP/IP represents how networks actually operate.
