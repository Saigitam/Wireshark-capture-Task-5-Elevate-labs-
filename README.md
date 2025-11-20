# ELEVATE LABS – Cybersecurity Internship  
## Task 5: Capture and Analyze Network Traffic Using Wireshark  
**Name:** Kothamasu Sai Prasad  

This task demonstrates how I captured and analyzed **live network traffic** using **Wireshark** on my Windows system.  
The goal was to record packets, filter different protocols, identify traffic types, and export the capture as a `.pcap` file.

---

## 🔧 Tools Used
- **Wireshark (Free & Open Source)**
- **Windows 10/11**
- Active Network Adapter (Wi-Fi)

---

## 🟦 Step-by-Step Process

### **1. Installing Wireshark**
- Downloaded the latest version of Wireshark.
- Installed along with **Npcap**, which is required for capturing packets.
- Verified that my network interface appeared in the capture list.

---

### **2. Selecting Capture Interface**
- Opened Wireshark.  
- Chose the active network interface (Wi-Fi).  
- Clicked **Start Capture** (Shark fin icon).

---

### **3. Generating Live Traffic**
To generate network packets:
- Opened browser and visited websites (e.g., google.com).
- Also tested using:
ping 8.8.8.8
- Continued activity for about **1 minute**.

---

### **4. Stopping the Capture**
- Clicked the **red square** (Stop button) in Wireshark.
- This froze the captured traffic for analysis.

---

## 📊 Protocols Identified & Filters Applied

### I applied the following filters in Wireshark:
- **DNS** → `dns`  
- **HTTP** → `http`  
- **TCP** → `tcp`  
- **ICMP (Ping)** → `icmp`  
- **ARP** → `arp` *(optional)*  

---

## 🛑 Protocol Analysis Summary

### **1. DNS (Domain Name System)**
**Purpose:** Resolves domain names into IP addresses.  
**Observation:**  
- Observed queries for domains I visited.  
- Example: Request for `google.com`.  
- Indicators: Standard DNS query & response messages.  

---

### **2. TCP (Transmission Control Protocol)**
**Purpose:** Reliable transport protocol used by most applications.  
**Observation:**  
- Identified the **3-way handshake**:
- SYN  
- SYN-ACK  
- ACK  
- Observed multiple TCP streams for browser connections.

---

### **3. HTTP (Web Traffic)**
**Purpose:** Protocol used for loading web pages.  
**Observation:**  
- Saw browser sending `GET` requests to websites.  
- Response headers from servers included status codes (e.g., 200 OK).  

---

### **4. ICMP (Ping Traffic)**
**Purpose:** Used for diagnostics (ping command).  
**Observation:**  
- Captured ICMP echo request & echo reply packets.  

---

## 💾 Exporting the Capture
- Saved the captured traffic file as:
task5_network_capture.pcap
- This file can be opened in Wireshark for detailed review.

---

## 📝 Summary of Findings
During the capture, I successfully identified **four major protocols**:

| Protocol | Summary |
|----------|---------|
| **DNS** | Domain name resolution for visited websites |
| **TCP** | Handshake, retransmissions, and data packets |
| **HTTP** | Web browsing traffic including GET requests |
| **ICMP** | Ping traffic generated manually |

These observations helped me understand how different network layers operate when performing everyday internet activities.

---

## 🎉 Conclusion
This task improved my hands-on skills in:
- Capturing real-time network traffic  
- Using Wireshark filters  
- Identifying different protocols  
- Exporting `.pcap` files for documentation  

Wireshark is an essential tool for cybersecurity analysis, and this exercise helped build foundation-level packet inspection and protocol awareness.

---
