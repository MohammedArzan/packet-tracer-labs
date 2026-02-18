📡 EIGRP Routing – 4 Router Ring Topology (Packet Tracer Lab)

📘 Project Overview

This lab demonstrates EIGRP (Enhanced Interior Gateway Routing Protocol) in a 4-router ring topology.
The objective of this project is to help beginners understand:
How dynamic routing works
How routers exchange routes using EIGRP
How different IP networks are advertised
How a ring topology provides multiple path redundancy
How routing tables are built dynamically

This lab is designed strictly for learning and concept clarity purposes.

🏗️ Topology Design
The topology consists of:
4 Routers (R1, R2, R3, R4)
3 LAN networks
4 WAN links forming a ring

🔁 Ring Connectivity

R1 ↔ R2 (169.0.0.0 network)

R2 ↔ R3 (195.0.0.0 network)

R3 ↔ R4 (77.0.0.0 network)

R4 ↔ R1 (172.10.0.0 network)

This creates a closed loop (ring) allowing route redundancy.

🖥️ LAN Networks

R1 LAN → 192.168.1.0/24

R2 LAN → 195.168.10.0/24

R3 LAN → 192.168.2.0/24

Each LAN is connected to one router and advertised via EIGRP.

🧠 Why Different IP Ranges Are Used

Different IP ranges are intentionally used to help learners:

Clearly distinguish between LAN and WAN networks

Understand route advertisement

Identify networks in show ip route

Observe how EIGRP handles various network classes

This approach improves conceptual clarity.

🔄 How EIGRP Works in This Lab

Each router runs EIGRP in AS 10.
Routers advertise directly connected networks.
Neighbor relationships are formed over serial links.
Routing tables are built dynamically
All LAN networks become reachable from every router.
After configuration, routers automatically learn:
Remote LAN networks
Alternate paths in the ring
Best path based on EIGRP metric

🔎 Verification Commands

To verify EIGRP operation:
show ip route
show ip eigrp neighbors
show ip eigrp topology

Routes learned via EIGRP will appear as:

D 192.168.x.x
(D = EIGRP learned route)
