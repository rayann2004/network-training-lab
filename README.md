 Network_Training_Labs

This repository includes the configurations and setups I worked on during my network training  
It covers Cisco switch labs Cisco ASA firewall configurations and a Mikrotik router setup  

 Repository_Structure
- Switch/  VLANs port security trunking and DHCP snooping  
- Firewall/  ASA firewall full running configuration and step by step setup  
- MikroTik/  Screenshot of my Mikrotik router configuration  

 Devices_and_Tools
- Cisco Catalyst Switch IOS  
- Cisco ASA 5506 Firewall ASA OS 9.8  
- Mikrotik RouterOS
- Putty
  

 What_I_Configured


-Switch Configuration
Hostname set (rayan) with local admin user and enable secret
VLANs 10 (Sales) and 20 (Marketing) with inter-VLAN separation
Port security on access ports (FastEthernet0/1, 0/2)
Trunk port (GigabitEthernet0/1) allowing VLANs 10 & 20
Rapid-PVST spanning tree
QoS: COS trust enabled
DHCP snooping and Dynamic ARP inspection for security
SSH enabled, HTTP disabled, HTTPS enabled

-ASA Firewall Configuration
Hostname (rayan) and domain name (ccg)
Encrypted enable password
Interfaces configured:
Outside (DHCP client)
Inside VLANs: Sales (192.168.30.1/24), Marketing (192.168.20.1/24)
Management (192.168.10.5/24)
DHCP pools for Sales & Marketing VLANs with Google DNS (8.8.8.8, 8.8.4.4)
ACL to block 38.98.0.111 while allowing other traffic
Dynamic NAT from inside to outside
Threat detection and protocol inspection (DNS, FTP, SIP, H323, SQLNet, etc.)
SSH management restricted to 192.168.10.0/24
Console always on

-Mikrotik Router Configuration
Dual WAN setup with failover (two modems)
Basic routing and network address translation
Screenshot included in the repository



These labs were part of my training program and helped me practice real world networking and security configurations

