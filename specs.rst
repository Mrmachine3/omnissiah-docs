Hardware Requirements
=====================

* Edge router
* Intel NUC-like desktop server

Networking Requirements
=======================

* Software firewall (pfSense) that  supports network routing with NAT translation in order to make connections from within the data center outbound to the Internet.
* Network switching that will allow for virtual local area networks (VLANs) to segment the various infrastructure and services on the network
* Network port mirroring to allow packets to be copied over to a destination switch interface port where network traffic will be funneled through various network monitoring sensors.
* Support for multiple wireless access point SSIDs

Virtualization Requirements
===========================

* Virtualization software supporting software-based network appliances, specifically switches, VPNs, VLANs
* Virtualization software supporting pooled computing and storage resources
* Virtualization software supporting containerized workloads

Storage Requirements
====================

* 24 hour rolling retention of full PCAP data
* Three month rolling retention of zeek logs
* Three month rolling retention of source code CI/CD build logs
* Six month rolling retention of endpoint security event logs
* Twelve month rolling retention of source code commit history logs
* Twelve month rolling retention of metric data

Security Requirements
=====================

* Least privileged access to all physical hosts, virtual hosts, and networking appliances
* Authenticated access to all physical and virtual hosts
* Jump host server deployed in cloud 
* Jump host proxied access to data center remote access control server
* SSH access to data center physical and virtual hosts managed by pre-shared SSH keys
* Multi-factor authentication for all web-based services
* Firewall rules for authorized IPs by machine
* Full PCAP storage on security lab physical and virtual networks

Compliance Requirements
=======================

* Security logging for all physical endpoints, virtual endpoints, and containerized workloads
* Performance logging for all physical endpoints, virtual endpoints, and containerized workloads
* Log forwarding support for hardware firewall appliance, hypervisor hosts, wireless access points, virtual servers, and networked workstations
* Key and secrets management integration into configuration management tool - ansible
