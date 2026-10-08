# enterprise-network-eve-ng
Multi-branch enterprise network in EVE-NG: VLAN, OSPF, GRE, NAT, ACL and Layer 2 security (Cisco IOS)
# Enterprise Network Design: HQ and Branches (EVE-NG)

Design and implementation of a multi-branch enterprise network in EVE-NG, covering LAN, WAN, routing, internet access and security.

![Topology](images/topology.png)

## Highlights
- **LAN:** VLAN, Trunk, EtherChannel (LACP), Inter-VLAN Routing, RSTP with Root Bridge
- **WAN:** GRE tunnels over L3 ISP cloud with TDM backup link, OSPF (multi-area), tuned timers (failure detection reduced from 30s to 6s)
- **Internet:** PAT for users, Static NAT for DMZ services
- **Access control:** Extended ACLs for Local, DMZ and Network servers
- **Layer 2 security:** SSH, Port Security, DHCP Snooping, Dynamic ARP Inspection, BPDU Guard, CDP/LLDP disabled on external ports

## Tools
Cisco IOS, EVE-NG

## Documentation
Full step-by-step documentation (goal, configuration, verification and result for each step) is in [docs/Technical_Report.pdf](docs/Technical_Report.pdf) (Persian).
## Device Configurations
Final configuration of every device is available in the [configs/](configs/) folder (switches and routers of HQ, Branch 1, Branch 2 and ISP).

## Note
This is a lab environment. Passwords in the configs are for lab use only.
