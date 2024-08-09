**Objective**

The main motive of this project is to design and implement a secure Telecommunication Company Network which has two floors of departments. One floor is hosting HR and Finance (40), Product Brand and Marketing (45), and Admin and Corporate departments (35). The second floor is hosting IT Network & Support (45), Software Engineering (36), and Cloud Engineering departments (32) departments. The company has subscribed to Seacom ISP for internet services and has purchased one 5525-X Cisco ASA Firewall, one Catalyst 3850 48-Port Switch, 3 Catalyst 2960 48-Port Switches, 2 Catalyst 2960 24-Port Switches, 1 Cisco Voice Gateway, 1 Cisco WLC, and 6 LAPs. The company has Cisco Voice Gateways to provide VoIP or telephony services in the network and Cisco WLC to provide central management for Aps.
The company has emphasized high performance, redundancy, scalability, and availability, and hence you are required to provide a complete Cairo Telco network infrastructure design and implementation. The company will be using the following IP address: 10.20.0.0/16 for WLAN, 192.168.10.0/24 for LAN, 172.16.10.0/24 for Voice, 10.10.10.0/28 for DMZ and 197.200.100.0 for public addresses.

**Details of design**

Hierarchical Design- Use a hierarchical model providing redundancy at every layer.
ISPs- The network is also expected to connect to a Seacom ISP Router.
WLC- Each department is required to have a WAP providing both employees and guest WIFI managed by WLC.
VoIP- Each department should have IP phones.
VLAN- The LAN, WLAN, and VoIP VLANs remain at 50, 60 & 101 respectively for the entire network.
EtherChannel- Use standard LACP as a method of link aggregation.
STP PortFast and BPDUguard- configure the two protocols to enable faster port transition from blocking to forwarding.
Subnetting- Provided the networks above, carry out subnetting to allocate the correct number of IP addresses to each department.
Basic settings- Configure basic device settings such as hostnames, and console passwords, enable passwords, and banner messages, encrypt all passwords, and disable IP domain lookup.
Inter-VLAN Routing- Devices in all the departments are required to communicate with each other with the respective multilayer switch configured for inter-VLAN routing.
Core Switch- The Multilayer switches are expected to carry out both routing and switching functionalities and thus will be assigned IP addresses.
DHCP Server- All devices in the network (except IP phones) are expected to obtain an IP address dynamically from the AD servers located at the server farm site.
Cisco 2811 Router- Ensure to have a router that can support telephony service i.e Cisco Catalyst 2811(the VoIP router should be connected to the l3-switch).
Static Addressing- Devices in the server room are to be allocated IP addresses statically.
Telephony Service- Configure VoIP on the voice gateway router and allocate dial numbers in format (1...).
Routing Protocol- Use OSPF as the routing protocol to advertise routes both on the routers and multilayer switches.
Cisco ASA Firewall- Configure security levels, zones, and policies to define how resources are accessed in the network
Final- Test Communication, ensure everything configured is working as expected.

**Technologies Implementation Sequence**

Creating a network topology using Cisco Packet Tracer.
Hierarchical Network Design.
Connecting Networking devices with Correct cabling.
Configuring Basic device settings.
Creating VLANs and assigning ports VLAN numbers.
Creating both data and voice VLANs and assigning ports VLAN numbers.
Configuring Spanning-Tree Protocol - STP PortFast and BPDUGuard EtherChannel using LACP method.
Subnetting and IP Addressing configuration.
Configuring Inter-VLAN Routing both on the Switches (SVI) and Routers (router-on-a-stick).
Configuring Dedicated DHCP Server device for Data to provide dynamic IP allocation.
Configuring Routers as DHCP server for Voice to provide IP Phones dynamic IP allocation.
Configuring Active Directory as DHCP Server.
Configuring WLAN network- Wireless LAN Controller + Wireless Lightweight Access Points.
Configuring SSH for secure Remote access to only Senior Network Security Engineer.
Configuring OSPF as the routing protocol.
Configuring Standard ACL for VTY interfaces to restrict remote Access using SSH.
Configuring VoIP or Telephony service configuration in VoIP routers.
Configuring Cisco ASA Firewall Interface descriptions, zones, and security levels.
Configuring Cisco ASA Firewall Object Network + NAT + Default Static Routes.
Configuring Cisco ASA Firewall OSPF.
Configuring Cisco ASA Firewall Inspection Policies to filter traffic based on predetermined ACLs.
Host Device Configurations.
