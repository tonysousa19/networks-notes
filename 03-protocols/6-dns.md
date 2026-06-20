# DNS (Domain Name System)

## Definition

DNS (Domain Name System) is a protocol that translates domain names into IP addresses.

It works like the Internet's phone book.

DNS operates at:

- OSI Layer 7 - Application
- TCP/IP Application Layer

---

# Why DNS Exists

Humans use names:

```
google.com
```

Computers communicate using IP addresses:

```
142.250.72.14
```

DNS connects the two.

---

# DNS Process

Example:

User types:

```
www.example.com
```

The process:

1. Computer checks local cache
2. Query is sent to DNS server
3. DNS server finds the IP address
4. Response returns the IP
5. Browser connects to the server

---

# DNS Hierarchy

DNS is organized in levels.

```
.
|
.com
|
example.com
|
www.example.com
```

---

# DNS Records

## A Record

Maps a domain to an IPv4 address.

Example:

```
example.com → 192.168.1.10
```

---

## AAAA Record

Maps a domain to an IPv6 address.

---

## MX Record

Defines mail servers.

Used for email delivery.

---

## CNAME Record

Creates an alias.

Example:

```
www.example.com
```

points to:

```
example.com
```

---

# DNS Ports

DNS uses:

```
UDP 53
```

For normal queries.

```
TCP 53
```

For larger responses and zone transfers.

---

# DNS Security Issues

## DNS Spoofing

Attackers send fake DNS responses.

Users are redirected to malicious sites.

---

## DNS Cache Poisoning

Fake information is stored in DNS caches.

---

## DNS Tunneling

Attackers hide data inside DNS queries.

---

# Protection

Methods:

- DNSSEC
- Secure DNS servers
- Monitoring

---

# Summary

DNS translates domain names into IP addresses.

Without DNS, users would need to remember IP addresses for every website.
