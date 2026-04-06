# NexusFlow-Enterprise-Infrastructure

<img width="1512" height="739" alt="Screenshot 2026-04-06 113550" src="https://github.com/user-attachments/assets/1f686e74-5ed8-4979-a3a8-17173b7fb42e" />

## 📌 Project Overview
**NexusFlow** is a high-availability, multi-site enterprise network simulation designed using **Cisco Packet Tracer**. The project demonstrates a robust corporate infrastructure connecting four major geographical branches using advanced dynamic routing and a fault-tolerant topology.

## 🏗️ Architecture & Topology
The network is built on a **Mesh-Ring Topology** to ensure maximum redundancy and reliable inter-branch communication.

### Core Components:
* **Edge Routers:** 4x Cisco 2911 Routers managing multi-site connectivity.
* **Access Layer:** 4x Cisco 2960 Switches handling local area networks (LAN) for each branch.
* **End Devices:** A fleet of PCs and Laptops distributed across all four sites to simulate a real-world corporate environment.

## 🛠️ Technical Specifications
* **Routing Protocol:** **OSPF (Open Shortest Path First) Area 0** for seamless dynamic routing and optimal path calculation.
* **High Availability:** Configured with redundant links to ensure the network remains operational even if a primary WAN link fails.
* **IP Addressing:** Strategic IPv4 addressing scheme designed for scalability and minimal conflict.
* **WAN Connectivity:** High-speed Serial links (DTE/DCE) with optimized clock rates and encapsulation.
* **DHCP Services:** Each branch router acts as a local DHCP server, providing automated IP management for its respective LAN.

## 🚀 Key Features
- [x] Full Mesh-Ring connectivity across all 4 geographical sites.
- [x] Automated failover and rerouting via OSPF convergence.
- [x] Zero-config end-device setup through localized DHCP pools.
- [x] Scalable framework ready for additional branches or VLAN implementation.

## 💻 How to Run
1. Download the `.pkt` file from this repository.
2. Open it using **Cisco Packet Tracer (v8.2 or higher)**.
3. Observe the OSPF adjacency process until all link lights are green.
4. Test connectivity by performing a **Ping** or **Trace Route** between any two devices in different branches.

---
**Developed by:** Belal Eladawy
**Field:** Network Engineering | Systems Architecture
