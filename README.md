# NexusFlow-Enterprise-Infrastructure

<img width="1512" height="739" alt="Screenshot 2026-04-06 113550" src="https://github.com/user-attachments/assets/1f686e74-5ed8-4979-a3a8-17173b7fb42e" />

## 📌 Project Overview
**NexusFlow** is a high-availability, multi-site enterprise network simulation designed using **Cisco Packet Tracer**. The project demonstrates a robust corporate infrastructure connecting four geographical branches to a centralized Data Center using advanced routing and switching protocols.

## 🏗️ Architecture & Topology
The network is built on a **Mesh-Ring Topology** to ensure maximum redundancy and zero-downtime.

### Core Components:
* **Edge Routers:** 4x Cisco 2911 Routers managing inter-branch connectivity.
* **Data Center:** Dedicated Server Farm (DNS, HTTP, DHCP) connected via high-speed links.
* **Access Layer:** Cisco 2960 Switches handling multi-department end-devices (PCs & Laptops).

## 🛠️ Technical Specifications
* **Routing Protocol:** Dynamic **OSPF (Open Shortest Path First)** Area 0 for fast convergence and optimal path selection.
* **IP Addressing:** VLSM-optimized IPv4 addressing scheme to prevent IP wastage.
* **Network Services:**
    * **DHCP:** Automated IP allocation for all branches and the Server Farm.
    * **WAN Connectivity:** Serial DCE/DTE links with HDLC encapsulation.
    * **Redundancy:** Failover paths configured to maintain connectivity if a primary link fails.

## 🚀 Key Features
- [x] Full End-to-End connectivity between all branches.
- [x] Automated IP management via centralized/distributed DHCP pools.
- [x] Scalable design (Ready to add more branches or VLANs).
- [x] OSPF Router-ID implementation for organized management.

## 💻 How to Run
1. Download the `.pkt` file from this repository.
2. Open it using **Cisco Packet Tracer (v8.2 or higher)**.
3. Wait for OSPF convergence (Green lights on all interfaces).
4. Test connectivity by pinging from any Branch PC to the **Data Center Server (192.168.5.x)**.

---
**Developed by:** Belal Eladawy
**Field:** Network Engineering | Systems Architecture
