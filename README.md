# Enterprise Network Design & Implementation | Cisco Packet Tracer

## 📌 Project Overview

This project demonstrates the design and implementation of an enterprise-style network using **Cisco Packet Tracer**. The network is segmented into multiple VLANs to improve organization and security, with inter-VLAN routing, IP address allocation, name resolution, external connectivity, and access control.

The project focuses on practical networking concepts, network segmentation, traffic control, and troubleshooting.

## 🎯 Objectives

- Design a structured enterprise network topology.
- Implement VLAN-based network segmentation.
- Enable communication between VLANs using Layer 3 switching.
- Configure DHCP and DNS services.
- Implement static routing and simulated ISP connectivity.
- Configure NAT/PAT for outbound connectivity.
- Apply Access Control Lists (ACLs) to restrict unauthorized traffic.
- Validate network connectivity and security policies.

## 🛠️ Technologies & Components

- **Cisco Packet Tracer** — Network simulation
- **Cisco Catalyst 3560 Layer 3 Switch** — Inter-VLAN routing using SVIs
- **Cisco 2911 Router** — Edge routing and external connectivity
- **VLANs and Trunk Links** — Network segmentation and inter-switch communication
- **DHCP and DNS** — IP address allocation and name resolution
- **Static Routing** — Route configuration between network segments
- **NAT/PAT** — Address translation for simulated external connectivity
- **Access Control Lists (ACLs)** — Traffic filtering and network access control

## 🏗️ Network Architecture

The network is divided into four VLANs:

| VLAN ID | Department / Purpose |
|---|---|
| 10 | Management |
| 20 | Users / Employees |
| 30 | Servers |
| 40 | Security |

The Layer 3 switch handles inter-VLAN routing, while the edge router connects the internal network to a simulated ISP environment.

Trunk links carry traffic for multiple VLANs between network devices. ACLs enforce restrictions on selected inter-VLAN traffic.

## ⚙️ Implementation

### 1. VLAN Segmentation
Created separate VLANs for Management, Users, Servers, and Security to logically isolate network resources.

### 2. Switching and Trunking
Configured switch access ports and trunk links to support communication across the VLAN infrastructure.

### 3. Inter-VLAN Routing
Configured Switch Virtual Interfaces (SVIs) on the Layer 3 switch to route traffic between VLANs.

### 4. DHCP and DNS
Configured network services for IP address allocation and name resolution.

### 5. Static Routing and ISP Simulation
Configured static routes and an edge router to establish connectivity with a simulated external network.

### 6. NAT/PAT
Implemented address translation to support outbound connectivity from the internal network to the simulated external environment.

### 7. ACL-Based Security
Applied access control rules to restrict selected traffic between VLANs and demonstrate network segmentation.

## 🧪 Testing & Validation

The following checks were performed during the project:

- **External connectivity:** Verified connectivity from the internal network to a simulated external server through the NAT/PAT configuration.
- **ACL enforcement:** Confirmed that the tested traffic between Users and Management was blocked by the configured access control policy.
- **Server connectivity:** Verified that the internal web server at `192.168.30.20` was reachable using ping.
- **HTTP testing:** The browser displayed a blank page during testing. Successful HTTP content delivery was therefore not confirmed.

## 📸 Project Evidence

Screenshots and configuration evidence will be organized in the repository to document:

- Overall network topology
- VLAN and trunk configurations
- Layer 3 switch routing table
- Edge router routing table
- NAT/PAT configuration and testing
- ACL configuration and verification

## 📂 Project Files

The repository will contain the following items as they are added:

- Cisco Packet Tracer `.pkt` project file
- Network topology screenshots
- Configuration documentation
- Testing evidence
- Troubleshooting notes

## 📚 Key Learnings

- Designing and segmenting enterprise networks using VLANs
- Configuring Layer 3 switching and inter-VLAN routing
- Understanding static routing and edge-router connectivity
- Implementing NAT/PAT
- Applying ACLs to control network traffic
- Testing network connectivity and troubleshooting configuration issues

## 🚀 Future Improvements

- Complete HTTP service troubleshooting and verify web-page access.
- Document the IP addressing plan and device configurations.
- Expand security controls and validate additional traffic policies.
- Add further network hardening and management features.

## 👨‍💻 Author

**Networking & Cybersecurity Lab Project**

Built as part of practical networking development and preparation for cybersecurity and SOC analyst roles.
