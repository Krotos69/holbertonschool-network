# Network Basics

## Overview

Computer networks allow devices to communicate, share resources, and exchange data. Understanding networking fundamentals is essential for system administrators, developers, and cybersecurity professionals.

This guide covers the following core concepts:

- The OSI Model and its layers
- LAN (Local Area Network)
- WAN (Wide Area Network)
- The Internet and IP addressing
- TCP and UDP protocols
- Common networking ports
- Basic connectivity testing

---

# OSI Model

## What is the OSI Model?

The **OSI (Open Systems Interconnection) Model** is a conceptual framework that standardizes how computers communicate over a network. It divides the communication process into seven layers, each responsible for a specific task.

### How many layers does it have?

The OSI Model contains **7 layers**.

### How is it organized?

| Layer | Name | Purpose |
|---------|---------|---------|
| 7 | Application | Provides network services to applications |
| 6 | Presentation | Handles data formatting, encryption, and compression |
| 5 | Session | Establishes and manages communication sessions |
| 4 | Transport | Provides end-to-end communication and reliability |
| 3 | Network | Handles routing and IP addressing |
| 2 | Data Link | Manages physical addressing (MAC) and frame transmission |
| 1 | Physical | Transmits bits through physical media |

### OSI Layers Mnemonic

**Please Do Not Throw Sausage Pizza Away**

- Physical
- Data Link
- Network
- Transport
- Session
- Presentation
- Application

---

# LAN (Local Area Network)

## What is a LAN?

A **Local Area Network (LAN)** connects devices within a limited geographic area.

### Typical Usage

- Home networks
- Office networks
- School networks
- Small business environments

### Typical Geographic Size

- Single room
- Building
- Campus

LANs usually cover a relatively small area and offer high-speed connectivity.

---

# WAN (Wide Area Network)

## What is a WAN?

A **Wide Area Network (WAN)** connects multiple LANs across larger geographic distances.

### Typical Usage

- Connecting company branches
- Internet Service Provider (ISP) infrastructure
- Global business networks

### Typical Geographic Size

- City-wide
- Country-wide
- Continental
- Worldwide

The Internet is the largest example of a WAN.

---

# The Internet

## What is the Internet?

The **Internet** is a global network of interconnected networks that communicate using the TCP/IP protocol suite.

### What is an IP Address?

An **IP (Internet Protocol) address** is a unique identifier assigned to a device connected to a network.

Examples:

- IPv4: `192.168.1.1`
- IPv6: `2001:db8::1`

### What are the 2 Types of IP Address?

1. **IPv4**
   - 32-bit addressing
   - Example: `192.168.1.1`

2. **IPv6**
   - 128-bit addressing
   - Example: `2001:db8::1`

### What is localhost?

**localhost** is a special hostname that refers to the current machine.

Common addresses:

- IPv4: `127.0.0.1`
- IPv6: `::1`

### What is a Subnet?

A **subnet** is a smaller network created by dividing a larger network into logical segments.

Example:

- Network: `192.168.1.0/24`
- Host range: `192.168.1.1 - 192.168.1.254`

### Why Was IPv6 Created?

IPv6 was created because:

- IPv4 addresses were becoming exhausted.
- The number of Internet-connected devices continued to grow.
- IPv6 provides a much larger address space.
- IPv6 improves routing efficiency and scalability.

---

# TCP and UDP

## What Are the Two Main Transport Layer Protocols?

The two primary protocols that operate at the **Transport Layer (Layer 4)** are:

- TCP (Transmission Control Protocol)
- UDP (User Datagram Protocol)

### What Is the Main Difference Between TCP and UDP?

| TCP | UDP |
|------|------|
| Connection-oriented | Connectionless |
| Reliable delivery | Best-effort delivery |
| Error checking and retransmission | No retransmission |
| Slower | Faster |
| Used for web browsing and SSH | Used for streaming and gaming |

### What Is a Port?

A **port** is a logical communication endpoint that identifies a specific service or application running on a device.

An IP address identifies the device, while a port identifies the service.

### What Are the SSH, HTTP, and HTTPS Port Numbers?

| Service | Port |
|-----------|------|
| SSH | 22 |
| HTTP | 80 |
| HTTPS | 443 |

### What Tool Is Commonly Used to Check Connectivity?

The **ping** command is commonly used to check whether a host can be reached over a network.

Example:

```bash
ping google.com
```

Ping uses the **ICMP (Internet Control Message Protocol)** to test connectivity.

---

