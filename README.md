# enterprise-network-packet-tracer-lab
Cisco Packet Tracer enterprise network featuring VLAN segmentation, inter-VLAN routing, trunking, EtherChannel, DNS, HTTP, and email services.


## Overview

This project demonstrates the design and configuration of a multi-VLAN enterprise network using Cisco Packet Tracer.

The network consists of five Cisco switches, six client laptops, and three servers. A Layer 3 multilayer switch provides routing between VLANs while the remaining switches operate at Layer 2.

## Technologies and Concepts

- Cisco Packet Tracer
- VLANs
- Inter-VLAN Routing
- Switched Virtual Interfaces (SVIs)
- 802.1Q Trunking
- EtherChannel
- Layer 2 and Layer 3 Switching
- Static IPv4 Addressing
- DNS
- HTTP
- Email Services
- Network Troubleshooting

## Network Architecture

The environment includes:

- 5 Cisco switches
- 6 client laptops
- 3 servers
- VLAN 10
- VLAN 20
- VLAN 30
- Layer 3 routing between VLANs
- EtherChannel connection between the main switches

## VLAN Networks

VLAN 10
192.168.10.0/24

VLAN 20
192.168.20.0/24

VLAN 30
192.168.30.0/24

The first usable address in each subnet is configured as the VLAN gateway using an SVI on the multilayer switch.

## Server Network

Web Server:
10.10.10.10

DNS Server:
10.10.10.11

Email Server:
10.10.10.12

## Configuration

All switch-to-switch links were configured as trunk links.

Connections to laptops and servers were configured as access ports and assigned to their appropriate VLANs.

The main multilayer switch performs inter-VLAN routing using SVIs.

EtherChannel was configured between the main switches to combine multiple physical connections into one logical link.

## DNS and Web Services

The DNS server was configured with records for:

student.com

www.student.com

Both domain names resolve to the internal web server.

The HTTP server hosts a customized webpage, and connectivity was verified from client devices across the network.

## Verification

The completed network was tested to verify:

- Communication between VLANs
- Correct VLAN membership
- Trunk connectivity
- EtherChannel operation
- DNS name resolution
- HTTP connectivity
- Client-to-server connectivity
- Routing between subnets
