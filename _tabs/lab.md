---
layout: page
title: Lab
icon: fas fa-flask
order: 5
---

#  Lab Challenges

This section showcases selected networking lab challenges I have completed during my training and personal learning. Each lab demonstrates practical application of networking concepts, troubleshooting skills, and understanding of protocols.

---

# 🔹 Lab Challenge 1  
## Packet Tracer – Build a Switch and Router Network

### 📌 Problem Statement

The objective of this lab was to design and configure a basic network topology using:

- 1 Router (Cisco 4221)
- 1 Switch (Cisco 2960)
- 2 PCs

The goal was to:

- Configure IPv4 and IPv6 addressing
- Enable routing between two subnets
- Verify connectivity
- Use IOS commands to analyze interfaces and routing tables

---

###  Approach

1. **Cabled the topology** using Packet Tracer.
2. Initialized the router and switch to default configuration.
3. Assigned static IP addresses to PC-A and PC-B.
4. Configured router:
   - Hostname
   - Password encryption
   - Console & VTY access
   - IPv4 and IPv6 addressing
   - Enabled `ipv6 unicast-routing`
   - Activated interfaces using `no shutdown`
5. Configured switch:
   - Hostname
   - VLAN 1 IP address
   - Default gateway
6. Verified connectivity using:
   - `ping`
   - `show ip route`
   - `show ipv6 route`
   - `show ip interface brief`

---

###  Tools Used

- Cisco Packet Tracer  
- Cisco IOS CLI  
- IPv4 & IPv6 configuration  
- Routing table analysis  
- Interface troubleshooting commands  

---

###  Key Observations

- Initial pings failed because router interfaces were not yet configured.
- After enabling routing and assigning correct IP addresses, communication between subnets succeeded.
- The routing table showed:
  - `C` for directly connected networks
  - `L` for local interfaces
- Verified operational status:  
  `GigabitEthernet0/0/1 is up, line protocol is up`

---

###  Key Lessons Learned

- Importance of correct default gateway configuration
- How routers enable Layer 3 communication between subnets
- Practical use of `show` commands for troubleshooting
- How incorrect IP configuration can cause conflicts
- The role of `no shutdown` in activating interfaces

This lab strengthened my foundational understanding of Cisco routing, switching, and network troubleshooting.

---

#  Lab Challenge 2  
## Packet Tracer – Investigate the TCP/IP and OSI Models in Action

###  Problem Statement

This lab focused on analyzing real-time network communication using Packet Tracer Simulation Mode.

Objectives included:

- Examining HTTP web traffic
- Understanding TCP/IP protocol suite
- Observing OSI model encapsulation and decapsulation
- Analyzing DNS, TCP, and HTTP processes

---

###  Approach

1. Switched Packet Tracer from Realtime to **Simulation Mode**.
2. Filtered events to observe HTTP traffic.
3. Generated web traffic by accessing `www.osi.local`.
4. Examined:
   - OSI Model tab
   - In Layers & Out Layers
   - PDU Details
5. Observed DNS queries and TCP session establishment.
6. Tracked encapsulation from:
   - Layer 7 (Application – HTTP)
   - Layer 4 (TCP)
   - Layer 3 (IP)
   - Layer 2 (MAC addresses)
   - Layer 1 (Physical transmission)

---

###  Tools Used

- Cisco Packet Tracer Simulation Mode  
- HTTP, DNS, TCP protocol analysis  
- OSI Model inspection  
- PDU analysis  

---

### 🔎 Key Findings

- HTTP traffic used **Port 80**
- DNS queries used **Port 53**
- TCP established connection state before data transfer
- Source and destination ports reversed between request and response
- Encapsulation process clearly demonstrated TCP/IP model mapping to OSI layers

Example observations:

- Layer 7: HTTP request to server  
- Layer 4: Destination Port = 80  
- Layer 3: Destination IP = 192.168.1.1  
- Layer 2: Source and Destination MAC addresses  

---

###  Key Lessons Learned

- Clear understanding of how TCP establishes and closes connections
- Relationship between OSI model and TCP/IP model
- Importance of port numbers in service communication
- Visualization of encapsulation and decapsulation
- How DNS resolves domain names before HTTP communication begins

This lab provided practical insight into how real-world client-server communication works at different protocol layers.

---

#  Overall Learning Impact

These lab challenges strengthened my:

- Network configuration skills  
- Troubleshooting ability  
- Understanding of routing and switching  
- Knowledge of TCP/IP and OSI models  
- Ability to analyze live protocol communication  

They demonstrate both practical configuration skills and deep protocol-level understanding.

---
