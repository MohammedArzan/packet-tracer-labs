# Static Routing – Packet Tracer Lab

This lab demonstrates static routing using Cisco Packet Tracer.

## Static Route Syntax
**ip route <destination-network> <subnet-mask> <next-hop-ip>
ex: 10.0.0.0 255.0.0.0 193.168.1.2**

## Objective
To understand static routing by manually configuring routes between multiple routers.

## Topology Used
- 3 Routers connected using serial links
- Each router has its own LAN network
- Static routes are added to reach remote networks

LAN Networks:
- 10.0.0.0/24
- 130.0.0.0/24
- 192.168.1.0/24

## What is Static Routing?
Static routing is when routes are manually added by the network administrator.
Routers do not learn routes automatically.

## Verification
- Ping between PCs in different networks
- Check routing table using:
