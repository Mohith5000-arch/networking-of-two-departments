# networking-of-two-departments
Cisco Packet Tracer project connecting Accounts and Delivery departments through a router.
Accounts and Delivery Department Network

Project Overview

This project documents the subnetting plan for connecting the Accounts and Delivery departments. The network address used is 192.168.40.0, divided into two subnets so that each department can use a separate IP address range.

Subnetting Calculation

There are 2 departments, so 2 subnets are required.

Number of required subnets: 2

Subnet calculation: 2^n = 2

Therefore, n = 1 borrowed bit.

Subnet mask in binary: 11111111.11111111.11111111.10000000

Subnet mask in decimal: 255.255.255.128

CIDR prefix: /25

Subnet 1

Network ID -192.168.40.0/25
Subnet mask -255.255.255.128
Usable host IP range -192.168.40.1 – 192.168.40.126
Broadcast ID -192.168.40.127

Subnet 2


Network ID -192.168.40.128/25

Subnet mask -255.255.255.128

Usable host IP range -192.168.40.129 – 192.168.40.254

Broadcast ID -192.168.40.255

How This Supports the Project

The two subnets provide separate IP address ranges for the two departments. A router can be configured with an interface in each subnet to route traffic between them.

Planned Network

Accounts: 192.168.40.0/25

Delivery: 192.168.40.128/25

Routing device: Router with one interface in each subnet

Validation

After configuring the router and end devices in Cisco Packet Tracer, test communication between PCs in different departments using ping. 
