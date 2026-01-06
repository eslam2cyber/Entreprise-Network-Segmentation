# Enterprise Network Segmentation with VLANs and ACLs





## Project Overview

This project demonstrates the design and implementation of a segmented enterprise network using VLANs, Router-on-a-Stick, and Extended Access Control Lists (ACLs).

The objective is to isolate sensitive departments (HR and Finance) while allowing administrative departments (Admin and IT) controlled access to shared resources such as servers.

This project was built and tested using Cisco Packet Tracer.



## Network Architecture

The network is divided into the following VLANs:

* VLAN 10 – Admin
* VLAN 20 – Human Resources (HR)
* VLAN 30 – Finance
* VLAN 40 – IT
* VLAN 50 – Server

Inter-VLAN routing is achieved using a Router-on-a-Stick configuration.



## Security Policy

The following security rules were implemented:

* Admin and IT departments can communicate with each other.
* Admin and IT can access the Server VLAN.
* HR and Finance can access the Server VLAN only.
* HR and Finance cannot communicate with Admin, IT, or each other.
* Administrative VLANs are restricted from accessing HR and Finance networks.

These rules are enforced using Extended ACLs applied at the router level.



## Technologies Used

* Cisco Packet Tracer
* VLANs
* Trunking (802.1Q)
* Router-on-a-Stick
* Extended Access Control Lists (ACLs)
* 

## What I Learned

* Designing segmented enterprise networks
* Implementing inter-VLAN routing
* Applying Extended ACLs for traffic control
* Understanding the limitations of stateless ACLs
* Troubleshooting real-world network security issues
* 

## Design Limitations

During the design phase, a stateful firewall approach was considered.
However, Cisco Packet Tracer does not support Zone-Based Firewalls.

As a result, Extended ACLs were used to enforce security policies.
This project documents the limitations of ACL-based designs and highlights
why stateful firewalls are preferred in real enterprise environments.



\## Network Topology



!\[Network Topology](diagrams/network-topology.png)

