# ARP (Address Resolution Protocol)

## Definition

ARP (Address Resolution Protocol) is a network protocol used to find the MAC address associated with an IP address inside a local network.

It operates between:

- OSI Layer 2 - Data Link
- OSI Layer 3 - Network

ARP allows devices to communicate on the same local network.

---

# Why ARP Exists

Devices communicate using:

- IP addresses (logical addresses)
- MAC addresses (physical addresses)

When a computer knows the destination IP but does not know the MAC address, it uses ARP.

Example:

Computer A wants to communicate with:

```
192.168.1.20
```

But it needs the MAC address.

It sends an ARP request asking:

"Who has 192.168.1.20?"

The device responds with its MAC address.

---

# ARP Process

## ARP Request

Broadcast message:

```
Who has 192.168.1.20?
Tell 192.168.1.10
```

Every device receives it.

---

## ARP Reply

The correct device answers:

```
192.168.1.20 is at AA:BB:CC:DD:EE:FF
```

The sender stores this information.

---

# ARP Table

Devices keep ARP mappings.

View ARP table:

```bash
arp -a
```

or:

```bash
ip neigh
```

Example:

```
192.168.1.20
MAC: AA:BB:CC:DD:EE:FF
```

---

# ARP Security Issues

## ARP Spoofing

An attacker sends fake ARP messages.

Example:

Attacker says:

```
192.168.1.1 is my MAC address
```

Traffic is redirected to the attacker.

---

## Man-in-the-Middle Attack

ARP spoofing can allow attackers to intercept communication.

---

# Protection

Methods:

- Static ARP entries
- Network segmentation
- Dynamic ARP Inspection
- Encryption (HTTPS, VPN)

---

# Summary

ARP connects IP addresses to MAC addresses on local networks.

It is essential for communication inside LANs but can be abused by attackers.
