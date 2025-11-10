# 🌐 Classless Static Routing with DHCP and TFTP Server

## 🧠 Project Overview
This project demonstrates how to configure **Classless Static Routing**, **DHCP**, and **TFTP services** in a multi-router network using **Cisco Packet Tracer**.  
It simulates a small enterprise network setup where routers handle data routing between different subnets, DHCP dynamically assigns IP addresses, and TFTP manages configuration backups.

---

## ⚙️ Network Components

| Device Type | Role |
|--------------|------|
| **Router 1 & Router 2** | Configured with classless static routes for inter-network communication |
| **Switches** | Connect LAN devices within each subnet |
| **DHCP Server** | Provides automatic IP address assignment to clients |
| **TFTP Server** | Stores and retrieves router configuration backups |
| **PCs/Clients** | Receive IPs via DHCP and test network connectivity |

---

## 🧩 Key Configurations

### 🔸 1. Classless Static Routing
Each router is configured with static routes that define how to reach other networks using next-hop IPs.  
Unlike classful routing, **CIDR (Classless Inter-Domain Routing)** allows using variable-length subnet masks for efficient IP utilization.

Example:
```bash
Router(config)# ip route 192.168.20.0 255.255.255.0 10.0.0.2
Router(config)# ip route 192.168.30.0 255.255.255.0 10.0.0.6
