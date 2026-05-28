# Small Business VLAN + ACL Lab

This is a Packet Tracer lab I built while practicing networking.

I wanted to understand how a small business network could be set up with different groups separated, like Admin, Employees, Guests, and the Server/Printer side.

**Tools:** Cisco Packet Tracer  
**Practiced:** VLANs, trunking, DHCP, router-on-a-stick, and ACLs

## What I set up

- VLAN 10 for Admin
- VLAN 20 for Employees
- VLAN 30 for Guest users
- VLAN 40 for Server/Printer
- DHCP so the PCs get IP addresses automatically
- Router-on-a-stick so the VLANs can communicate
- An ACL to block Guest users from reaching internal devices

## IP setup

| VLAN | Name | Subnet |
|---|---|---|
| 10 | Admin | 192.168.10.0/24 |
| 20 | Employees | 192.168.20.0/24 |
| 30 | Guest | 192.168.30.0/24 |
| 40 | Server/Printer | 192.168.40.0/24 |

## What I tested

I tested it before and after adding the ACL.

Before the ACL, the Guest PC could reach the server and employee network.

After I added the ACL, the Guest PC was blocked from reaching those internal devices.

Admin and Employee PCs could still reach the server, so the ACL only blocked the Guest side like I wanted.

## Main takeaway

This lab helped me understand VLANs better. VLANs separate the network, but ACLs are what control who can actually access what.
