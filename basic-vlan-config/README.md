# VLAN Configuration Lab – Cisco Packet Tracer

## 📌 Project Overview

This lab demonstrates VLAN configuration and Layer 2 network segmentation using Cisco 2950 switches in Packet Tracer.

The goal of this project is to understand:

- How VLANs separate networks at Layer 2
- How broadcast domains are created
- How trunk links carry multiple VLANs between switches
- Why devices in different VLANs cannot communicate without routing

---

## 🖥️ VLAN Structure Implemented

| VLAN ID | Name | Network Address |
|----------|------|----------------|
| 10 | IT | 192.168.10.0/24 |
| 20 | HR | 192.168.20.0/24 |
| 30 | DEV | 192.168.30.0/24 |

Each VLAN represents a separate department and broadcast domain.

---

## 🔧 Switch Configuration

### VLAN Creation

```bash
vlan 10
 name IT

vlan 20
 name HR

vlan 30
 name DEV

Access Port Assignment (Example)
interface fa0/1
 switchport mode access
 switchport access vlan 20

interface fa0/3
 switchport mode access
 switchport access vlan 10

interface fa0/5
 switchport mode access
 switchport access vlan 30

Trunk Configuration (Between Switches)
interface fa0/7
 switchport mode trunk

🔎 Verification Commands Used

To verify VLAN configuration:
show vlan brief

To verify trunk link:
show interfaces trunk
