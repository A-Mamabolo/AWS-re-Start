# Networking Fundamentals – Study README

## Overview
This section covers the fundamental networking concepts required for cloud computing and AWS. Understanding networking is essential because AWS services such as EC2, VPC, Load Balancers, RDS, and Route 53 all rely on networking principles.
---

# Learning Objectives
* Explain how clients and servers communicate.
* Understand the purpose of network devices.
* Differentiate between LAN and WAN.
* Explain the role of IP addresses.
* Understand TCP and UDP protocols.
* Describe how data travels through a network.
* Understand AWS Virtual Private Cloud (VPC) fundamentals.
* Troubleshoot basic networking issues.
---

# Core Concepts

## Client and Server

### Client
A client is a device or application that requests services or data.
Examples:
* Laptop
* Smartphone
* Web browser

### Server
A server responds to requests from clients and provides services or data.
Examples:
* Web Server
* Database Server
* File Server
* Mail Server

### Client-Server Model
```text
Client → Request → Server
Client ← Response ← Server
```
Example:
A web browser requests a webpage from Amazon's servers, and the server returns the webpage.
---

# Network Interface Card (NIC)
A Network Interface Card (NIC) connects a device to a network.

Key facts:
* Also called a Network Adapter.
* Can be wired or wireless.
* Has a unique MAC Address.
* Operates at OSI Layer 2.

### MAC Address
A MAC Address is a unique hardware identifier assigned by the manufacturer.

Example:
00:1A:2B:3C:4D:5E

---

# Network Cables

## Fiber-Optic
* Uses light instead of electricity.
* Fastest cable type.
* Suitable for long distances.

## Coaxial
* Commonly used by internet service providers.
* Often used for cable internet and television.

## Twisted-Pair (Ethernet)
* Most common network cable.
* Used in homes and offices.
* Available as UTP and STP.

---

# Switch
A switch connects devices within the same network.

Functions:
* Uses MAC addresses.
* Sends data only to the intended device.
* Operates at Layer 2.

Benefits:
* Reduces unnecessary traffic.
* Improves network efficiency.
---

# Router
A router connects different networks together.

Functions:
* Uses IP addresses.
* Routes traffic between networks.
* Filters traffic.
* Operates at Layers 2 and 3.

Example:
A router connects your home network to the internet.
---

# Modem
A modem connects a network to an Internet Service Provider (ISP).

Typical connection:
```text
Internet
   ↓
 Modem
   ↓
 Router
   ↓
 Devices
```
---

# LAN and WAN

## LAN (Local Area Network)
A network covering a small area.

Examples:
* Home network
* School network
* Office network

## WAN (Wide Area Network)
A network covering large geographical areas.

Examples:
* The Internet
* Corporate branch networks
---

# Network Protocols
A protocol is a set of rules that define how data is transmitted across a network.
---

# Internet Protocol (IP)
IP is responsible for:
* Addressing devices.
* Routing packets.
* Delivering data between networks.

IP does not guarantee delivery.
---

# Connection-Oriented Protocol
Characteristics:
* Establishes a connection before communication.
* Waits for acknowledgment.
* Creates a session.
* Reliable.

Real-world example:
Phone call.
---

# Connectionless Protocol
Characteristics:
* No connection setup required.
* No session established.
* Fast transmission.
* No delivery guarantee.

Real-world example:
Sending a letter through the mail.
---

# Transmission Control Protocol (TCP)
TCP is:
* Connection-oriented.
* Reliable.
* Ordered.
* Error-checked.

Uses:
* Websites (HTTP/HTTPS)
* File transfers
* Banking systems
* Email

### TCP Three-Way Handshake
```text
1. SYN
2. SYN/ACK
3. ACK
```

Purpose:
Establishes a reliable connection before data transmission.

### TCP Connection Closing
```text
1. FIN
2. FIN/ACK
3. ACK
```

### Common TCP Flags
| Flag | Purpose             |
| ---- | ------------------- |
| SYN  | Start connection    |
| ACK  | Acknowledge receipt |
| FIN  | End connection      |
| RST  | Reset connection    |
---

# User Datagram Protocol (UDP)

UDP is:
* Connectionless.
* Fast.
* Lightweight.
* Unreliable.

Uses:
* Video streaming
* Online gaming
* Voice calls
* Live broadcasts

UDP does not:
* Confirm delivery.
* Guarantee packet order.
* Retransmit lost packets.
---

# TCP vs UDP
| Feature             | TCP    | UDP    |
| ------------------- | ------ | ------ |
| Connection-Oriented | Yes    | No     |
| Reliable            | Yes    | No     |
| Guarantees Delivery | Yes    | No     |
| Guarantees Order    | Yes    | No     |
| Handshake           | Yes    | No     |
| Speed               | Slower | Faster |
| Overhead            | Higher | Lower  |

Memory Tip:
TCP = Reliability
UDP = Speed
---

# AWS Virtual Private Cloud (VPC)
A VPC is a private virtual network in AWS.

Benefits:
* Isolated environment.
* Custom IP ranges.
* Public and private subnets.
* Security controls.
* Scalability.

Key components:
* VPC
* Subnets
* Route Tables
* Internet Gateway
* Security Groups
---

# Most Important Networking Labs

### Priority 1
1. Build Your VPC and Launch a Web Server (267)
2. Create Subnets in a VPC (263)
3. Networking Resources for a VPC (264)

### Priority 2
4. Troubleshooting a Network Issue (266)
5. Internet Protocol Troubleshooting Commands (265)

### Priority 3
6. Public and Private IP Addresses (261)
7. Static and Dynamic IP Addresses (262)
---

