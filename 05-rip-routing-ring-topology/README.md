# RIP Routing Lab – 4 Router Ring Topology (Cisco Packet Tracer)

## 📌 Project Overview

This project demonstrates dynamic routing using RIP (Routing Information Protocol) in a 4-router ring topology.

Each router represents a branch network with its own LAN. The routers are interconnected using serial WAN links and exchange routing information dynamically using RIP version 2.

This lab is designed for beginners and students who want to understand how dynamic routing works in real-world multi-router networks.

---

## 🏗️ Network Design

### LAN Networks

| Router | LAN Network |
|--------|------------|
| R1 | 192.168.10.0/24 |
| R2 | 192.168.20.0/24 |
| R3 | 192.168.30.0/24 |
| R4 | No local LAN (WAN transit router) |

### WAN Links

| Link | Network |
|------|---------|
| R1 ↔ R2 | 192.168.40.0/24 |
| R2 ↔ R3 | 192.168.50.0/24 |
| R3 ↔ R4 | 192.168.60.0/24 |
| R4 ↔ R1 | 192.168.70.0/24 |

The routers form a ring topology, allowing multiple path possibilities.

---

## 🧠 Concepts Covered

- Dynamic Routing using RIP v2
- Router-to-router WAN connectivity
- Ring topology design
- Automatic route learning
- Route table verification
- End-to-end LAN communication

---

## 🔁 How RIP Works in This Lab

- Each router advertises its directly connected networks.
- Routers exchange routing updates every 30 seconds.
- Routing decisions are made based on hop count.
- The best path is selected automatically.
- If a link fails, RIP recalculates an alternate route (if available).

RIP version 2 is used to support classless routing and subnet mask awareness.

---

## 🔍 Verification

To confirm RIP is working:

- Use `show ip route`
- RIP-learned routes appear with the letter **R**
- Test connectivity using `ping` between PCs in different LANs

Successful communication confirms correct dynamic routing operation.

---

## 🧪 Testing Results

✔ All LAN networks can communicate with each other  
✔ Routes are learned dynamically (no static routes used)  
✔ Routing tables update automatically  
✔ Full end-to-end connectivity achieved  

---

## 📂 Files Included

- rip-routing-4-router-ring.pkt
- topology.png
- router-configs.txt

---

## 🎯 Learning Outcomes

Through this project, I learned:

- The difference between static and dynamic routing
- How RIP automatically exchanges route information
- How routing tables are built dynamically
- How multi-router WAN topologies operate
- How to verify routing protocol functionality

This project strengthens foundational CCNA routing concepts and real-world network design understanding.
