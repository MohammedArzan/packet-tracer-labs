🛰️ OSPF Routing – Multi Router Topology (Packet Tracer Lab)
📘 Project Overview

This lab demonstrates the configuration and operation of OSPF (Open Shortest Path First) dynamic routing protocol in a multi-router environment.

The objective of this project is to help learners understand:

How OSPF works

How routers form OSPF neighbor relationships

How networks are advertised using wildcard masks

How Area 0 (Backbone Area) functions

How routing tables are dynamically built

This lab is designed for CCNA students and networking beginners.

🏗️ Topology Design

The topology consists of:

4 Routers (R1, R2, R3, R4)

Multiple LAN networks

Serial WAN links connecting routers

All routers configured in Area 0

🌐 Network Overview
LAN Networks

R1 → 50.1.0.0/16

R3 → 153.1.0.0/16

R4 → 192.168.1.0/24

R4 → 192.168.2.0/24

WAN Networks

R1 ↔ R2 → 10.0.0.0

R2 ↔ R3 → 129.2.1.0

R2 ↔ R4 → 30.5.0.0

All networks are advertised in Area 0 (Backbone Area).

🧠 How OSPF Works in This Lab

OSPF is enabled on each router.

Networks are added using wildcard masks.

Routers form neighbor relationships over serial links.

Link-State Advertisements (LSAs) are exchanged.

Each router builds a complete topology database.

Shortest path is calculated using Dijkstra’s SPF algorithm.

Routes are installed into the routing table.

🔎 Verification Commands
Use the following commands to verify OSPF operation:
show ip ospf neighbor
show ip route
show ip ospf database
OSPF learned routes will appear as:
O 192.168.x.x
(O = OSPF learned route)

📚 Key Learning Points
OSPF process ID is locally significant
All routers must be in the same area to form adjacency
Wildcard masks are inverse of subnet masks
Area 0 is the backbone of OSPF
OSPF uses cost as metric
Dynamic route convergence

🎯 Learning Outcomes
After completing this lab, you will understand:
Link-state routing concepts
OSPF neighbor formation
Route advertisement using wildcard masks
OSPF Area design basic
Dynamic routing verification
Shortest path calculation behavior
