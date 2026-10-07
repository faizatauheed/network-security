Network Configuration & Security | Cisco Packet Tracer 
Project Overview  
This project shows you how to design, implement and set up the security of a segmented enterprise network using Cisco Packet Tracer.  
It was configured with VLANs, IPv4 subnetting, 802.1Q trunking, router-on-a-stick inter-VLAN routing, and extended Access Control Lists (ACLs). 
 The main goal of the security was to keep different network segments separate, and to deny access to the sensitive network segments (Admin and IT VLANs) from the Guest VLAN, while still providing the necessary network connectivity. 
Objectives 
 Design an enterprise network with segments.  
•	Design a segmented enterprise network. 
•	Configure multiple VLANs. 
•	Implement IPv4 subnetting and IP addressing. 
•	Configure 802.1Q trunk links. 
•	Implement router-on-a-stick inter-VLAN routing. 
•	Configure extended ACLs for network access control. 
•	Restrict Guest VLAN access to sensitive network segments. 
•	Test connectivity and security policies. 
•	Troubleshoot VLAN, routing, trunking, and ACL issues. 
 
Network Architecture 
The network consists of separate VLANs representing different departments and user groups. 
VLAN 	Department 	Network 	Default Gateway 
10 	Admin 	192.168.10.0/24 	192.168.10.1 
20 	IT 	192.168.20.0/24 	192.168.20.1 
30 	Guest 	192.168.30.0/24 	192.168.30.1 
 
Network Design 
  
Access Policy 
Source 	Destination 	Access 
Admin 	IT 	Allowed 
Admin 	Guest 	Allowed 
IT 	Admin 	Allowed 
IT 	Guest 	Allowed 
Guest 	Internet/Permitted Services 	Allowed 
Guest 	Admin 	  Denied 
Guest 	IT 	  Denied 
 
Technologies Used 
•	Cisco Packet Tracer 
•	Cisco IOS 
•	VLANs 
•	IPv4 
•	Subnetting 
•	802.1Q Trunking 
•	Router-on-a-Stick 
•	Inter-VLAN Routing 
•	Extended ACLs 
•	Ping Testing 
•	Network Troubleshooting 
Testing 
The implementation was tested using Cisco IOS commands and end-device connectivity tests. 
Examples: 
show vlan brief show interfaces trunk show ip interface brief show access-lists 
Connectivity was tested using: 
ping 192.168.10.1 ping 192.168.20.1 ping 192.168.30.1 
 
Troubleshooting 
When implementing, a number of typical networking configuration problems were taken into account:  
•	Incorrect VLAN assignment  
•	Missing VLAN configuration  
•	Trunk configuration errors  
•	Incorrect subnet masks  
•	Incorrect default gateways  
•	The configuration of the subinterface on the router  
•	Incorrect ACL placement  
Addressing errors that involve the incorrect source/destination addresses: Connectivity errors due to configuration errors The troubleshooting included checking VLAN membership, trunk status, IP addressing, routing configuration, and ACL counters. 
 
Repository Contents 
 
README.md 
REPORT.md 
TOPOLOGY.md 
CONFIGURATIONS.md 
TESTING.md 
TROUBLESHOOTING.md 
SECURITY.md 
 
configs/ screenshots/ packet-tracer/ 
 
Skills Demonstrated 
This project demonstrates practical knowledge of: 
•	Network segmentation 
•	VLAN configuration 
•	IPv4 subnetting 
•	Cisco IOS 
•	Inter-VLAN routing 
•	802.1Q trunking 
•	Access Control Lists 
•	Network security 
•	Connectivity testing 
•	Network troubleshooting 
•	Cisco Packet Tracer 
Author 
Faiza Tauheed 
BS Cyber Security 
Project Purpose 
This project was developed as a practical networking and cybersecurity exercise to demonstrate how network segmentation and access-control policies can be implemented using Cisco networking technologies. 
