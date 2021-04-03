Networking Requirements
=======================

  - Network routing with NAT translation in order to make connections from within the LAN outbound to the Internet.
  - Network switching that will allow for virtual local area networks (VLANs) to segment the various infrastructure and services on the network
  - Network port mirroring to allow packets to be copied over to a destination switch interface port where network traffic will be funneled through various network monitoring sensors.
  - Support for multiple wireless access point SSIDs

Virtualization Requirements
===========================

  - Hardware virtualization capable of supporting virtual networking appliances, specifically switches
  - Hardware virtualization capable of supporting pooled computing and storage resources
  - Hardware virtualization capable of supporting containerized workloads

Storage Requirements
====================

  - 24 hour rolling retention of full PCAP data
  - Three month rolling retention of source code commit history logs, CI/CD logs, and deployment logs
  - Six month rolling retention of endpoint access and authentication logs
  - Six month rolling retention of network access and authentication logs

Security Requirements
=====================
  - Least privileged access to all physical hosts, virtual hosts, and networking appliances
  - Authenticated access to all physical and virtual hosts
  - Jump host routing/proxy access to physical and virtual hosts
  - Whitelisted IP addressed of management devices
  - Full PCAP storage on security lab physical and virtual networks

Compliance Requirements
=======================
  - Logging for all physical endpoints, virtual endpoints, and containerized workloads
  - Log forwarding support for hardware firewall appliance, hypervisor hosts, wireless access points, virtual servers, and networked workstations
  - Key and secrets management integration into configuration management tool - ansible
