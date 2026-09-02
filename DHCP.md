## DHCP (Dynamic Host Configuration Protocol)
- Its a protocol that automatically provides network configuration (IP Address, Subnet Mask, Default Gateway and server) to network clients.
- Instead of manually configuring each device, DHCP allows a DHCP server to provide configuration automatically.
- Example:
    - IP address- 192.168.1.20
    - Subnet Mask- 255.255.255.0
    - Default Gateway- 192.168.1.1
    - DNS server- 8.8.8.8
 
## DHCP Client
- UDP Port- 68
- The device requesting network configuration
- Example- Laptop, Desktop, Phones, Printer

## DHCP Server
- UDP Port- 67
- Device that provides network configuration
- Example: In home network router acts as a DHCP server

## DHCP DORA Process
- DORA= Discover → Offer → Request → Acknowledgment
   - Discover- The client searches for an available DHCP server.
   - DHCP Offer- The DHCP server offers an IP address and network configuration
   - Request- The client requests/chooses the offered configuration.
   - Acknowledgment- DHCP server confirms

## DHCP Lease
- DHCP usually doesn't give a device an IP address permanently. It gives the address for a certain period called lease
- It is basically a time period till which the assigned IP address remain valid
- Example- IP Address: 192.168.1.20 , lease time: 8 hrs

## DHCP Address Pool
- DHCP server usually has a range of addresses that it is allowed to distribute
- DHCP Pool: 192.168.1.100 to 192.168.1.200
- DHCP Server can assign addresses from this pool

## DHCP Reservation
- It allows a specific device to consistently receive a particular IP address, usually based on its MAC address.
- Example- Printer MAC address → DHCP Reservation → 192.168.1.50

## DHCP VS Static IP
|DHCP| Static IP|
|----|----|
|Automatically configured| Manually configured|
|Address may change| Usually remain fixed|
|Uses DHCP server| Doesn't require DHCP|
|Easier to manage| Require manual configuration|
Common for client devices| Common for servers|

## DHCP Troubleshooting
- If a client cannot obtain an IP address through DHCP, possible cause includes:
    - DHCP server unavailable
    - DHCP pool exhausted
    - Network connectivity problem
    - VLAN/ network configuration issue
    - DHCP service failure
