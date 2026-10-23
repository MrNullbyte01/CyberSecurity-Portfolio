# VLAN Configuration and Inter-VLAN Routing

## Project Overview
In this Cisco Packet Tracer lab, I created and configured multiple VLANs and implemented inter-VLAN routing to enable communication between devices in different VLANs.

## Objectives
- Create VLAN 10, VLAN 20, VLAN 30, and VLAN 40.
- Assign switch ports to the appropriate VLANs.
- Configure inter-VLAN routing.
- Enable communication between devices in different VLANs.
- Verify connectivity using ping tests.

## Technologies Used
- Cisco Packet Tracer
- Cisco IOS CLI
- VLANs
- Inter-VLAN Routing
- IPv4 Addressing

## Configuration Steps
1. Created VLANs 10, 20, 30, and 40 on the switch.
2. Assigned access ports to their corresponding VLANs.
3. Configured the required IP addressing for end devices.
4. Configured inter-VLAN routing to allow communication between VLANs.
5. Tested connectivity between devices using ping commands.

## What I Learned
- How VLANs separate a network into logical broadcast domains.
- How to configure VLANs and assign switch ports.
- How inter-VLAN routing enables communication between different VLANs.
- How to troubleshoot network connectivity using ping tests and CLI commands.

## Project Status
Completed — Cisco Packet Tracer lab.

## Evidence
assets/Inter-Vlan Routing (Router on a Stick).png






# Multilayer Switch Default Gateway Configuration

## Project Overview

In this Cisco Packet Tracer lab, I configured the default gateway on a multilayer switch to enable communication with devices outside the local network.

## Objectives

- Configure a multilayer switch.
- Set up the default gateway for management or Layer 3 connectivity, depending on the network configuration.
- Understand how a default gateway is used to reach remote networks.
- Verify network connectivity.

## Technologies Used

- Cisco Packet Tracer
- Cisco IOS CLI
- Multilayer Switching
- Default Gateway
- IPv4 Networking

## What I Learned

- The purpose of a default gateway in a network.
- The difference between a Layer 2 switch's management default gateway and a Layer 3 switch's IP routing configuration.
- How multilayer switches can perform routing between networks.
- How to verify connectivity and troubleshoot gateway-related issues.

## Project Status

Completed — Cisco Packet Tracer lab.

## Evidence

Network topology screenshots and relevant CLI configurations can be added here.






# EtherChannel Configuration Between Two Switches

## Project Overview

In this Cisco Packet Tracer lab, I configured an EtherChannel connection between two switches to combine multiple physical links into one logical link.

## Objectives

- Connect two switches using multiple physical links.
- Configure EtherChannel between the switches.
- Improve link redundancy and utilize multiple physical connections.
- Verify the EtherChannel status and connectivity.

## Technologies Used

- Cisco Packet Tracer
- Cisco IOS CLI
- EtherChannel
- Link Aggregation
- Switch-to-Switch Connectivity

## Configuration Steps

1. Connected two switches using multiple physical Ethernet links.
2. Configured the participating interfaces on both switches.
3. Created an EtherChannel group to combine the physical links.
4. Verified the Port-Channel interface and link status.
5. Tested network connectivity between devices connected to the switches.

## What I Learned

- How EtherChannel combines multiple physical links into one logical link.
- How link aggregation can provide redundancy and increased aggregate bandwidth.
- How to configure and verify EtherChannel between switches.
- How to troubleshoot EtherChannel configuration mismatches.

## Project Status

Completed — Cisco Packet Tracer lab.

## Evidence

Add screenshots of the network topology, EtherChannel configuration, and verification commands.

Useful verification commands:

- `show etherchannel summary`
- `show interfaces port-channel 1`
- `show interfaces trunk`






# DHCP, DNS, and Static Routing Configuration

## Project Overview

In this Cisco Packet Tracer project, I configured a router as a DHCP server, set up DNS services, and implemented static routing to enable communication between different networks and provide name resolution for network devices.

## Objectives

- Configure a router as a DHCP server to assign IP addresses automatically.
- Configure a DNS server to resolve domain names into IP addresses.
- Implement static routes to enable communication between different networks.
- Test network connectivity and verify DHCP and DNS functionality.

