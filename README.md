# CMPG325 Computer Networks — Milestone 1: Client Design Review

**Student Name:** SEMARA, K  
**Student Number:** 36233137  
**Project ID:** CMPG325-2026-127  
**Client ID:** CLI-127  
**Assigned Organisation:** North-West Community Radio FM (Mahikeng)  
**Industry:** Media  
**Assigned Subnet Block:** 172.30.82.0/23  
**Assigned Technical Challenge:** EtherChannel (Link Aggregation)  
**Submission Date:** 28 August 2026  

---

## 1. Client Requirements Analysis & Design Justification

### 1.1 Business Context & Problem Statement
North-West Community Radio FM is a media broadcasting station based in Mahikeng. Modern broadcasting environments require high-availability, low-latency, and scalable network architectures to support concurrent digital audio streams, live station feeds, dedicated broadcast management systems, and general administrative services. This project presents a structured network solution designed and simulated in Cisco Packet Tracer to fulfill the client's operational demands.

### 1.2 Client Scope & Operational Constraints
* **IP Addressing Assignment:** Subnet allocation strictly using `172.30.82.0/23`.
* **Design Constraint (Restricted Server Access):** Server room infrastructure must be physically and logically restricted to authorized IT personnel only.
* **Assigned Technical Challenge:** EtherChannel implementation using LACP (Link Aggregation Control Protocol) across switch inter-connects to eliminate network bottlenecks and provide link redundancy.
* **Client Change Request (CR2):** Seamless logical and physical network expansion to accommodate an additional floor/building area without disrupting the baseline operational architecture.

---

## 2. Network Topology Architecture

### 2.1 Physical Topology: Extended Hierarchical Star
The physical infrastructure uses an **Extended Hierarchical Star Topology**. A centralized Core/Distribution switch layer acts as the star hub, interconnecting access switches dedicated to specific operational zones:
* **Spoke 1:** Studio & On-Air Production Access Switch
* **Spoke 2:** Administration & Management Access Switch
* **Spoke 3:** Restricted Server Room Access Switch
* **Spoke 4 (CR2):** Additional Floor Expansion Access Switch
