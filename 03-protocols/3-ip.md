# IP (Internet Protocol)

## Definition

IP (Internet Protocol) is a network layer protocol responsible for addressing and routing data between devices.

It allows packets to travel across different networks until they reach their destination.

IP operates at:

- OSI Layer 3 - Network
- TCP/IP Internet Layer

---

# Main Functions

## Addressing

IP assigns addresses to devices.

Example:

```
192.168.1.10
```

Each device on a network needs an IP address to communicate.

---

## Routing

IP determines where packets should go.

Routers examine IP addresses and forward packets toward the destination.

---

## Packet Delivery

IP breaks communication into packets and sends them across networks.

It does not guarantee delivery.

---

# Versions of IP

## IPv4

The most common version.

Uses 32-bit addresses.

Example:

```
192.168.0.1
```

Total addresses:

About 4.3 billion

---

## IPv6

Created to replace IPv4.

Uses 128-bit addresses.

Example:

```
2001:0db8:85a3::8a2e:0370:7334
```

Advantages:

- Huge address space
- Better efficiency
- Built-in security features

---

# IPv4 Address Structure

Example:

```
192.168.1.50
```

It contains:

Network portion:
```
192.168.1
```

Host portion:
```
50
```

The network identifies the network.

The host identifies the device.

---

# Private IP Addresses

Used inside local networks.

Ranges:

```
10.0.0.0/8

172.16.0.0/12

192.168.0.0/16
```

Example:

Home routers use:

```
192.168.1.1
```

---

# Public IP Addresses

Used on the Internet.

They identify networks globally.

Example:

A company's internet connection has a public IP assigned by an ISP.

---

# IP Header Information

Contains:

- Source IP address
- Destination IP address
- TTL (Time To Live)
- Protocol information

---

# Related Protocols

## ICMP

Used for network diagnostics.

Example:

```bash
ping google.com
```

---

## ARP

Maps IP addresses to MAC addresses inside a local network.

---

# IP Security Concerns

## IP Spoofing

An attacker changes the source IP address to hide their identity.

---

## Packet Sniffing

Attackers capture IP traffic to analyze communication.

---

## Routing Attacks

Attackers manipulate routes to redirect traffic.

---

# Useful Commands

Show IP address:

```bash
ip addr
```

Test connectivity:

```bash
ping target
```

Trace route:

```bash
traceroute target
```

---

# Summary

IP is the foundation of modern networking.

It provides:

- Device addressing
- Packet delivery
- Routing between networks

Almost every Internet communication depends on IP.
