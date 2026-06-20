# ICMP (Internet Control Message Protocol)

## Definition

ICMP (Internet Control Message Protocol) is a network layer protocol used for diagnostics and error reporting.

It helps devices understand network problems.

ICMP operates at:

- OSI Layer 3 - Network
- TCP/IP Internet Layer

---

# Purpose

ICMP is used to communicate information about:

- Connectivity
- Errors
- Network conditions

It does not transfer user data like TCP or UDP.

---

# Common ICMP Messages

## Echo Request

A device asks:

"Are you reachable?"

---

## Echo Reply

The destination responds:

"Yes, I am reachable."

This is used by the ping command.

---

# Ping

Example:

```bash
ping google.com
```

Ping checks:

- If a host is reachable
- Response time
- Packet loss

Example output:

```
64 bytes from server
time=20ms
```

---

# Traceroute

Traceroute uses ICMP to discover the path packets take.

Example:

```bash
traceroute google.com
```

It shows:

- Routers on the path
- Network delays

---

# ICMP Error Messages

Examples:

## Destination Unreachable

The destination cannot be reached.

---

## Time Exceeded

Packet exceeded its TTL.

---

# ICMP Security Issues

## ICMP Flood

Attacker sends huge amounts of ICMP traffic.

Can cause denial of service.

---

## ICMP Tunneling

Attackers can hide data inside ICMP packets.

---

# Protection

Methods:

- Firewall rules
- Rate limiting
- Monitoring traffic

---

# Summary

ICMP helps troubleshoot networks and report errors.

Tools like ping and traceroute depend on ICMP.
