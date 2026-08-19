## TCP/IP Model    (4 layers)
- It is a practical system used to communicate across internet

## Layers of TCP/IP Model 
# layer4 (Application layer)
  - Provides service to user application
  - Protocols- HTTP, HTTPS, DNS, SSH, FTP
  - Ex- Opening a website in a browser
# layer3 (Transport layer)
  - End to end communication
  - ensures reliable and fast data delivery
  - Protocols- TCP, UDP
  - Ex- sending email(TCP), streaming video(UDP)
# layer2 (Internet layer)
  - Ensures addressing and routing data packets
  - Protocols- IPv4, IPv6
  - Ex- Finding best path for data to reach its destination
# layer1 (Network layer)
  - Handles data transmission over physical network
  - Through- Ethernet, wifi, ARP
  - Ex- Sending data through a network cable or wireless connection


## TCP/IP----OSI Layer mapping
| TCP/IP | OSI | What it does |
|-----|-----|-----|
|Application| 7. Application, 6. Presentation, 5. Session | service to user application, data format, manages session|
|Transport| 4. Transport | End to end delivery, TCP/UDP |
|Internet | 3. Network | IP addressing and routing |
|Network access | 2. Data link layer, 1. Physical layer| Frames, MAC address, signals, cables, radio |


## Common Protocols
|Protocol|Layer|Purpose|
|----|----|----|
|HTTP |Application |web communication|
|HTTPS | Application | secure web communication|
|DNS| Application | Domain name to IP address|
|SSH| Application | secure remote access |
|TCP| Transport | reliable, connection oriented |
|UDP| Transport | fast, connectionless communication|
|IP| Internet | addressing and routing packets|
|Ethernet | Network access | LAN communication |


## TCP VS UDP
|TCP |UDP |
|---|---|
|Connection oriented |connectionless |
|reliable | no delivery guarantee|
| more overhead | lower overhead|
| ex- file transfer, webpage, email | ex- streaming videos, online gaming|
|Data unit- segment| Data unit- Datagram|
|slow | fast |


## TCP/IP Model Encapsulation
- Suppose you send an HTTP request
    - Application layer 
       - http data
    - Transport layer
        - TCP Header + HTTP Data
    - Internet layer
        - IP Header + TCP Header + HTTP data
    - Network access layer
        - Ethernet Header + IP header + TCP header + HTTP data + trailer


## TCP/IP Model Decapsulation
   # Network Access Layer (L1)
   - ethernet header + IP Header + TCP Header + HTTP data + trailer
                - ( remove ethernet header)
   # Internet Layer (L2)
  - IP Header + TCP header + HTTP Header  
           - ( remove IP header)
   # Transport Layer (L3)
  - TCP header + HTTP header
           - (remove TCP header)
   # Application Layer (L1)
  - HTTP data
           - ( remove HTTP header)


## Real world example of TCP/IP Model- YouTube
   # Application layer (Browser requests the service)
  - Protocol- HTTPS+DNS
   # Transport Layer (end to end transport)
  - Protocol- TCP/UDP
   # Internet Layer (addressing and routing)
   - Protocol- IP
   # Network Access Layer (Data travelling physically over internet)
   - Protocol/ networking technologies - wifi/ethernet

                 