## Technologies Used

- Cisco Packet Tracer
- Cisco IOS CLI
- DHCP
- DNS
- Static Routing
- IPv4 Addressing

## Configuration Steps

1. Configured DHCP pools on the router, including network addresses, default gateways, and DNS server information.
2. Configured a DNS server and added DNS records for name resolution.
3. Configured static routes on the routers to reach remote networks.
4. Configured end devices to obtain IP addresses automatically through DHCP.
5. Tested connectivity using ping commands and verified DNS name resolution.

## What I Learned

- How DHCP automatically assigns IP configuration to network devices.
- How DNS translates domain names into IP addresses.
- How to configure static routes between different networks.
- How DHCP, DNS, and routing work together in a network.
- How to troubleshoot connectivity and name resolution issues.

## Verification Commands

- `show ip dhcp binding`
- `show ip route`
- `ping <destination-ip>`

## Project Status

Completed — Cisco Packet Tracer lab.

## Evidence

Add screenshots of the network topology, DHCP configuration, DNS records, static routing table, and successful connectivity tests.





# Network Security and Switch Hardening

## Project Overview

In this Cisco Packet Tracer project, I configured a router as a DHCP server and implemented multiple Layer 2 security measures to improve network security, reduce unauthorized access, and protect the switching infrastructure.

## Objectives

- Configure a router as a DHCP server.
- Establish EtherChannel between SW0 and SW1.
- Shut down all unused switch ports.
- Configure switch port security.
- Disable DTP and CDP where appropriate.
- Implement DHCP Snooping to help prevent rogue DHCP server attacks.
- Configure STP PortFast and BPDU Guard on appropriate access ports.
- Add descriptions to all switch interfaces for easier network management.

## Technologies Used

- Cisco Packet Tracer
- Cisco IOS CLI
- DHCP
- EtherChannel
- Port Security
- DHCP Snooping
- Spanning Tree Protocol (STP)
- PortFast and BPDU Guard
- DTP and CDP
- Interface Descriptions

## Configuration Steps

1. Configured DHCP services on the router to assign IP addresses automatically.
2. Configured EtherChannel between SW0 and SW1 to combine multiple physical links into one logical link.
3. Administratively shut down unused switch ports.
4. Applied port security to selected access ports to restrict unauthorized devices.
5. Disabled Dynamic Trunking Protocol (DTP) and CDP where appropriate.
6. Enabled DHCP Snooping and configured trusted interfaces as required.
7. Enabled PortFast and BPDU Guard on appropriate end-device access ports.
8. Added descriptions to switch interfaces to identify their purpose and connected devices.

## Security Benefits

- Reduces the risk of unauthorized device connections.
- Helps protect against rogue DHCP servers.
- Reduces unnecessary exposure from unused switch ports.
- Helps protect the Layer 2 network against certain spanning-tree attacks.
- Improves interface management and troubleshooting.
- Provides redundancy and link aggregation through EtherChannel.

## Verification Commands

- `show ip dhcp binding`
- `show etherchannel summary`
- `show port-security`
- `show ip dhcp snooping`
- `show spanning-tree`
- `show interfaces status`
- `show running-config`

## What I Learned

Through this project, I gained practical experience with router-based DHCP configuration, EtherChannel, Layer 2 security hardening, switch port management, and spanning-tree protection mechanisms.

## Project Status

Completed — Cisco Packet Tracer lab.

## Evidence

Add screenshots of the network topology, EtherChannel status, port-security settings, DHCP Snooping configuration, STP protection, and interface descriptions.





# Static Routing: Default, Floating, and Static Routes

## Project Overview

In this Cisco Packet Tracer lab, I configured different types of static routes to control how traffic is forwarded between networks. The project covers standard static routes, default routes, and floating static routes for backup connectivity.

## Objectives

- Configure standard static routes to reach remote networks.
- Configure a default route for destinations without a more specific routing-table entry.
- Configure floating static routes as backup routes.
- Understand administrative distance and route selection.
- Verify routing-table entries and network connectivity.

## Technologies Used

- Cisco Packet Tracer
- Cisco IOS CLI
- IPv4 Routing
- Static Routing
- Default Routing
- Floating Static Routes
- Administrative Distance

