# Wide-LAN-SDN
Implementation of a Wide Local Area Network using Software Defined Networking


Keywords: Software Defined Networking (SDN), Mininet, OpenDayLight (ODL), Java, Controller, Filtering, Broadcast, Address Resolution Protocol (ARP), Internet Control Message Protocol version 6 (ICMPv6)


The use of Ethernet as a network technology in corporative networks is justified by its low cost and ease regarding configuration and maintenance. However, this kind of networks that interconnects thousands of devices, is not scalable, especially due to the broadcast radiation. The broadcast radiation is produced when several devices send packets to the multicast address of the network. This process not only consumes the resources of the networks, but it also reduces the devices throughput.

With SDN, today’s static network can evolve into an extensible service delivery platform capable of responding rapidly to changing business, end-user, and market needs. Software Defined Networking (SDN) represents a new paradigm where the switches performance can be reprogrammed in a centralized way. This implies a reduction of the costs and eases the reconfiguration of the network performance. Thus, the network will adapt itself to the environment and provide a Quality of Service (QoS) appropriate to the network’s state.

The main purpose of this research will be the implementation of a wide Local Area Network using SDN, which implies a new paradigm able to reprogram networks in a flexible and centralized way.

Specifically, algorithms to reduce the impact of the broadcast storms will be designed by programming the filtering on SDN, which allows the implementation of wider local area networks, appropriate to meet the corporative networks requirements. In particular, procedures for dealing with auto configuration of IPv6 and IP and hardware address resolution on IPv4 and IPv6 will be addressed. Thus, the controller of the SDN will be programmed. It is is considered the “brain” of the network since it is responsible of managing the traffic routing on the network through the switches.

Regarding the controller’s application programming, OpenDayLight will be used as it is a SDN controller widely used and the filtering designed will be programmed in Java. The main tool used to work with SDN is the network emulator Mininet, that creates a realistic virtual network, running real kernel, switch and application code, on a single machine.

Previous research shows the limitation of the Ethernet-based networks, mainly regarding to the scalability due to the bootstrapping protocols. Especially, Address Resolution Protocol (ARP) and Internet Control Message Protocol version 6 (ICMPv6), since these two protocols are responsible of a high amount of generated traffic.

Bearing this in mind, the design of the solution is introduced divided on three stages of detection and identification of packets, filtering and redirection for each of these protocols, being able to perform simultaneously for both of them.

Generally speaking, since the controller is responsible of receiving and transmitting all the data traffic to the network, it will have a filter together with a table to store all the information available regarding the nodes belonging the network. Thus, the controller will be able to reply itself ARP and ICMPv6 requests, which makes unnecessary redirecting those requests to the rest of the network. This will make the data traffic of the network decrease, increasing at the same time the performance of the system.

Finally, the paper includes an evaluation stage presenting the results obtained in different experiments, which proves how the utilization of a controller with the solution implemented means a notable reduction of the data traffic in the network and proposes the possibility of extending the design to new protocols with the purpose of networks throughput optimization.
