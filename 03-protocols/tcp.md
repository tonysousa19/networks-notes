# TCP (Transmission Control Protocol)

## Definition

TCP (Transmission Control Protocol) is a transport layer protocol responsible for reliable communication between devices.

It ensures that data arrives at the destination correctly, in the correct order, and without missing information.

TCP operates at:

- OSI Layer 4 - Transport
- TCP/IP Transport Layer

---

# Characteristics

## Connection-Oriented

TCP requires a connection to be established before sending data.

It creates a communication session between two devices.

---

## Reliable Delivery

TCP guarantees that data reaches the destination.

It uses:

- Acknowledgments (ACK)
- Retransmission
- Error checking

If data is lost, TCP sends it again.

---

## Ordered Data

TCP keeps packets organized.

Even if packets arrive in a different order, TCP rebuilds them correctly.

---

## Flow Control

TCP controls the amount of data sent.

This prevents a fast sender from overwhelming a slower receiver.

---

# TCP Three-Way Handshake

Before communication starts, TCP establishes a connection.

```
Client                Server

SYN  ------------->

     <------------- SYN-ACK

ACK  ------------->

Connection Established
```

Steps:

1. Client sends SYN
2. Server responds with SYN-ACK
3. Client sends ACK

After this, data transmission begins.

---

# TCP Header Information

TCP headers contain:

- Source port
- Destination port
- Sequence number
- Acknowledgment number
- Flags
- Window size

---

# Common TCP Ports

| Service | Port |
|---|---|
| HTTP | 80 |
| HTTPS | 443 |
| SSH | 22 |
| FTP | 21 |
| SMTP | 25 |
| DNS (TCP) | 53 |

---

# TCP Security Concerns

## SYN Flood Attack

An attacker sends many SYN requests but does not complete the handshake.

This can exhaust server resources.

---

## TCP Hijacking

An attacker takes control of an existing TCP session.

---

## Packet Analysis

Security professionals analyze TCP traffic to identify:

- Suspicious connections
- Open ports
- Unusual communication patterns

---

# Commands

Check TCP connections:

```bash
ss -t
```

Scan TCP ports:

```bash
nmap -sT target_ip
```

---

# Summary

TCP provides reliable, ordered, and controlled communication.

It is widely used when accuracy is more important than speed, such as:

- Websites
- Email
- File transfers
- Remote connections