## Configuration Steps

1. Configured static routes to reach specific remote networks.
2. Configured a default route to forward traffic to an upstream router.
3. Configured floating static routes with a higher administrative distance than the primary route.
4. Verified the routing table and route selection.
5. Tested connectivity between networks and checked backup-route behavior.

## What I Learned

- How static routes direct traffic to specific destination networks.
- How default routes provide a path for destinations not listed more specifically in the routing table.
- How floating static routes can provide backup paths when a preferred route becomes unavailable.
- How administrative distance affects route selection.
- How to troubleshoot routing and connectivity issues.

## Verification Commands

- `show ip route`
- `show running-config`
- `ping <destination-ip>`
- `traceroute <destination-ip>`

## Project Status

Completed — Cisco Packet Tracer lab.

## Evidence

Add screenshots of the network topology, routing configurations, routing tables, and successful connectivity tests.





# OSPF Configuration and ISP Connectivity

## Project Overview

In this Cisco Packet Tracer project, I configured dynamic routing using OSPF, established default-route connectivity for EV1 and EV2 through Delta, configured DHCP services for LANs, and set the DNS server address to 8.8.8.8. I then verified end-to-end network connectivity.

## Objectives

- Configure EV1 and EV2 to reach Delta through a default route.
- Configure OSPF on the Delta network.
- Configure DHCP for LAN devices.
- Set the DNS server address to 8.8.8.8.
- Verify connectivity between devices and networks.

## Technologies Used

- Cisco Packet Tracer
- Cisco IOS CLI
- OSPF Dynamic Routing
- Default Routing
- DHCP
- DNS
- IPv4 Networking

## Configuration Steps

1. Configured default routes so EV1 and EV2 could forward traffic toward Delta.
2. Enabled OSPF on the Delta network to exchange routing information dynamically.
3. Configured DHCP services for the LANs to assign IP addresses automatically.
4. Set the DNS server address to 8.8.8.8 in the relevant DHCP configuration.
5. Tested connectivity between network devices and verified routing behavior.

## What I Learned

- How default routes provide a path toward an upstream network.
- How OSPF dynamically advertises and learns routes.
- How to configure DHCP for multiple LANs.
- How DNS server information can be distributed to clients through DHCP.
- How to troubleshoot routing and end-to-end connectivity.

## Verification Commands

- `show ip route`
- `show ip ospf neighbor`
- `show ip protocols`
- `show ip dhcp binding`
- `ping <destination-ip>`
- `traceroute <destination-ip>`

## Project Status

Completed — Cisco Packet Tracer lab.

## Evidence

Add screenshots of the network topology, OSPF neighbors, routing tables, DHCP assignments, DNS settings, and successful connectivity tests.





# ACL Configuration and Traffic Filtering

## Project Overview

In this Cisco Packet Tracer lab, I performed the initial network configuration and implemented Standard and Extended Access Control Lists (ACLs) to control traffic between specific hosts, LANs, and network services.

## Objectives

- Perform the initial network configuration.
- Configure an Extended ACL to block HTTP traffic from LAN1.
- Block ICMP traffic from PC7 to the web server.
- Configure a Standard ACL to block PC11 from accessing the DNS server.
- Verify that permitted traffic works and denied traffic is blocked as intended.

## Technologies Used

- Cisco Packet Tracer
- Cisco IOS CLI
- Standard ACLs
- Extended ACLs
- HTTP Traffic Filtering
- ICMP Filtering
- DNS Access Control
- IPv4 Networking

## Configuration Steps

1. Completed the initial configuration of the network devices and interfaces.
2. Configured an Extended ACL to deny HTTP traffic originating from LAN1.
3. Applied an Extended ACL rule to block ICMP traffic from PC7 to the web server.
4. Configured a Standard ACL to deny traffic sourced from PC11, applying it in the appropriate direction to restrict access to the DNS server.
5. Tested the ACL rules and verified the expected traffic filtering behavior.

## What I Learned

- The difference between Standard and Extended ACLs.
- How ACLs filter traffic based on source and destination information.
- How Extended ACLs can filter specific protocols and services, such as HTTP and ICMP.
- How Standard ACLs filter traffic based on source IP addresses.
- How ACL placement and interface direction affect traffic filtering.
- How to troubleshoot ACL behavior using connectivity tests and configuration commands.

