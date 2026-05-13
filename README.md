# RTS of Protocol Layering

## Introduction
Protocol layering is a networking architecture that divides communication functions into different layers. Each layer performs specific tasks and communicates with adjacent layers to ensure efficient data transmission.

The most common protocol layering models are:

- OSI Model
- TCP/IP Model

---

# Protocol Layering Architecture

<img width="1536" height="1024" alt="ChatGPT Image May 13, 2026, 06_15_55 PM" src="https://github.com/user-attachments/assets/41af7ea2-f401-4efb-9300-8161fa1aa1db" />


---

# What is Protocol Layering?

Protocol layering is the process of organizing network communication into multiple layers where each layer handles a particular function.

### Advantages
- Simplifies communication
- Easier troubleshooting
- Modular design
- Standardization
- Better interoperability

### Disadvantages
- Increased overhead
- Processing delay
- Complex implementation

---

# OSI Model

The OSI (Open Systems Interconnection) model contains 7 layers.

![OSI Model](https://upload.wikimedia.org/wikipedia/commons/8/8d/OSI_Model_v1.svg)

| Layer Number | Layer Name | Main Function |
|---|---|---|
| 7 | Application | User services |
| 6 | Presentation | Encryption & translation |
| 5 | Session | Session management |
| 4 | Transport | Reliable delivery |
| 3 | Network | Routing |
| 2 | Data Link | Framing & MAC |
| 1 | Physical | Bit transmission |

---

# Physical Layer

### Functions
- Bit transmission
- Signal conversion
- Data transmission through media

### Devices
- Hub
- Repeater
- Cables

---

# Data Link Layer

### Functions
- Framing
- Error detection
- MAC addressing

### Devices
- Switch
- Bridge

---

# Network Layer

### Functions
- Routing
- Logical addressing
- Packet forwarding

### Protocols
- IP
- ICMP
- ARP

---

# Transport Layer

### Functions
- Reliable communication
- Error recovery
- Flow control

### Protocols
- TCP
- UDP

---

# Session Layer

### Functions
- Session establishment
- Synchronization
- Session maintenance

---

# Presentation Layer

### Functions
- Encryption
- Compression
- Data formatting

---

# Application Layer

### Functions
- Web browsing
- Email
- File transfer

### Protocols
- HTTP
- FTP
- SMTP
- DNS

---

# TCP/IP Model

The TCP/IP model is widely used in real-world Internet communication.

<img width="1536" height="1024" alt="ChatGPT Image May 13, 2026, 06_23_02 PM" src="https://github.com/user-attachments/assets/7df007e1-94ee-49d6-8fec-9f9f7de611b1" />


| TCP/IP Layer | Corresponding OSI Layer |
|---|---|
| Application | Application + Presentation + Session |
| Transport | Transport |
| Internet | Network |
| Network Access | Data Link + Physical |

---

# Encapsulation and Decapsulation

Encapsulation is the process of adding headers at each layer before transmission.

Decapsulation is the process of removing headers at the receiver side.

<img width="1536" height="1024" alt="ChatGPT Image May 13, 2026, 06_27_58 PM" src="https://github.com/user-attachments/assets/c58fc536-8944-4ee7-8ef1-bea0a01ee3b6" />


| Layer | Data Unit |
|---|---|
| Application | Data |
| Transport | Segment |
| Network | Packet |
| Data Link | Frame |
| Physical | Bits |

---

# Communication Process

## Sender Side
1. User creates data
2. Application layer processes data
3. Transport layer segments data
4. Network layer adds IP address
5. Data link layer creates frames
6. Physical layer transmits bits

## Receiver Side
1. Physical layer receives bits
2. Data link layer checks frames
3. Network layer verifies IP
4. Transport layer reassembles data
5. Application layer delivers data

---

# OSI vs TCP/IP Comparison

<img width="1536" height="1024" alt="ChatGPT Image May 13, 2026, 06_30_13 PM" src="https://github.com/user-attachments/assets/4ed64454-04b9-498d-9eae-794be812f0e9" />


| Feature | OSI Model | TCP/IP Model |
|---|---|---|
| Layers | 7 | 4 |
| Developed By | ISO | DARPA |
| Usage | Reference model | Practical implementation |
| Protocol Dependency | Independent | Dependent |

---

# Real-Time Applications

Protocol layering is used in:

- Internet communication
- Online gaming
- Video conferencing
- Cloud computing
- IoT systems
- Email systems
- Mobile communication

---

# Conclusion

Protocol layering is one of the fundamental concepts in computer networking. It divides communication tasks into multiple layers and enables reliable and scalable communication between devices.

The OSI and TCP/IP models are widely used to understand and implement modern networking systems.

---

# Viva Questions

## 1. What is protocol layering?
Protocol layering is the division of communication tasks into different layers.

## 2. What is encapsulation?
Adding headers at each layer during transmission.

## 3. What is decapsulation?
Removing headers at each layer during reception.

## 4. Which model is used practically?
TCP/IP model.

## 5. Which layer performs routing?
Network layer.

## 6. Which protocols work in the transport layer?
TCP and UDP.

## 7. Which layer uses IP addressing?
Network layer.

## 8. What are the advantages of protocol layering?
Standardization, modularity, and easier troubleshooting.

---

# References

1. Andrew S. Tanenbaum – Computer Networks
2. Behrouz A. Forouzan – Data Communications and Networking
3. Cisco Networking Documentation
4. RFC Internet Standards

---

# Author

**Aravinth N**  
B.E Electronics and Communication Engineering  
Saveetha Engineering College
