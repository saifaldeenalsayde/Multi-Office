Multi-Site Office Network Design
Detailed Explanation of the Network Topology

This network diagram represents a multi-site enterprise network connecting Office A and Office B. The design is based on the principles of redundancy, scalability, and high availability, with integration of wireless, IP telephony, and server infrastructure.

Key Components of the Topology:
1. Offices A and B:

Office A and Office B are connected through high-speed redundant links, ensuring reliable communication between both locations.

Each office is equipped with various devices for end-user access, such as laptops, IP phones, and desktop PCs, and is connected to a local network via Layer 2 switches (ASWs).

2. Layer 2 Switches (ASWs) in Both Offices:

ASW-A1, ASW-A2, ASW-A3 in Office A and ASW-B1, ASW-B2, ASW-B3 in Office B serve as the access layer switches, connecting devices like laptops, PCs, and IP phones.

These switches manage the traffic within their respective office network and aggregate user devices into VLANs.

3. Distribution Layer Switches (DSWs):

DSW-A1, DSW-A2 in Office A and DSW-B1, DSW-B2 in Office B are responsible for inter-VLAN routing, network segmentation, and redundant connectivity.

These switches ensure that data can flow between different VLANs within the same office and across the two offices.

Redundant links (black dashed lines) between these distribution switches and the core layer improve fault tolerance and ensure high availability.

4. Core Layer and Routing:

The Core Layer is represented by Router R1, which is responsible for routing between the offices and connecting the entire network to the Internet.

R1 manages routing between Office A and Office B, and also provides internet connectivity to both offices via WAN links (red lines).

Static or dynamic routing protocols (e.g., OSPF, EIGRP) could be used between R1 and the distribution layer to ensure optimal path selection.

5. Wireless and Telephony Infrastructure:

Each office contains Wireless LAN Controllers (WLC) and Lightweight Access Points (LWAP) to manage wireless network connectivity for devices like laptops.

IP Phones in each office are connected to the network to provide voice communication services. These phones are typically powered through the Ethernet network (PoE) and rely on the IP network for voice traffic.

6. Servers and Additional Devices:

Office B includes a server (SRV1) connected to the network, providing essential services like file storage, authentication, or other enterprise applications.

Both offices also include Laptops, PCs, and IP Phones, all of which communicate over VLANs designed to segregate traffic and improve network performance.

7. Redundancy and High Availability:

The redundant links between the distribution and core layers, shown with red lines, ensure that the network remains operational even if one link fails.

Spanning Tree Protocol (STP) or similar protocols prevent Layer 2 loops while maintaining fault tolerance.

8. Internet Connectivity:

The Internet is connected to the core via Router R1, which serves as the gateway to external services.

Key Features of the Design:

VLAN Segmentation: Devices in each office are organized into VLANs to improve network performance and security.

Redundancy: The network utilizes multiple links between switches to ensure that if one path fails, another will take over without disruption.

Scalability: The design allows for easy expansion by adding additional devices or office locations, and new VLANs can be easily configured.

Wireless Integration: The design supports wireless connectivity for mobile devices, allowing seamless access to the network.

IP Telephony: The network infrastructure supports IP phones, enabling voice services across the organization.