## Verification Commands

- `show access-lists`
- `show ip interface`
- `show running-config`
- `ping <destination-ip>`

## Project Status

Completed — Cisco Packet Tracer lab.

## Evidence

Add screenshots of the network topology, ACL configurations, ACL hit counters, and connectivity tests demonstrating the blocked and permitted traffic.





# Enterprise Multi-Branch Network Configuration

## Project Overview

In this Cisco Packet Tracer project, I designed and configured a multi-branch enterprise network connecting multiple branches to the Delta network. The project combines dynamic and static routing, VLANs, network security, NAT, and GRE tunneling to provide connectivity between branch offices.

## Project Objectives

- Perform the initial configuration of network devices.
- Configure IP addressing for network devices and end hosts.
- Configure DHCP servers on RAB Branch 2 and Kapital Branch 1.
- Implement inter-VLAN routing at KapitalBank Branch 2.
- Configure EtherChannel at Branch 2.
- Implement port security at KapitalBank Branch 2.
- Configure an access control list to permit only HTTPS access to the web server.
- Configure OSPF on the Delta network.
- Connect all branches to Delta using default routes.
- Configure NAT Overload (PAT) on all branches.
- Establish a GRE tunnel between branches.

## Technologies Used

- Cisco Packet Tracer
- Cisco IOS CLI
- IPv4 Addressing
- DHCP
- VLANs and Inter-VLAN Routing
- EtherChannel
- Port Security
- Access Control Lists (ACLs)
- OSPF
- Default Routing
- NAT Overload (PAT)
- GRE Tunneling

## Configuration Steps

1. Completed the initial configuration of routers and switches.
2. Assigned IP addresses to network interfaces and end devices.
3. Configured DHCP services on RAB Branch 2 and Kapital Branch 1.
4. Configured inter-VLAN routing at KapitalBank Branch 2.
5. Established EtherChannel between switches at Branch 2.
6. Applied port security to selected access ports at KapitalBank Branch 2.
7. Configured ACL rules to restrict web server access to HTTPS traffic.
8. Enabled OSPF on the Delta network to exchange routing information dynamically.
9. Configured default routes on the branches to reach Delta.
10. Implemented NAT Overload (PAT) at each branch to translate private IP addresses for external connectivity.
11. Configured a GRE tunnel between branches to provide a logical point-to-point path across the underlying network.

## What I Learned

- How to design and configure a multi-branch network topology.
- How to combine DHCP, VLANs, and inter-VLAN routing.
- How EtherChannel improves link redundancy and aggregate bandwidth.
- How port security and ACLs help protect network access.
- How OSPF and default routes support network connectivity.
- How NAT Overload enables multiple internal hosts to share an external IP address.
- How GRE tunnels encapsulate traffic to create logical connections between remote networks.
- How to verify routing, security policies, and end-to-end connectivity.

## Verification Commands

- `show ip interface brief`
- `show ip route`
- `show ip ospf neighbor`
- `show ip dhcp binding`
- `show etherchannel summary`
- `show port-security`
- `show access-lists`
- `show ip nat translations`
- `show interfaces tunnel`

## Project Status

Completed — Cisco Packet Tracer lab.

## Evidence

Add screenshots of the complete network topology, IP addressing, DHCP assignments, inter-VLAN routing, EtherChannel status, port-security configuration, ACL rules, OSPF neighbors, NAT translations, GRE tunnel status, and successful connectivity tests.


## Conclusion

Through these Cisco Packet Tracer projects, I developed practical networking skills by configuring and troubleshooting different network technologies. I gained hands-on experience with VLANs, inter-VLAN routing, DHCP, DNS, static routing, OSPF, EtherChannel, NAT Overload, GRE tunnels, and network security mechanisms such as ACLs, port security, DHCP Snooping, and STP protections.

These projects helped me better understand how networks are designed, configured, secured, and interconnected. I continue to strengthen my networking fundamentals and apply what I learn through practical labs as part of my cybersecurity journey.

My goal is to build a strong foundation in networking and network security while developing the practical skills needed for a future career in cybersecurity.

