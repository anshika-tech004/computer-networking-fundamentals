## Networking Devices
- They are the hardware components that connect devices
- Ensures that data reaches its correct destination efficiently

## Types of Networking Devices
- HUB
   -Connects multiple computer
   -Broadcasts data to all connected devices
   -OSI Layer- physical
   -cheap
   -Used to create LAN
   
  Drawback
  - half duplex: which means data cannot be sent and received simultaneously
  - data cannot be sent privately which means each connected device will receive it

    
    ![HUB figure](HUB.png)

- SWITCH
   -Connects devices within a single network 
   -Forwards data only to specific or intended user by identifying the MAC address where the data packets are to be sent
   - OSI Layer- Data Link layer
   - faster & efficient 
   - If a node fails there will be no effect on entire network

   Drawback
   - Difficult to setup
   - Expensive

      ![switch figure](switch.png)

- ROUTER
   - Chooses a traffic free path through which data packet will travel
   - Distributes the internet to the devices
   - Connects different network together
   - OSI Layer- Network Layer
   - Can work in LAN and WAN both

   Drawback
  - Expensive
  - Security issue


- MODEM (Modulator & Demodulator)
   -It brings Internet to the house while the router distributes it to the respective devices
        or
   -Device that connects your home/office network to ISP by converting signal from
           digital to analog (Modulator)
           analog to digital (demodulator)
   -OSI Layer- Physical and Data link layer

   ![modem working](modem.png)

   (my understanding) about above 3
   - Modem- main water meter that brings water from city to home
   - Router- distributes that water to rooms
   - Switch- extra splitter that adds more outlet within house      


- REPEATER
   - Boosts/regenerates weak signal
   - OSI Layer- Physical
   - Uses no address
   - Example- Suppose my wifi signal is strong in living room but weak in bedroom so I'll use repeater to boost the signal

  ![Repeater working](repeater.png)


- BRIDGE
    - Connects 2 LAN segments
    - OSI layer- Data Link Layer
    - can only have 2-4 ports only
     
   Working: 
      It collects data from LAN1 examines it, then notes the MAC address & port number  of destination (LAN2) & then
     forwards the data to LAN2

   ![Bridge working](bridge.png)


- GATEWAY
    - Connects similar/disimilar netowrks
    - Acts as a path or door for devices to reach external networks
    - OSI Layer-  ALL

   ![Gateway](gateway.png)


## Comparison 

 | Device | Main Purpose | OSI Layer | Uses | 
 |---|---|---|---|
 | HUB | Broadcasts data to all computer | Physical (layer1) | Signals |
 | Switch | Connects devices in a LAN & sends data only to the intended user | Data Link Layer (Layer2) | MAC address |
 | Router | Connects different network | Network layer (layer3) | IP address |
 | Modem | Connects to ISP network | Physical & Data link layer | ISP access |
 | Repeater | Regenerates signal | Physical (layer1) | signals |
 | Bridge | Connects LAN segments | Data link layer (layer2) | MAC address |
 | Gateway | Connects similar or dissimilar networks | All | IP/Protocols |

 ## My learning
 I learned how different networking devices work together to enable communication between devices and network.
   - HUB- understood basic broadcasting of data and why it's inefficient.
   - Switch- understood that it's faster and efficient and only transfers data to the intended user.
   - Router- Understood how routers use IP addresses to communicate between different networks.
   - Repeater- Learned how signal regeneration helps extend network communication over greater distances.
   - Bridge- Understood how bridges connect and filter traffic between network segments.
   - Gateway- Learned that a gateway acts as an entry and exit point between different networks.
   - Modem- Learned how a network connects to an ISP's access network.
 
 

 

  
     

      

        

   
     
