# CMPG 325 Individual Project - CLI-127
**Student Name:** SEMARA, K  
**Student ID:** 36233137  
**Client:** North-West Community Radio FM (Mahikeng)  

## Project Overview
This repository contains the design, documentation, Packet Tracer network simulation, and configuration evidence for North-West Community Radio FM.

## Milestone Breakdown
- [x] Milestone 1: Requirements Analysis, Topology Design, & IP Addressing Plan
- [ ] Milestone 2: Packet Tracer Implementation & EtherChannel Verification
- [ ] Final Submission: Complete Video Demo, Technical Report, & Documentation

## Subnetting & IP Addressing Scheme
- Base Address: 172.30.82.0/23
- Design Constraints Included: Restricted Server Access (VLAN 30) & CR2 Expansion (VLAN 40).
- 
### Physical Topology: Hierarchical Extended Star
The physical network utilizes a Hierarchical Star Topology centered on a dual-switch Core/Distribution backbone. 

- **Core Node:** A central distribution switch acts as the central hub of the star topology.
- **Access Spokes:** Edge switches located in each station department (Studio, Admin, Restricted Server Room, and the CR2 Floor Expansion) connect directly to the central core in a point-to-point star configuration.
- **Redundant Trunking:** Links between the star hub and access switches are configured using LACP EtherChannel (Link Aggregation), providing high-speed redundant trunks to support uncompressed media streaming and prevent single points of failure.
