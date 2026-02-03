
## Overview
This lab demonstrates inter-VLAN routing using the router-on-a-stick method. Two VLANs (HR and IT) are configured across two switches with a trunk link, and a router provides routing between VLANs using subinterfaces and 802.1Q tagging.

## Topology
![Topology](screenshots/topology.png)

## VLANs
### Switch1 VLANs
![Switch1 VLAN](screenshots/switch1_vlan.png)

### Switch2 VLANs
![Switch2 VLAN](screenshots/switch2_vlan.png)

## Trunking
### Switch1 Trunk
![Switch1 Trunk](screenshots/switch1_trunk.png)

### Switch2 Trunk
![Switch2 Trunk](screenshots/switch2_trunk.png)

## Router Configuration
### Router Interfaces
![Router IP Interface Brief](screenshots/router_ip_int_brief.png)

## Connectivity Test
### Inter-VLAN Ping Success
![Ping Test](screenshots/ping_success.png)

## Skills Demonstrated
- VLAN creation and port assignment
- Trunking (802.1Q)
- Router-on-a-stick subinterfaces
- Inter-VLAN routing
- Connectivity testing and troubleshooting

## Troubleshooting
### Issue:
Devices could not ping across VLANs.

### Cause:
Trunk link was not allowing VLAN 10 and 20.

### Fix:
Configured allowed VLANs on trunk ports using: switchport trunk allowed vlan 10,20
