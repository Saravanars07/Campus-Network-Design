# Campus Network Design with Inter-VLAN Routing, VTP, ACL, DHCP, and /25 Subnetting

## Project Overview
This project simulates a campus network in Cisco Packet Tracer using inter-VLAN routing, VTP, ACLs, DHCP, and /25 subnetting.  
The network is divided into multiple departments such as HR, DEV, TEST, and ACC to improve security, scalability, and traffic management.

## Objectives
- Create VLAN-based department separation.
- Enable communication between VLANs using inter-VLAN routing.
- Use VTP for centralized VLAN management.
- Apply ACLs to control access between departments.
- Configure DHCP for automatic IP assignment.
- Use /25 subnetting for efficient IP utilization.

## Topology Summary
- 1 Router
- Multiple Switches
- Multiple PCs
- VLAN-based segmentation

## Technologies Used
- VLAN
- Trunking
- Inter-VLAN Routing
- VTP
- ACL
- DHCP
- Subnetting /25

## Department VLANs
- VLAN 10 – HR
- VLAN 20 – DEV
- VLAN 30 – TEST
- VLAN 40 – ACC

## IP Addressing Plan
- VLAN 10: 192.168.10.0/25
- VLAN 20: 192.168.10.128/25
- VLAN 30: 192.168.11.0/25
- VLAN 40: 192.168.11.128/25

## Features
- Secure VLAN segmentation
- Dynamic IP assignment using DHCP
- Traffic filtering using ACL
- Efficient addressing using /25 subnetting
- Central VLAN management using VTP
- Inter-VLAN communication using router subinterfaces

 ## Verification Commands
 - router
   ```
   show ip interface brief
   show ip route
   show running-config
    show ip dhcp binding
    show access-lists
    ```
  - Switch
    ```
    show vlan brief
    show interfaces trunk
    show vtp status
    show running-config
    ```
## Testing
- Ping between PCs in same VLAN
- Ping between different VLANs
- Verify DHCP IP allocation
- Check ACL restrictions
- Verify VLAN propagation through VTP

## Conclusion
This project demonstrates a real-world style campus network design and strengthens practical knowledge of Cisco switching, routing, security, and IP planning.
