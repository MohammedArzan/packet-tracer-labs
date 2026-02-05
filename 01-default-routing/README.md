# Default Routing – Packet Tracer Lab

## 📌 Objective
To understand how default routing works between two routers using Cisco Packet Tracer.

## 🧠 What is Default Routing?
Default routing is used when a router does not have a specific route
for a destination network. The router forwards traffic to a predefined
next-hop router.

## 🗺️ Network Topology
- Two routers (R1 and R2)
- Each router connected to its own LAN
- Routers connected using a point-to-point network (10.0.0.0/8)

## 🌐 IP Addressing
### R1
- LAN: 192.168.1.1/24
- WAN: 10.0.0.1/8

### R2
- LAN: 192.168.2.1/24
- WAN: 10.0.0.2/8

## ⚙️ Routing Configuration
Default route configured on both routers:

