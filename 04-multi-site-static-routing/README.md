# Multi-Site Static Routing Lab – Cisco Packet Tracer

## 📌 Project Overview

This project demonstrates a multi-site WAN network using static routing in Cisco Packet Tracer.

The topology consists of 4 routers connecting three branch offices (Bengaluru, Mumbai, Delhi) through a central MAIN router using serial WAN links.

Each branch office has its own LAN network connected via a switch.

The objective of this lab is to understand:

- Static routing configuration
- WAN serial connectivity
- Multi-site network design
- End-to-end communication across different networks

---

## 🏢 Network Topology

### Branch Networks

| Location     | LAN Network        | Gateway IP     |
|-------------|-------------------|---------------|
| Bengaluru   | 10.0.0.0/8         | 10.0.0.1      |
| Mumbai      | 192.16.10.0/24     | 192.16.10.1   |
| Delhi       | 31.1.0.0/16        | 31.1.0.1      |

### WAN Links

| Connection | Network Used |
|------------|-------------|
| Bengaluru ↔ MAIN | 133.12.0.0 |
| MAIN ↔ Delhi     | 155.12.0.0 |
| MAIN ↔ Mumbai    | 7.0.0.0    |

Each WAN link is configured using serial interfaces.

---

## 🧠 Concepts Covered

- Static Route Configuration
- Serial Interface Configuration
- IP Addressing and Subnetting
- Default Gateway Setup
- Routing Table Verification
- End-to-End Connectivity Testing

---

## ⚙️ Basic Static Route Syntax Used
```bash
ip route <destination-network> <subnet-mask> <next-hop-ip>

🔧 Router Configuration Summary
Each router was configured with:
LAN interface IP address
Serial WAN interface IP address
Static routes to reach remote networks
no shutdown on all active interfaces
The MAIN router contains static routes for all branch networks.

```bash
ip route <destination-network> <subnet-mask> <next-hop-ip>
