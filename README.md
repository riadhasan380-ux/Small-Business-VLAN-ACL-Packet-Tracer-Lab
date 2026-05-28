# Small Business VLAN + ACL Lab

This is a Packet Tracer lab I built while practicing networking basics.

The goal was to make a small business network with separate VLANs for Admin, Employees, Guests, and the Server/Printer side.

## What I set up

- VLAN 10 for Admin
- VLAN 20 for Employees
- VLAN 30 for Guest users
- VLAN 40 for Server/Printer
- DHCP so the PCs get IP addresses automatically
- Router-on-a-stick so the VLANs can route through the router
- An ACL to block Guest users from reaching internal devices

## What I tested

I tested the network before and after adding the ACL.

Before the ACL, the Guest PC could reach internal devices.

After adding the ACL, the Guest PC could not reach the server or employee network anymore.

Admin and Employee PCs could still reach the server.

## Main takeaway

This helped me understand how VLANs separate devices into different networks, and how ACLs can control what traffic is allowed or blocked.
