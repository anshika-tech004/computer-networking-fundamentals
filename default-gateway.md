## Default Gateway
- It is a device usually a router, that a host sends traffic to when the destination is outside its local network.
- Role- Routing traffic from your network to to other network.
- Different network → Default Gateway → Other network
 # Why we need default gateway
 - Situation1:
     - Suppose my laptop wants to send data to printer:
        - Laptop → 192.168.1.100
        - Printer → 192.168.1.103 (on same network)
        - Since both are in: 192.168.1.0/24 my laptop will directly communicate to printer
 - Situation2:
     - Suppose I want to send data to server on another network
        - Laptop → 192.168.1.10
        - Server on another network → 192.168.2.20
     - My laptop will send the packet to default gateway(router) which further will forward it to its destination.
 - Observation:
     - Default gateway acts as the exit point from the local network.
     - Devices use it to communicate with devices on other networks.

# What happens when Gateway is incorrect?
- A device may still communicate with same devices on its local network but may not be able to reach other network/ internet.
- Can cause connectivity problem outside local subnet
  
## How to check Default Gateway?

  ![screenshot1 using ipconfig in my command prompt](checking-Default-gateway)
  ![screenshot2 using ipconfig/all](default-gateway-check)
  ![screenshot3 part of screenshot2](default-gateway-checking)

# Troubleshooting 
- If a device can communicate with local devices but cannot reach another network check:
   - IP Address
   - Subnet Mask
   - Default Gateway
   - DNS configuration
   - Router connectivity
  
  
