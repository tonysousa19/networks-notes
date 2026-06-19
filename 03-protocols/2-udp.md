# UDP (User Datagram Protocol)

## Definition

UDP (User Datagram Protocol) is a transport layer protocol used for fast communication without establishing a connection.

Unlike TCP, UDP does not guarantee delivery, order, or error recovery.

UDP operates at:

- OSI Layer 4 - Transport
- TCP/IP Transport Layer

---

# Characteristics

## Connectionless

UDP sends data without creating a session first.

There is no handshake process.

---

## Faster Communication

Because UDP has fewer controls than TCP, it has lower overhead and can transmit data faster.

---

## No Delivery Guarantee

UDP does not check if data arrived successfully.

Lost packets are not automatically retransmitted.

---

## No Ordering

Packets may arrive:

- Out of order
- Duplicated
- Missing

The application must handle this if needed.

---

# TCP vs UDP

| Feature | TCP | UDP |
|---|---|---|
| Connection | Yes | No |
| Reliability | High | Low |
| Speed | Slower | Faster |
| Ordering | Yes | No |
| Retransmission | Yes | No |

---

# Common UDP Ports

| Service | Port |
|---|---|
| DNS | 53 |
| DHCP | 67/68 |
| TFTP | 69 |
| SNMP | 161 |
| NTP | 123 |

---

# Where UDP Is Used

## DNS

DNS queries are usually sent using UDP because they are small and need quick responses.

---

## Online Games

Games prioritize speed and low latency.

A lost packet is often less important than delay.

---

## Video Streaming

Real-time media uses UDP because waiting for retransmissions causes delays.

---

## VoIP

Voice communication needs fast delivery.

---

# UDP Security Concerns

## UDP Flood

An attacker sends a large amount of UDP traffic to overload a target.

---

## UDP Scanning

Attackers use UDP scans to discover services.

Example:

```bash
nmap -sU target_ip
```

---

# Summary

UDP is designed for speed and efficiency.

It is preferred when:

- Low latency is important
- Some data loss is acceptable
- Real-time communication is needed
