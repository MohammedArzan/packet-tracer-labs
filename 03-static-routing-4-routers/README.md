# Static Routing – 4 Router Topology (Packet Tracer)

## Static Route Syntax
ip route <destination-network> <subnet-mask> <next-hop-ip>


## Objective
To understand static routing in a network with four routers by manually
configuring routes between multiple LANs.

## Topology Used
- 4 Routers connected using serial links
- Each router has its own LAN network
- Static routes are configured to enable full connectivity

## What is Static Routing?
Static routing is a routing method where routes are manually added by the
network administrator. Routers do not exchange routing information automatically.

## Verification
- Ping between PCs in different LANs
- Verify routes using:
show ip route


## Files Included
- static-routing-4-routers.pkt
- topology.png
- Router configuration files (R1 to R4)
