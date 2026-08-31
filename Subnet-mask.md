## Subnet Mask
- Tells a computer which part of IP address represents network and which part represents host.
- Used in- IPv4
- Example 1:
     - IP Address: 172.16.5.20
     - Default Subnet Mask:255.255.0.0
          - 172.16.5= Network portion
          - 20= Host portion
    - IP Address: 192.168.1.10
    - Default Subnet Mask: 255.255.255.0
          - 192.168.1= Network portion
          - 10= Host portion

# Why we need?
- To know whether the destination device there on my local network or do I need to send the packet to a router

## Network Portion VS Host Portion
|Basis |Network Portion| Host Portion|
|----|----|----|
|Meaning | Identifies the network| Identifies specific device on network|
|Uniqueness| Same for devices in same network| Different for each device in same network|
|Analogy| street/city| House no.|
|Assigned to| Network| Individual device|
|Example| IP Address: 192.168.1.25/24, Network portion: 192.168.1| IP Address: 192.168.1.25/24, Host Portion: 10|

