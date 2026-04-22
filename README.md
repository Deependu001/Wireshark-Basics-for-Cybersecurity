# 🦈 Wireshark Basics for Cybersecurity
A beginner-friendly guide to understanding network traffic using Wireshark, covering packet analysis, filters, and core networking protocols for cybersecurity.
This document provides a clear and structured introduction to Wireshark, covering its interface, features, filters, and basic usage for beginners in cybersecurity.

---

## 📌 What is Wireshark?

Wireshark is a widely used network protocol analyzer that captures and inspects data packets traveling across a network in real time.

It is commonly used by:
- Network engineers for troubleshooting  
- Security analysts for traffic inspection  
- Ethical hackers for packet analysis  

---

## 🎯 Why Use Wireshark?

Wireshark helps you:
- Monitor live network traffic  
- Analyze packet-level communication  
- Detect anomalies or suspicious behavior  
- Understand how protocols like HTTP, DNS, and TCP work  

---

## ⚙️ Core Features

- Real-time packet capture  
- Deep packet inspection (layer-by-layer analysis)  
- Support for hundreds of protocols  
- Advanced filtering capabilities  
- Cross-platform compatibility (Windows, Linux, macOS)  

---

## 🖥️ Wireshark Interface Breakdown

### 1. Capture Interface
Displays all available network interfaces such as Wi-Fi and Ethernet. You select one to begin capturing packets.

### 2. Packet List Pane
Shows all captured packets in a table format with key details:
- Packet Number  
- Timestamp  
- Source IP  
- Destination IP  
- Protocol  
- Packet Length  
- Summary Info  

### 3. Packet Details Pane
Provides a structured breakdown of the selected packet across different protocol layers (Frame, Ethernet, IP, TCP/UDP, etc.).

### 4. Packet Bytes Pane
Displays raw packet data in hexadecimal and ASCII format, useful for low-level analysis.

---

## ▶️ How to Start Packet Capture

1. Launch Wireshark  
2. Choose a network interface (Wi-Fi/Ethernet)  
3. Click the Start Capture (shark fin icon)  
4. Generate traffic (e.g., open a website or ping a server)  
5. Click Stop Capture (red square icon)  

---

## 🔍 Filtering in Wireshark

Filtering is essential to analyze only relevant traffic.

### 📥 Capture Filters (Before Capture)

```
tcp
port 80
host 192.168.1.1
```

---

### 📤 Display Filters (After Capture)

```
http
dns
ip.addr == 192.168.1.1
tcp.port == 443
icmp
```

---

## 🌐 Common Network Protocols

- HTTP → Unencrypted web traffic  
- HTTPS → Encrypted web communication  
- DNS → Resolves domain names to IP addresses  
- TCP → Reliable, connection-based communication  
- UDP → Fast, connectionless communication  
- ICMP → Used for ping and network diagnostics  

---

## 🧪 Basic Practical Tasks

- Capture traffic while browsing a website  
- Filter and analyze DNS queries (dns)  
- Observe ping traffic using icmp  
- Identify your system’s IP and its communication  

---

## ⚠️ Important Notes

- Run Wireshark with administrator/root privileges  
- Avoid capturing traffic on networks without permission  
- Large captures may consume significant system resources  

---

## 📚 Learning Outcomes

After completing these basics, you will be able to:
- Understand packet structure and flow  
- Identify common protocols in real traffic  
- Apply filters to isolate specific data  
- Perform basic network traffic analysis  

---

## 🚀 Next Steps

- Analyze TCP 3-way handshake  
- Inspect HTTP requests and responses  
- Learn packet analysis for security threats  
- Practice hands-on labs  

---

## 🏁 Conclusion

Wireshark is a foundational tool in cybersecurity. Mastering its basics will give you strong visibility into how networks operate and how data flows between systems.